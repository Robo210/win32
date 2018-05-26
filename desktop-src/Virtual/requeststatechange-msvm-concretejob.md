---
title: RequestStateChange method of the Msvm\_ConcreteJob class
description: Requests that the state of the job be changed to the value specified.
ms.assetid: aa091976-acb2-40ab-9481-0237835bb45b
keywords:
- RequestStateChange method Hyper-V
- RequestStateChange method Hyper-V , Msvm_ConcreteJob class
- Msvm_ConcreteJob class Hyper-V , RequestStateChange method
topic_type:
- apiref
api_name:
- Msvm_ConcreteJob.RequestStateChange
api_location:
- Root\Virtualization
api_type:
- COM
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# RequestStateChange method of the Msvm\_ConcreteJob class

Requests that the state of the job be changed to the value specified in the *RequestedState* parameter. Invoking the **RequestStateChange** method multiple times could result in earlier requests being overwritten or lost. If 0 is returned, then the task completed successfully. Any other return code indicates an error condition.

## Syntax


```mof
uint32 RequestStateChange(
  [in] uint16   RequestedState,
  [in] datetime TimeoutPeriod
);
```



## Parameters

<dl> <dt>

*RequestedState* \[in\]
</dt> <dd>

Type: **uint16**

The new state of a job.

<dt>

<span id="Start"></span><span id="start"></span><span id="START"></span>

<span id="Start"></span><span id="start"></span><span id="START"></span>**Start** (2)


</dt> <dd>

Changes the state to "Running".

</dd> <dt>

<span id="Suspend"></span><span id="suspend"></span><span id="SUSPEND"></span>

<span id="Suspend"></span><span id="suspend"></span><span id="SUSPEND"></span>**Suspend** (3)


</dt> <dd>

Stops the job temporarily. The intention is to subsequently restart the job with "Start". It might be possible to enter the "Service" state while suspended. (This is job-specific.)

</dd> <dt>

<span id="Terminate"></span><span id="terminate"></span><span id="TERMINATE"></span>

<span id="Terminate"></span><span id="terminate"></span><span id="TERMINATE"></span>**Terminate** (4)


</dt> <dd>

Stops the job cleanly, saving data, preserving the state, and shutting down all underlying processes in an orderly manner.

</dd> <dt>

<span id="Kill"></span><span id="kill"></span><span id="KILL"></span>

<span id="Kill"></span><span id="kill"></span><span id="KILL"></span>**Kill** (5)


</dt> <dd>

Terminates the job immediately with no requirement to save data or preserve the state.

</dd> <dt>

<span id="Service"></span><span id="service"></span><span id="SERVICE"></span>

<span id="Service"></span><span id="service"></span><span id="SERVICE"></span>**Service** (6)


</dt> <dd>

Puts the job into a vendor-specific service state. It might be possible to restart the job.

</dd> <dt>

<span id="DMTF_Reserved"></span><span id="dmtf_reserved"></span><span id="DMTF_RESERVED"></span>

<span id="DMTF_Reserved"></span><span id="dmtf_reserved"></span><span id="DMTF_RESERVED"></span>**DMTF Reserved**


</dt> <dd>

Reserved.

</dd> <dt>

<span id="Vendor_Reserved"></span><span id="vendor_reserved"></span><span id="VENDOR_RESERVED"></span>

<span id="Vendor_Reserved"></span><span id="vendor_reserved"></span><span id="VENDOR_RESERVED"></span>**Vendor Reserved**


</dt> <dd>

Reserved.

</dd> </dl> </dd> <dt>

*TimeoutPeriod* \[in\]
</dt> <dd>

Type: **datetime**

A timeout period that specifies the maximum amount of time that the client expects the transition to the new state to take. The interval format must be used to specify the timeout period. A value of 0 or a null parameter indicates that the client has no time requirements for the transition. If this property does not contain 0 or **null** and the implementation does not support this parameter, a return code of 4098 (Use Of Timeout Parameter Not Supported) must be returned.

</dd> </dl>

## Return value

Type: **uint32**

This method returns one of the following values.

<dl> <dt>

**Completed with No Error** (32768)
</dt> <dt>

**Not Supported** (32769)
</dt> <dt>

**Unknown/Unspecified Error** (32770)
</dt> <dt>

**Cannot complete within Timeout Period** (32771)
</dt> <dt>

**Failed** (32772)
</dt> <dt>

**Invalid Parameter** (32773)
</dt> <dt>

**In Use** (32774)
</dt> <dt>

**Method Parameters Checked - Transition Started** (32775)
</dt> <dt>

**Invalid State Transition** (32776)
</dt> <dt>

**Use of Timeout Parameter Not Supported** (32777)
</dt> <dt>

**Busy** (32778)
</dt> <dt>

**Vendor Specific** (32768 65535)
</dt> </dl>

## Remarks

Access to the [**Msvm\_ConcreteJob**](msvm-concretejob.md) class might be restricted by UAC Filtering. For more information, see [User Account Control and WMI](https://msdn.microsoft.com/library/aa826699).

## Requirements



|                                     |                                                                                                      |
|-------------------------------------|------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | None supported<br/>                                                                            |
| Minimum supported server<br/> | Windows Server 2008<br/>                                                                       |
| End of client support<br/>    | None supported<br/>                                                                            |
| End of server support<br/>    | Windows Server 2012<br/>                                                                       |
| Namespace<br/>                | Root\\Virtualization<br/>                                                                      |
| MOF<br/>                      | <dl> <dt>WindowsVirtualization.mof</dt> </dl> |



## See also

<dl> <dt>

[**Msvm\_ConcreteJob**](msvm-concretejob.md)
</dt> </dl>

 

 




