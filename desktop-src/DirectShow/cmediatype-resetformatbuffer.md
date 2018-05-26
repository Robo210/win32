---
Description: The ResetFormatBuffer method deletes the format block. The method sets the cbFormat and pbFormat members of the AM\_MEDIA\_TYPE structure to NULL.
ms.assetid: 5eb6dfc8-cfba-41dd-b422-8fe93ca904c1
title: CMediaType.ResetFormatBuffer method
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# CMediaType.ResetFormatBuffer method

The `ResetFormatBuffer` method deletes the format block. The method sets the **cbFormat** and **pbFormat** members of the **AM\_MEDIA\_TYPE** structure to **NULL**.

## Syntax


```C++
void ResetFormatBuffer();
```



## Parameters

This method has no parameters.

## Return value

This method does not return a value.

## Requirements



|                    |                                                                                                                                                                                            |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>Mtype.h (include Streams.h)</dt> </dl>                                                                                     |
| Library<br/> | <dl> <dt>Strmbase.lib (retail builds); </dt> <dt>Strmbasd.lib (debug builds)</dt> </dl> |



## See also

<dl> <dt>

[**CMediaType Class**](cmediatype.md)
</dt> </dl>

 

 



