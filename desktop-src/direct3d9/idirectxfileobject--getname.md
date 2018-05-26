---
Description: Retrieves a pointer to a DirectX file objects name. Deprecated.
ms.assetid: feb3faa2-22b9-47ed-8a38-33092821d484
title: IDirectXFileObjectGetName method
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# IDirectXFileObject::GetName method

Retrieves a pointer to a DirectX file object's name. Deprecated.

## Syntax


```C++
HRESULT GetName(
  [out]     LPSTR   pstrNameBuf,
  [in, out] LPDWORD pdwBufLen
);
```



## Parameters

<dl> <dt>

*pstrNameBuf* \[out\]
</dt> <dd>

Type: **[**LPSTR**](winprog.windows_data_types)**

Pointer to the buffer in which the DirectX file object's name will be copied. Set to **NULL** if only the buffer length is needed.

</dd> <dt>

*pdwBufLen* \[in, out\]
</dt> <dd>

Type: **[**LPDWORD**](winprog.windows_data_types)**

Pointer to a DWORD specifying the length of the buffer pointed to by pstrNameBuf. The pdwBufLen parameter value will be modified to the buffer length needed to hold the object's name even if pstrNameBuf is **NULL**. In either case, the function will return DXFILEERR\_BADVALUE if the original value of pdwBufLen is not as large as or larger than the length needed to hold the object's name.

</dd> </dl>

## Return value

Type: **[**HRESULT**](455d07e9-52c3-4efb-a9dc-2955cbfd38cc)**

If the method succeeds, the return value is DXFILE\_OK. If the method fails, the return value can be one of the following values.DXFILEERR\_BADALLOC DXFILEERR\_BADVALUE

## Requirements



|                    |                                                                                       |
|--------------------|---------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>DXFile.h</dt> </dl>   |
| Library<br/> | <dl> <dt>D3dxof.lib</dt> </dl> |



## See also

<dl> <dt>

[IDirectXFileObject](idirectxfileobject.md)
</dt> </dl>

 

 



