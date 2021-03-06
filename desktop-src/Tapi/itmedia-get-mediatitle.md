---
description: The get\_MediaTitle method retrieves a textual title for the media that the application can use for informational or display purposes. This must be an ASCII convertible string if the character set is ASCII. Otherwise, it can be any BSTR string.
ms.assetid: c5567672-54f0-45d6-81d2-5a501a33c25f
title: ITMedia::get_MediaTitle method (Sdpblb.h)
ms.topic: reference
ms.date: 05/31/2018
---

# ITMedia::get\_MediaTitle method

\[ Rendezvous IP Telephony Conferencing controls and interfaces are not available for use in Windows Vista, Windows Server 2008, and subsequent versions of the operating system. The RTC Client API provides similar functionality.\]

The **get\_MediaTitle** method retrieves a textual title for the media that the application can use for informational or display purposes. This must be an ASCII convertible string if the character set is ASCII. Otherwise, it can be any **BSTR** string.

## Syntax


```C++
HRESULT get_MediaTitle(
  [out] BSTR *ppMediaTitle
);
```



## Parameters

<dl> <dt>

*ppMediaTitle* \[out\]
</dt> <dd>

Pointer to a **BSTR** containing the title of the media.

</dd> </dl>

## Return value

This method can return one of these values.



| Return code                                                                                   | Description                                                     |
|-----------------------------------------------------------------------------------------------|-----------------------------------------------------------------|
| <dl> <dt>**S\_OK**</dt> </dl>          | Method succeeded.<br/>                                    |
| <dl> <dt>**E\_POINTER**</dt> </dl>     | The *ppMediaTitle* parameter is not a valid pointer.<br/> |
| <dl> <dt>**E\_OUTOFMEMORY**</dt> </dl> | Insufficient memory exists to perform the operation.<br/> |
| <dl> <dt>**E\_FAIL**</dt> </dl>        | Unspecified error.<br/>                                   |
| <dl> <dt>**E\_NOTIMPL**</dt> </dl>     | This method is not yet implemented.<br/>                  |



 

## Remarks

The application must use [**SysFreeString**](/windows/win32/api/oleauto/nf-oleauto-sysfreestring) to free the memory allocated for the *ppMediaTitle* parameter.

## Requirements



| Requirement | Value |
|-------------------------|---------------------------------------------------------------------------------------|
| TAPI version<br/> | Requires TAPI 3.0 or later<br/>                                                 |
| Header<br/>       | <dl> <dt>Sdpblb.h</dt> </dl>   |
| Library<br/>      | <dl> <dt>Uuid.lib</dt> </dl>   |
| DLL<br/>          | <dl> <dt>Sdpblb.dll</dt> </dl> |



## See also

<dl> <dt>

[**ITMedia**](itmedia.md)
</dt> <dt>

[**ITMedia::Put\_MediaTitle**](itmedia-put-mediatitle.md)
</dt> </dl>

 

