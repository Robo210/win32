---
Description: Proxy function for the GetColorContexts method.
ms.assetid: 1925a64e-558d-4931-a3c3-b35d2b92a292
title: IWICBitmapFrameDecode\_GetColorContexts\_Proxy function
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# IWICBitmapFrameDecode\_GetColorContexts\_Proxy function

Proxy function for the [**GetColorContexts**](/windows/win32/Wincodec/nf-wincodec-iwicbitmapframedecode-getcolorcontexts?branch=master) method.

## Syntax


```C++
HRESULT IWICBitmapFrameDecode_GetColorContexts_Proxy(
  _In_    IWICBitmapFrameDecode *THIS_PTR,
  _In_    UINT                  cCount,
  _Inout_ IWICColorContext      **ppIColorContexts,
  _Out_   UINT                  *pcActualCount
);
```



## Parameters

<dl> <dt>

*THIS\_PTR* \[in\]
</dt> <dd>

Type: **[**IWICBitmapFrameDecode**](/windows/win32/Wincodec/nn-wincodec-iwicbitmapframedecode?branch=master)\***

Pointer to this [**IWICBitmapFrameDecode**](/windows/win32/Wincodec/nn-wincodec-iwicbitmapframedecode?branch=master) object.

</dd> <dt>

*cCount* \[in\]
</dt> <dd>

Type: **UINT**

The number of color contexts to retrieve.

This value must be the size of, or smaller than, the size available to *ppIColorContexts*.

</dd> <dt>

*ppIColorContexts* \[in, out\]
</dt> <dd>

Type: **[**IWICColorContext**](/windows/win32/Wincodec/nn-wincodec-iwiccolorcontext?branch=master)\*\***

A pointer that receives a pointer to the [**IWICColorContext**](/windows/win32/Wincodec/nn-wincodec-iwiccolorcontext?branch=master) objects.

</dd> <dt>

*pcActualCount* \[out\]
</dt> <dd>

Type: **UINT\***

A pointer that receives the number of color contexts contained in the image frame.

</dd> </dl>

## Return value

Type: **HRESULT**

If this function succeeds, it returns **S\_OK**. Otherwise, it returns an **HRESULT** error code.

## Remarks

## Requirements



|                                     |                                                                                                                                                                  |
|-------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows XP with SP2, Windows Vista \[desktop apps only\]<br/>                                                                                              |
| Minimum supported server<br/> | Windows Server 2008 \[desktop apps only\]<br/>                                                                                                             |
| DLL<br/>                      | <dl> <dt>Windowscodecs.dll; </dt> <dt>Wincodec.lib</dt> </dl> |



 

 



