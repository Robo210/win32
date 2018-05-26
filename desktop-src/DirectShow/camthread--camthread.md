---
Description: Destructor method.
ms.assetid: eed6c566-8a03-4a97-9d99-8e500ce2954c
title: CAMThread.~CAMThread destructor
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# CAMThread.~CAMThread destructor

Destructor method.

## Syntax


```C++
virtual ~CAMThread();
```



## Remarks

The destructor calls the [**CAMThread::Close**](camthread-close.md) method, which waits for the thread to exit.

## Requirements



|                    |                                                                                                                                                                                            |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>Wxutil.h (include Streams.h)</dt> </dl>                                                                                    |
| Library<br/> | <dl> <dt>Strmbase.lib (retail builds); </dt> <dt>Strmbasd.lib (debug builds)</dt> </dl> |



## See also

<dl> <dt>

[**CAMThread Class**](camthread.md)
</dt> </dl>

 

 



