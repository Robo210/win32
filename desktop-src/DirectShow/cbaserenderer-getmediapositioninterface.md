---
Description: The GetMediaPositionInterface method retrieves the filters IMediaPosition and IMediaSeeking interface pointers.
ms.assetid: aeca4484-cecc-4d07-aa77-56221ff75699
title: CBaseRenderer.GetMediaPositionInterface method
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# CBaseRenderer.GetMediaPositionInterface method

The `GetMediaPositionInterface` method retrieves the filter's [**IMediaPosition**](/windows/win32/Control/nn-control-imediaposition?branch=master) and [**IMediaSeeking**](/windows/win32/Strmif/nn-strmif-imediaseeking?branch=master) interface pointers.

## Syntax


```C++
virtual HRESULT GetMediaPositionInterface(
   REFIID riid,
   void   **ppv
);
```



## Parameters

<dl> <dt>

*riid* 
</dt> <dd>

Reference identifier of the interface.

</dd> <dt>

*ppv* 
</dt> <dd>

Address of a variable that receives the interface pointer.

</dd> </dl>

## Return value

Returns an **HRESULT** value. Possible values include those shown in the following table.



| Return code                                                                                   | Description                         |
|-----------------------------------------------------------------------------------------------|-------------------------------------|
| <dl> <dt>**S\_OK**</dt> </dl>          | Success.<br/>                 |
| <dl> <dt>**E\_OUTOFMEMORY**</dt> </dl> | Insufficient memory.<br/>     |
| <dl> <dt>**E\_NOINTERFACE**</dt> </dl> | Interface not supported.<br/> |



 

## Remarks

The filter delegates all seeking commands to a [**CRendererPosPassThru**](crendererpospassthru.md) object, which passes them upstream. This method creates the **CRendererPosPassThru** object, if it does not yet exist, and queries it for the requested interface.

The [**CBaseRenderer::m\_pPosition**](cbaserenderer-m-pposition.md) member variable stores a pointer to the **CRendererPosPassThru** object.

## Requirements



|                    |                                                                                                                                                                                            |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>Renbase.h (include Streams.h)</dt> </dl>                                                                                   |
| Library<br/> | <dl> <dt>Strmbase.lib (retail builds); </dt> <dt>Strmbasd.lib (debug builds)</dt> </dl> |



## See also

<dl> <dt>

[**CBaseRenderer Class**](cbaserenderer.md)
</dt> </dl>

 

 



