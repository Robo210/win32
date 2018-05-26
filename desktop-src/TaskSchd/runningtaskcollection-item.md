---
title: RunningTaskCollection.Item property
description: For scripting, gets the specified task from the collection.
ms.assetid: e82e7e1b-a3bd-4456-85a9-e0005f954618
keywords:
- Item property Task Scheduler
- Item property Task Scheduler , RunningTaskCollection object
- RunningTaskCollection object Task Scheduler , Item property
topic_type:
- apiref
api_name:
- RunningTaskCollection.Item
api_location:
- taskschd.dll
api_type:
- COM
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# RunningTaskCollection.Item property

For scripting, gets the specified task from the collection.

## Syntax


```VB
RunningTaskCollection.Item( _
  ByVal Index _
) As RunningTask
```



## Property value

A [**RunningTask**](runningtask.md) object that contains the requested context.

## Remarks

Collections are 1-based. In other words, the index for the first item in the collection is 1.

## Requirements



|                                     |                                                                                         |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista \[desktop apps only\]<br/>                                          |
| Minimum supported server<br/> | Windows Server 2008 \[desktop apps only\]<br/>                                    |
| Type library<br/>             | <dl> <dt>Taskschd.tlb</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Taskschd.dll</dt> </dl> |



## See also

<dl> <dt>

[Task Scheduler](task-scheduler-start-page.md)
</dt> </dl>

 

 




