---
Description: The CreateAudioMediaType function initializes a media type from a WAVEFORMATEX structure.
ms.assetid: 2571b7b4-86e9-443f-a99d-9ba48f469522
title: CreateAudioMediaType function
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# CreateAudioMediaType function

The **CreateAudioMediaType** function initializes a media type from a [**WAVEFORMATEX**](/windows/win32/mmreg/?branch=master) structure.

## Syntax


```C++
HRESULT STDAPI CreateAudioMediaType(
   const WAVEFORMATEX  *pwfx,
         AM_MEDIA_TYPE *pmt,
         BOOL          bSetFormat
);
```



## Parameters

<dl> <dt>

*pwfx* 
</dt> <dd>

Pointer to the supplied [**WAVEFORMATEX**](/windows/win32/mmreg/?branch=master) structure.

</dd> <dt>

*pmt* 
</dt> <dd>

Pointer to the [**AM\_MEDIA\_TYPE**](/windows/win32/strmif/ns-strmif-_ammediatype?branch=master) structure to initialize.

</dd> <dt>

*bSetFormat* 
</dt> <dd>

Flag indicating whether to initialize the format block. Specify **TRUE** to initialize it, or **FALSE** otherwise.

</dd> </dl>

## Return value

Returns E\_OUTOFMEMORY if memory could not be allocated for the format data; S\_OK otherwise.

## Remarks

If the *bSetFormat* parameter is **TRUE**, the method allocates the memory for the format block. If the *pmt* parameter already contains an allocated format block, a memory leak will occur. To avoid a memory leak, call [**FreeMediaType**](freemediatype.md) before calling this function. After the method returns, call **FreeMediaType** again to free the format block.

## Requirements



|                    |                                                                                                                                                                                            |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>Mtype.h (include Streams.h)</dt> </dl>                                                                                     |
| Library<br/> | <dl> <dt>Strmbase.lib (retail builds); </dt> <dt>Strmbasd.lib (debug builds)</dt> </dl> |



## See also

<dl> <dt>

[**Media Type Functions**](media-type-functions.md)
</dt> </dl>

 

 



