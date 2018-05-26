---
Description: Disables the Virtual Machine Queue (VMQ) on the network adapter.
ms.assetid: d24cbc66-4b92-40bf-90b8-cf5719b8e0a5
title: Disable method of the MSFT\_NetAdapterVmqSettingData class
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# Disable method of the MSFT\_NetAdapterVmqSettingData class

Disables the Virtual Machine Queue (VMQ) on the network adapter.

## Syntax


```mof
uint32 Disable(
  [out] string cmdletOutput
);
```



## Parameters

<dl> <dt>

*cmdletOutput* \[out\]
</dt> <dd>

Returns an embedded instance of a [**MSFT\_NetAdapterVmqSettingData**](msft-netadaptervmqsettingdata.md) class.

</dd> </dl>

## Requirements



|                                     |                                                                                              |
|-------------------------------------|----------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | None supported<br/>                                                                    |
| Minimum supported server<br/> | Windows Server 2012<br/>                                                               |
| Namespace<br/>                | Root\\StandardCimv2<br/>                                                               |
| MOF<br/>                      | <dl> <dt>NetAdapterCim.mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>NetAdapterCim.dll</dt> </dl> |



## See also

<dl> <dt>

[**MSFT\_NetAdapterVmqSettingData**](msft-netadaptervmqsettingdata.md)
</dt> </dl>

 

 



