---
title: Data Notification
description: Objects that consume data from an external source sometimes need to be informed when data in that source changes.
ms.assetid: 286a1ecf-5255-4443-a17d-5ffa55ed0be1
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# Data Notification

Objects that consume data from an external source sometimes need to be informed when data in that source changes. For example, a stock ticker tape viewer that relies on data in some spreadsheet needs to be notified when that data changes so it can update its display. Similarly, a compound document needs information about data changes in its embedded objects so that it can update its data caches. In cases such as this, where dynamic updating of data is desirable, sources of data require some mechanism of notifying data consumers of changes as they occur without obligating the consumers to drop everything in order to update their data. Ideally, having been notified that a change has occurred in the data source, a consuming object can ask for an updated copy at its leisure.

COM's mechanism for handling asynchronous notifications of this type is an object called an advise sink, which is simply any COM object that implements an interface called [**IAdviseSink**](/windows/win32/ObjIdl/nn-objidl-iadvisesink?branch=master). Consumers of data implement the **IAdviseSink**. They register to receive notifications by handing a pointer to the data object of interest.

The [**IAdviseSink**](/windows/win32/ObjIdl/nn-objidl-iadvisesink?branch=master) interfaces exposes the following methods for receiving asynchronous notifications:



| Method                                                      | Notifies the advise sink that                                            |
|-------------------------------------------------------------|--------------------------------------------------------------------------|
| [**OnDataChange**](/windows/win32/ObjIdl/nf-objidl-iadvisesink-ondatachange?branch=master)<br/> | The calling object's data has changed.<br/>                        |
| [**OnViewChange**](/windows/win32/ObjIdl/nf-objidl-iadvisesink-onviewchange?branch=master)<br/> | The instructions for drawing the calling object have changed.<br/> |
| [**OnRename**](/windows/win32/ObjIdl/nf-objidl-iadvisesink-onrename?branch=master)<br/>         | The calling object's moniker has changed.<br/>                     |
| [**OnSave**](/windows/win32/ObjIdl/nf-objidl-iadvisesink-onsave?branch=master)<br/>             | The calling object has been saved to persistent storage.<br/>      |
| [**OnClose**](/windows/win32/ObjIdl/nf-objidl-iadvisesink-onclose?branch=master)<br/>           | The calling object has been closed.<br/>                           |



 

As the table indicates, the [**IAdviseSink**](/windows/win32/ObjIdl/nn-objidl-iadvisesink?branch=master) interface exposes methods for notifying the advise sink of events other than changes in the calling object's data. The calling object can also notify the sink when the way in which it draws itself changes, or it is renamed, saved, or closed. These other notifications are used mainly or entirely in the context of compound documents, although the notification mechanism is identical. For more information on compound-document notifications, see "Compound Documents."

In order to take advantage of the advise sink, a data source must implement [**IDataObject::DAdvise**](/windows/win32/ObjIdl/nf-objidl-idataobject-dadvise?branch=master), [**IDataObject::DUnadvise**](/windows/win32/ObjIdl/nf-objidl-idataobject-dunadvise?branch=master), and [**IDataObject::EnumDAdvise**](/windows/win32/ObjIdl/nf-objidl-idataobject-enumdadvise?branch=master). A data consumer calls the **DAdvise** mothod to notify a data object that it wishes to be notified when the object's data changes. The consuming object calls the **DUnadvise** method to tear down this connection. Any interested party can call the **EnumDAdvise** method to learn the number of objects having an advisory connection with a data object.

When data changes at the source, the data object calls [**IAdviseSink::OnDataChange**](/windows/win32/ObjIdl/nf-objidl-iadvisesink-ondatachange?branch=master) on all data consumers that have registered to receive notifications. To keep track of advisory connections and manage the dispatch of notifications, data sources rely on an object called a *data advise holder*. You can create your own data advise holder by implementing the [**IDataAdviseHolder**](/windows/win32/ObjIdl/nn-objidl-idataadviseholder?branch=master) interface. Or, you can let COM do it for you by calling the helper function [**CreateDataAdviseHolder**](/windows/win32/ole2/nf-objbase-createdataadviseholder?branch=master).

## Related topics

<dl> <dt>

[Data Transfer](data-transfer.md)
</dt> </dl>

 

 




