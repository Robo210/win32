---
Description: The ReceiveConnection method accepts a connection from another pin. This method implements the IPinReceiveConnection method.
ms.assetid: f17e7d93-ac45-4b8a-98c6-0c76ec7117c9
title: CBasePin.ReceiveConnection method
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# CBasePin.ReceiveConnection method

The `ReceiveConnection` method accepts a connection from another pin. This method implements the [**IPin::ReceiveConnection**](/windows/win32/Strmif/nf-strmif-ipin-receiveconnection?branch=master) method.

## Syntax


```C++
HRESULT ReceiveConnection(
   IPin          *pConnector,
   AM_MEDIA_TYPE *pmt
);
```



## Parameters

<dl> <dt>

*pConnector* 
</dt> <dd>

Pointer to the connecting pin's [**IPin**](/windows/win32/Strmif/nn-strmif-ipin?branch=master) interface.

</dd> <dt>

*pmt* 
</dt> <dd>

Pointer to an [**AM\_MEDIA\_TYPE**](/windows/win32/strmif/ns-strmif-_ammediatype?branch=master) structure that specifies the media type.

</dd> </dl>

## Return value

Returns an **HRESULT** value. Possible values include those in the following table.



| Return code                                                                                                | Description                                                                        |
|------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------|
| <dl> <dt>**S\_OK**</dt> </dl>                       | Success.<br/>                                                                |
| <dl> <dt>**E\_POINTER**</dt> </dl>                  | **NULL** pointer argument.<br/>                                              |
| <dl> <dt>**VFW\_E\_ALREADY\_CONNECTED**</dt> </dl>  | The pin is already connected.<br/>                                           |
| <dl> <dt>**VFW\_E\_NOT\_STOPPED**</dt> </dl>        | The filter is active and the pin does not support dynamic reconnection.<br/> |
| <dl> <dt>**VFW\_E\_TYPE\_NOT\_ACCEPTED**</dt> </dl> | The specified media type is not acceptable.<br/>                             |



 

## Remarks

The output pin calls this method on the input pin. If the input pin returns an error code, the connection fails.

In the base class, this method performs the following steps:

-   Checks whether the pin is already connected.
-   Checks whether the filter is stopped.
-   Calls the [**CBasePin::CheckConnect**](cbasepin-checkconnect.md) method to test whether the connecting pin is suitable.
-   Calls the [**CBasePin::CheckMediaType**](cbasepin-checkmediatype.md) method to test whether the media type is acceptable.

If all of these steps succeed, the method calls the [**CBasePin::CompleteConnect**](cbasepin-completeconnect.md) and [**SetMediaType**](cbasepin-setmediatype.md) methods to complete the connection. These methods store the media type and a pointer to the output pin.

If **CheckConnect** or **CheckMediaType** fail, the base class calls the [**CBasePin::BreakConnect**](cbasepin-breakconnect.md) method to break the connection and then returns an error code from `ReceiveConnection`.

## Requirements



|                    |                                                                                                                                                                                            |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>Amfilter.h (include Streams.h)</dt> </dl>                                                                                  |
| Library<br/> | <dl> <dt>Strmbase.lib (retail builds); </dt> <dt>Strmbasd.lib (debug builds)</dt> </dl> |



## See also

<dl> <dt>

[**CBasePin Class**](cbasepin.md)
</dt> </dl>

 

 



