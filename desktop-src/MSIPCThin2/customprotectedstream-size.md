---
title: CustomProtectedStream.Size property
description: Gets or sets the size of the protected data in bytes. Implements the IRandomAccessStream.Size property.
audience: developer
author: REDMOND\\bruceper
manager: REDMOND\\mbaldwin
ms.assetid: PMicrosoft.RightsManagement.CustomProtection.CustomProtectedStream.Size
ms.prod: windows-server-dev
ms.technology: active-directory-rights-management
ms.tgt_platform: multiple
keywords:
- Size property
- Size property, CustomProtectedStream class
- CustomProtectedStream class, Size property
topic_type:
- apiref
api_name:
- Microsoft.RightsManagement.CustomProtectedStream.Size
- Microsoft.RightsManagement.CustomProtectedStream.
- Microsoft.RightsManagement.CustomProtectedStream.
api_location:
- Microsoft.RightsManagement.dll
api_type:
- Assembly
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
---

# CustomProtectedStream.Size property

Gets or sets the size of the protected data in bytes. Implements the [IRandomAccessStream.Size](https://msdn.microsoft.com/library/windows/apps/windows.storage.streams.irandomaccessstream.size.aspx) property.

## Syntax


```C++
public:
property unsigned long long Size { 
   unsigned long long get();
   void set (unsigned long long value);
}
```



## Property value

Type: [UInt64](https://msdn.microsoft.com/library/system.uint64.aspx)

The size of the protected data in bytes.

## Remarks

> \[!Warning\]  
> To avoid data loss and/or corruption, [**FlushAsync**](customprotectedstream-flushasync.md) must be called if you modify the created stream or before object disposal.

 

## Requirements



|                                     |                                                                                                             |
|-------------------------------------|-------------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | None supported<br/>                                                                                   |
| Minimum supported server<br/> | None supported<br/>                                                                                   |
| Minimum supported phone<br/>  | Windows Phone 8.1<br/>                                                                                |
| Namespace<br/>                | Microsoft::RightsManagement<br/>                                                                      |
| Metadata<br/>                 | <dl> <dt>Microsoft.RightsManagement.winmd</dt> </dl> |



## See also

<dl> <dt>

[**CustomProtectedStream**](customprotectedstream.md)
</dt> </dl>

 

 




