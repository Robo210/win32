---
Description: The Notify method notifies the pin that a quality change is requested. This method implements the IQualityControlNotify method.
ms.assetid: 5e9394d9-8d3c-4091-b45f-345a3f7270db
title: CBasePin.Notify method
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# CBasePin.Notify method

The `Notify` method notifies the pin that a quality change is requested. This method implements the [**IQualityControl::Notify**](/windows/win32/Strmif/nf-strmif-iqualitycontrol-notify?branch=master) method.

## Syntax


```C++
HRESULT Notify(
   IBaseFilter *pSelf,
   Quality     q
);
```



## Parameters

<dl> <dt>

*pSelf* 
</dt> <dd>

Pointer to the [**IBaseFilter**](/windows/win32/Strmif/nn-strmif-ibasefilter?branch=master) interface of the filter that delivered the quality-control message.

</dd> <dt>

*q* 
</dt> <dd>

Specifies a [**Quality**](/windows/win32/strmif/ns-strmif-tagquality?branch=master) structure that contains the quality-control message.

</dd> </dl>

## Return value

The base class returns E\_NOTIMPL.

## Remarks

Output pins should override this method to accept quality-control messages.

If an external quality manager was installed (see [**CBasePin::SetSink**](cbasepin-setsink.md)), pass the message to that quality manager. Otherwise, the filter should handle the message itself, or pass the message upstream. For more information, see [Quality-Control Management](quality-control-management.md).

## Requirements



|                    |                                                                                                                                                                                            |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>Amfilter.h (include Streams.h)</dt> </dl>                                                                                  |
| Library<br/> | <dl> <dt>Strmbase.lib (retail builds); </dt> <dt>Strmbasd.lib (debug builds)</dt> </dl> |



## See also

<dl> <dt>

[**CBasePin Class**](cbasepin.md)
</dt> </dl>

 

 



