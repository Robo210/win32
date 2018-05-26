---
Description: The QueryPreferredFormat method retrieves the objects preferred time format. This method implements the IMediaSeekingQueryPreferredFormat method.
ms.assetid: 3b73b7cf-1ba7-47c5-8442-5f138b74f335
title: CSourceSeeking.QueryPreferredFormat method
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# CSourceSeeking.QueryPreferredFormat method

The `QueryPreferredFormat` method retrieves the object's preferred time format. This method implements the [**IMediaSeeking::QueryPreferredFormat**](/windows/win32/Strmif/nf-strmif-imediaseeking-querypreferredformat?branch=master) method.

## Syntax


```C++
HRESULT QueryPreferredFormat(
   GUID *pFormat
);
```



## Parameters

<dl> <dt>

*pFormat* 
</dt> <dd>

Pointer to a variable that receives a time format GUID. See [**Time Format GUIDs**](time-format-guids.md).

</dd> </dl>

## Return value

Returns one of the **HRESULT** values listed in the following table.



| Return code                                                                               | Description                       |
|-------------------------------------------------------------------------------------------|-----------------------------------|
| <dl> <dt>**S\_OK**</dt> </dl>      | Success<br/>                |
| <dl> <dt>**E\_POINTER**</dt> </dl> | **NULL** pointer value<br/> |



 

## Remarks

The only time format supported by the base class is TIME\_FORMAT\_MEDIA\_TIME (100-nanosecond units).

## Requirements



|                    |                                                                                                                                                                                            |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>Ctlutil.h (include Streams.h)</dt> </dl>                                                                                   |
| Library<br/> | <dl> <dt>Strmbase.lib (retail builds); </dt> <dt>Strmbasd.lib (debug builds)</dt> </dl> |



## See also

<dl> <dt>

[**CSourceSeeking Class**](csourceseeking.md)
</dt> </dl>

 

 



