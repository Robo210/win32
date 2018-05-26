---
Description: Retrieves the number of IContextNode objects contained in this collection.
ms.assetid: 7cc60bea-9a4c-4ac8-ad1a-0fca5e941c5e
title: IContextNodesGetCount method
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# IContextNodes::GetCount method

Retrieves the number of [**IContextNode**](icontextnode.md) objects contained in this collection.

## Syntax


```C++
HRESULT GetCount(
  [out] ULONG *pulCount
);
```



## Parameters

<dl> <dt>

*pulCount* \[out\]
</dt> <dd>

The number of [**IContextNode**](icontextnode.md) objects contained in this collection.

</dd> </dl>

## Return value

For a description of the return values, see [Classes and Interfaces - Ink Analysis](classes-and-interfaces---ink-analysis.md).

## Requirements



|                                     |                                                                                                               |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows XP Tablet PC Edition \[desktop apps only\]<br/>                                                 |
| Minimum supported server<br/> | None supported<br/>                                                                                     |
| Header<br/>                   | <dl> <dt>IACom.h (also requires IACom\_i.c)</dt> </dl> |
| DLL<br/>                      | <dl> <dt>IACom.dll</dt> </dl>                          |



## See also

<dl> <dt>

[**IContextNodes**](icontextnodes.md)
</dt> <dt>

[Ink Analysis Reference](ink-analysis-reference.md)
</dt> </dl>

 

 



