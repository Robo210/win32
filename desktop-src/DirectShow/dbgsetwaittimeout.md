---
Description: Sets the debugging time-out value. Ignored in retail builds.
ms.assetid: d0f60d8b-34f2-44b2-bdd6-5e8e6f7806d8
title: DbgSetWaitTimeout function
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# DbgSetWaitTimeout function

Sets the debugging time-out value. Ignored in retail builds.

## Syntax


```C++
void DbgSetWaitTimeout(
   DWORD dwTimeout
);
```



## Parameters

<dl> <dt>

*dwTimeout* 
</dt> <dd>

Time-out value in milliseconds, or INFINITE to wait indefinitely.

</dd> </dl>

## Return value

This function does not return a value.

## Remarks

In debug builds, the [**DbgWaitForMultipleObjects**](dbgwaitformultipleobjects.md) and [**DbgWaitForSingleObject**](dbgwaitforsingleobject.md) functions use this value as the time-out interval.

## Requirements



|                    |                                                                                                                                                                                            |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>Wxdebug.h (include Streams.h)</dt> </dl>                                                                                   |
| Library<br/> | <dl> <dt>Strmbase.lib (retail builds); </dt> <dt>Strmbasd.lib (debug builds)</dt> </dl> |



## See also

<dl> <dt>

[Wait Debugging Functions](wait-debugging-functions.md)
</dt> </dl>

 

 



