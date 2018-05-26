---
title: IAdminIndexServer MachineName property
description: Contains the case-insensitive name of the computer where Indexing Service is running.
ms.assetid: 064130a0-ece0-4593-a27e-a07e4cee3c0c
keywords:
- MachineName property Indexing Service
- MachineName property Indexing Service , IAdminIndexServer interface
- IAdminIndexServer interface Indexing Service , MachineName property
topic_type:
- apiref
api_name:
- IAdminIndexServer.MachineName
- IAdminIndexServer.get_MachineName
- IAdminIndexServer.put_MachineName
api_location:
- Ciodm.dll
api_type:
- COM
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# IAdminIndexServer::MachineName property

\[Indexing Service is no longer supported as of Windows XP and is unavailable for use as of Windows 8. Instead, use [Windows Search](https://msdn.microsoft.com/library/windows/desktop/aa965362) for client side search and [Microsoft Search Server Express]( http://go.microsoft.com/fwlink/p/?linkid=258445) for server side search.\]

Contains the case-insensitive name of the computer where Indexing Service is running. This property is read/write, but once it is set it cannot be changed. It identifies the computer that the administration object controls and can be set only once. If not set, the content index on the local computer is administered by default.

This property is read/write.

## Syntax


```C++
HRESULT put_MachineName(
  [in]          BSTR newVal
);

HRESULT get_MachineName(
  [out, retval] BSTR *pVal
);
```



## Property value

Specifies the name of the computer (can be done only once).

## Remarks

This property must be set to administer Indexing Service on remote computers. If this property is not set, the local computer is administered by default. The local computer name is represented by ".". Attempting to set this property more than once results in the creation of an error object with the **Number** property set to ERROR\_ALREADY\_INITIALIZED.

## Requirements



|                                     |                                                                                      |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 2000 Professional \[desktop apps only\]<br/>                           |
| Minimum supported server<br/> | Windows 2000 Server \[desktop apps only\]<br/>                                 |
| End of client support<br/>    | Windows 7<br/>                                                                 |
| End of server support<br/>    | Windows Server 2008 R2<br/>                                                    |
| DLL<br/>                      | <dl> <dt>Ciodm.dll</dt> </dl> |



## See also

<dl> <dt>

[**IAdminIndexServer**](iadminindexserver.md)
</dt> </dl>

 

 




