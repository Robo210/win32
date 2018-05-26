---
Description: Reads the access rules for a given type.
ms.assetid: fd569e7f-ca5c-4571-bbaa-c669e8780a97
title: IPStoreReadAccessRuleSet method
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# IPStore::ReadAccessRuleSet method

\[Protected Storage (Pstore) is available for use in Windows Server 2003 and Windows XP. It is only available for read-only operations in Windows Server 2008 and Windows Vista, but may be unavailable in subsequent versions. Pstore uses an older implementation of data protection. Developers are strongly encouraged to take advantage of the stronger data protection provided by the [**CryptProtectData**](security.cryptprotectdata) and [**CryptUnprotectData**](security.cryptunprotectdata) functions.\]

\[This method is not implemented.\]

Reads the access rules for a given type.

## Syntax


```C++
HRESULT ReadAccessRuleSet(
  [in]       PST_KEY            Key,
  [in] const GUID               *pType,
  [in] const GUID               *pSubtype,
  [in]       PPST_TYPEINFO      pInfo,
  [in]       PPST_ACCESSRULESET **ppRules,
  [in]       DWORD              dwFlags
);
```



## Parameters

<dl> <dt>

*Key* \[in\]
</dt> <dd>

Reserved.

</dd> <dt>

*pType* \[in\]
</dt> <dd>

Reserved.

</dd> <dt>

*pSubtype* \[in\]
</dt> <dd>

Reserved.

</dd> <dt>

*pInfo* \[in\]
</dt> <dd>

Reserved.

</dd> <dt>

*ppRules* \[in\]
</dt> <dd>

Reserved.

</dd> <dt>

*dwFlags* \[in\]
</dt> <dd>

Reserved.

</dd> </dl>

## Return value

Calls to this method will always fail.

## Requirements



|                   |                                                                                        |
|-------------------|----------------------------------------------------------------------------------------|
| Header<br/> | <dl> <dt>Pstore.h</dt> </dl>    |
| DLL<br/>    | <dl> <dt>Pstorec.dll</dt> </dl> |



## See also

<dl> <dt>

[**IPStore**](ipstore.md)
</dt> </dl>

 

 



