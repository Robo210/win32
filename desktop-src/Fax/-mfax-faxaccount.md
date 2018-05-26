---
Description: Represents a fax account on the server, including the accounts name, folders, and the events for which it is listening. It also provides a method for setting those events.
ms.assetid: 85adc440-3dc8-47ce-aae8-dfb04f824b09
title: FaxAccount object
ms.date: 05/31/2018
ms.topic: interface
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# FaxAccount object

Represents a fax account on the server, including the account's name, folders, and the events for which it is listening. It also provides a method for setting those events.

## Members

The **FaxAccount** object has these types of members:

-   [Methods](#methods)
-   [Properties](#properties)

### Methods

The **FaxAccount** object has these methods.



| Method                                                                     | Description                                                                                                                                                                           |
|:---------------------------------------------------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**ListenToAccountEvents**](-mfax-faxaccount-listentoaccountevents-vb.md) | Sets the flags of a [**FAX\_ACCOUNT\_EVENTS\_TYPE\_ENUM**](/windows/previous-versions/FaxComex/ne-faxcomex-fax_account_events_type_enum?branch=master) variable that represents the events for which the account is listening.<br/> |



 

### Properties

The **FaxAccount** object has these properties.



| Property                                                                    | Access type          | Description                                                                                                                          |
|:----------------------------------------------------------------------------|:---------------------|:-------------------------------------------------------------------------------------------------------------------------------------|
| [**AccountName**](-mfax-faxaccount-accountname-vb.md)<br/>           | Read-only<br/> | Retrieves the name of a particular fax account on the server.<br/>                                                             |
| [**Folders**](-mfax-faxaccount-folders-vb.md)<br/>                   | Read-only<br/> | Represents the folders of the account, including the incoming and outgoing archives and the incoming and outgoing queues.<br/> |
| [**RegisteredEvents**](-mfax-faxaccount-registeredevents-vb.md)<br/> | Read-only<br/> | A set of flags indicating the type of events for which the account is listening.<br/>                                          |



 

## Remarks

![faxaccounts, faxaccount, and faxaccountfolders](images/faxaccount.png)

To create a **FaxAccount** object in Microsoft Visual Basic or C++, call the [**AddAccount**](-mfax-faxaccountset-addaccount-vb.md) or [**GetAccount**](-mfax-faxaccountset-getaccount-vb.md) methods of the [**IFaxAccountSet**](/windows/previous-versions/FaxComex/nn-faxcomex-ifaxaccountset?branch=master) interface.

## Requirements



|                                     |                                                                                         |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista \[desktop apps only\]<br/>                                          |
| Minimum supported server<br/> | Windows Server 2008 \[desktop apps only\]<br/>                                    |
| Header<br/>                   | <dl> <dt>Faxcomex.h</dt> </dl>   |
| DLL<br/>                      | <dl> <dt>Fxscomex.dll</dt> </dl> |
| IID<br/>                      | CLSID\_FaxAccount<br/>                                                            |



## See also

<dl> <dt>

[**IFaxAccount**](/windows/previous-versions/FaxComex/nn-faxcomex-ifaxaccount?branch=master)
</dt> </dl>

 

 



