---
title: Msvm\_NetworkJob class
description: Represents a network operation job created by the Network VSP WMI management service.
ms.assetid: af2f23ed-026c-4154-b910-53aefc2cb71c
keywords:
- Msvm_NetworkJob class Hyper-V
- Msvm_NetworkJob class Hyper-V , described
topic_type:
- apiref
api_name:
- Msvm_NetworkJob
- Msvm_NetworkJob.KillJob
- Msvm_NetworkJob.RequestStateChange
- Msvm_NetworkJob.GetError
- Msvm_NetworkJob.Caption
- Msvm_NetworkJob.Description
- Msvm_NetworkJob.ElementName
- Msvm_NetworkJob.InstallDate
- Msvm_NetworkJob.OperationalStatus
- Msvm_NetworkJob.StatusDescriptions
- Msvm_NetworkJob.Status
- Msvm_NetworkJob.HealthState
- Msvm_NetworkJob.JobStatus
- Msvm_NetworkJob.TimeSubmitted
- Msvm_NetworkJob.ScheduledStartTime
- Msvm_NetworkJob.StartTime
- Msvm_NetworkJob.ElapsedTime
- Msvm_NetworkJob.JobRunTimes
- Msvm_NetworkJob.RunMonth
- Msvm_NetworkJob.RunDay
- Msvm_NetworkJob.RunDayOfWeek
- Msvm_NetworkJob.RunStartInterval
- Msvm_NetworkJob.LocalOrUtcTime
- Msvm_NetworkJob.UntilTime
- Msvm_NetworkJob.Notify
- Msvm_NetworkJob.Owner
- Msvm_NetworkJob.Priority
- Msvm_NetworkJob.PercentComplete
- Msvm_NetworkJob.DeleteOnCompletion
- Msvm_NetworkJob.ErrorCode
- Msvm_NetworkJob.ErrorDescription
- Msvm_NetworkJob.ErrorSummaryDescription
- Msvm_NetworkJob.RecoveryAction
- Msvm_NetworkJob.OtherRecoveryAction
- Msvm_NetworkJob.Name
- Msvm_NetworkJob.JobState
- Msvm_NetworkJob.TimeOfLastStateChange
- Msvm_NetworkJob.InstanceID
- Msvm_NetworkJob.TimeBeforeRemoval
- Msvm_NetworkJob.NetworkJobType
- Msvm_NetworkJob.CreatedInternalEthernetPort
- Msvm_NetworkJob.Hresult
api_location:
- Root\Virtualization
api_type:
- Schema
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# Msvm\_NetworkJob class

Represents a network operation job created by the Network VSP WMI management service.

The following syntax is simplified Managed Object Format (MOF) code, and it includes all of the inherited properties.

## Syntax

``` syntax
[Dynamic, Provider("VmmsWmiInstanceAndMethodProvider"), AMENDMENT]
class Msvm_NetworkJob : CIM_ConcreteJob
{
  string   Caption;
  string   Description;
  string   ElementName;
  datetime InstallDate;
  uint16   OperationalStatus[] = 2;
  string   StatusDescriptions[];
  string   Status;
  uint16   HealthState = 5;
  string   JobStatus;
  datetime TimeSubmitted;
  datetime ScheduledStartTime;
  datetime StartTime;
  datetime ElapsedTime;
  uint32   JobRunTimes = 1;
  uint8    RunMonth;
  sint8    RunDay;
  sint8    RunDayOfWeek;
  datetime RunStartInterval;
  uint16   LocalOrUtcTime;
  datetime UntilTime;
  string   Notify;
  string   Owner;
  uint32   Priority;
  uint16   PercentComplete;
  boolean  DeleteOnCompletion;
  uint16   ErrorCode;
  string   ErrorDescription;
  string   ErrorSummaryDescription;
  uint16   RecoveryAction;
  string   OtherRecoveryAction;
  string   Name;
  uint16   JobState;
  datetime TimeOfLastStateChange;
  string   InstanceID;
  datetime TimeBeforeRemoval = 00000000000500.000000:000;
  uint16   NetworkJobType;
  string   CreatedInternalEthernetPort;
  uint32   Hresult;
};
```

## Members

The **Msvm\_NetworkJob** class has these types of members:

-   [Methods](#methods)
-   [Properties](#properties)

### Methods

The **Msvm\_NetworkJob** class has these methods.



| Method                                           | Description                                                                                                                                                                                                                                                                                                                                                                                                                   |
|:-------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **GetError**                                     | When the job is executing or has terminated without error, then this method returns no [**CIM\_Error**](https://msdn.microsoft.com/library/mt445938) instance. However, if the job has failed because of some internal problem or because the job has been terminated by a client, then a **CIM\_Error** instance is returned. This method is inherited from [**CIM\_ConcreteJob**](https://msdn.microsoft.com/library/cc136808).<br/>                                        |
| [**GetErrorEx**](geterrorex-msvm-networkjob.md) | When the job is executing or has terminated without error, then this method returns no [**Msvm\_Error**](msvm-error.md) instance. However, if the job has failed because of some internal problem or because the job has been terminated by a client, then one or more **Msvm\_Error** instance is returned.<br/>                                                                                                      |
| **KillJob**                                      | This method is not supported.<br/>                                                                                                                                                                                                                                                                                                                                                                                      |
| **RequestStateChange**                           | Requests that the state of the job be changed to the value specified in the RequestedState parameter. Invoking the **RequestStateChange** method multiple times could result in earlier requests being overwritten or lost. If 0 is returned, then the task completed successfully. Any other return code indicates an error condition. This method is inherited from [**CIM\_ConcreteJob**](https://msdn.microsoft.com/library/cc136808).<br/> |



 

### Properties

The **Msvm\_NetworkJob** class has these properties.

<dl> <dt>

**Caption**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**MaxLen**](https://msdn.microsoft.com/library/aa393650) (64)
</dt> </dl>

A short textual description (one-line string) of the object. This property is inherited from [**CIM\_ManagedElement**](https://msdn.microsoft.com/library/cc136871).

</dd> <dt>

**CreatedInternalEthernetPort**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> </dl>

The **NvspWmiJobTypeSetupSwitch** job (**NetworkJobType** = 1) will create a [**Msvm\_InternalEthernetPort**](msvm-internalethernetport.md) as a part of the job. This property can be used to find the reference to the created Ethernet port.

</dd> <dt>

**DeleteOnCompletion**
</dt> <dd> <dl> <dt>

Data type: **boolean**
</dt> <dt>

Access type: Read/write
</dt> </dl>

This property is inherited from [**CIM\_Job**](https://msdn.microsoft.com/library/aa387873).

</dd> <dt>

**Description**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> </dl>

A textual description of the object. This property is inherited from [**CIM\_ManagedElement**](https://msdn.microsoft.com/library/cc136871).

</dd> <dt>

**ElapsedTime**
</dt> <dd> <dl> <dt>

Data type: **datetime**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**SubType**](https://msdn.microsoft.com/library/aa393651) ("Interval")
</dt> </dl>

The length of time that the job has been executing. This property is inherited from [**CIM\_Job**](https://msdn.microsoft.com/library/aa387873).

</dd> <dt>

**ElementName**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> </dl>

A user-friendly name for the object. This property is inherited from [**CIM\_ManagedElement**](https://msdn.microsoft.com/library/cc136871).

</dd> <dt>

**ErrorCode**
</dt> <dd> <dl> <dt>

Data type: **uint16**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**ModelCorrespondence**](https://msdn.microsoft.com/library/aa393650) ("[**CIM\_Job**](cim-job.md).**ErrorDescription**")
</dt> </dl>

This property is inherited from [**CIM\_Job**](https://msdn.microsoft.com/library/aa387873).

</dd> <dt>

**ErrorDescription**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**ModelCorrespondence**](https://msdn.microsoft.com/library/aa393650) ("[**CIM\_Job**](cim-job.md).**ErrorCode**")
</dt> </dl>

This property is inherited from [**CIM\_Job**](https://msdn.microsoft.com/library/aa387873).

</dd> <dt>

**ErrorSummaryDescription**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**ModelCorrespondence**](https://msdn.microsoft.com/library/aa393650) ("[**CIM\_Job**](cim-job.md).**ErrorCode**")
</dt> </dl>

This property is inherited from [**CIM\_Job**](https://msdn.microsoft.com/library/aa387873).

</dd> <dt>

**HealthState**
</dt> <dd> <dl> <dt>

Data type: **uint16**
</dt> <dt>

Access type: Read-only
</dt> </dl>

The current health of the element. This attribute expresses the health of this element but not necessarily that of its subcomponents. The possible values are 0 to 30, where 5 means the element is entirely healthy and 30 means the element is completely non-functional. This property is inherited from [**CIM\_ManagedSystemElement**](https://msdn.microsoft.com/library/aa387898) and it is always set to 5.

<dt>

<span id="OK"></span><span id="ok"></span>

<span id="OK"></span><span id="ok"></span>**OK** (5)


</dt> <dd>

The element is fully functional and operates within normal operational parameters and without error.

</dd> </dl>

</dd> <dt>

**Hresult**
</dt> <dd> <dl> <dt>

Data type: **uint32**
</dt> <dt>

Access type: Read-only
</dt> </dl>

The completion status of the job.

</dd> <dt>

**InstallDate**
</dt> <dd> <dl> <dt>

Data type: **datetime**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**MappingStrings**](https://msdn.microsoft.com/library/aa393650) ("MIF.DMTF\|ComponentID\|001.5")
</dt> </dl>

The date and time the virtual machine configuration was created. This property is inherited from [**CIM\_ManagedSystemElement**](https://msdn.microsoft.com/library/aa387898).

</dd> <dt>

**InstanceID**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**Key**](https://msdn.microsoft.com/library/aa392157)
</dt> </dl>

Within the scope of the instantiating Namespace, InstanceID opaquely and uniquely identifies an instance of this class. In order to ensure uniqueness within the NameSpace, the value of InstanceID SHOULD be constructed using the following 'preferred' algorithm: *OrgID*:*LocalID* Where *OrgID* and *LocalID* are separated by a colon ':', and where *OrgID* must include a copyrighted, trademarked or otherwise unique name that is owned by the business entity that is creating or defining the InstanceID, or that is a registered ID that is assigned to the business entity by a recognized global authority. (This requirement is similar to the *SchemaName*\_*ClassName* structure of Schema class names.) In addition, to ensure uniqueness *OrgID* must not contain a colon (':'). When using this algorithm, the first colon to appear in InstanceID must appear between *OrgID* and *LocalID*. *LocalID* is chosen by the business entity and should not be re-used to identify different underlying (real-world) elements. If the above 'preferred' algorithm is not used, the defining entity must assure that the resulting InstanceID is not re-used across any InstanceIDs produced by this or other providers for the NameSpace of this instance. For DMTF defined instances, the 'preferred' algorithm must be used with the *OrgID* set to 'CIM'. This property is inherited from [**CIM\_ConcreteJob**](https://msdn.microsoft.com/library/cc136808).

</dd> <dt>

**JobRunTimes**
</dt> <dd> <dl> <dt>

Data type: **uint32**
</dt> <dt>

Access type: Read/write
</dt> </dl>

This property is inherited from [**CIM\_Job**](https://msdn.microsoft.com/library/aa387873).

The possible values are.

<dt>



 (0)


</dt> <dd>

Repeat the job until the time specified by the **UntilTime** property or until it is manually shut down.

</dd> <dt>



 (1)


</dt> <dd>

Run the job once. This is the default value.

</dd> <dt>




</dt> <dd>

Run the job for the specified number of times.

</dd> </dl>

</dd> <dt>

**JobState**
</dt> <dd> <dl> <dt>

Data type: **uint16**
</dt> <dt>

Access type: Read-only
</dt> </dl>

The operational state of a job. It can also indicate transitions between these states, for example, 6 (Shutting Down) and 3 (Starting). This property is inherited from [**CIM\_ConcreteJob**](https://msdn.microsoft.com/library/cc136808).

The possible values are.

<dt>

<span id="New"></span><span id="new"></span><span id="NEW"></span>

<span id="New"></span><span id="new"></span><span id="NEW"></span>**New** (2)


</dt> <dd>

The job has never been started.

</dd> <dt>

<span id="Starting"></span><span id="starting"></span><span id="STARTING"></span>

<span id="Starting"></span><span id="starting"></span><span id="STARTING"></span>**Starting** (3)


</dt> <dd>

The job is moving from the **New**, **Suspended**, or **Service** states into the **Running** state.

</dd> <dt>

<span id="Running"></span><span id="running"></span><span id="RUNNING"></span>

<span id="Running"></span><span id="running"></span><span id="RUNNING"></span>**Running** (4)


</dt> <dd>

The Job is running.

</dd> <dt>

<span id="Suspended"></span><span id="suspended"></span><span id="SUSPENDED"></span>

<span id="Suspended"></span><span id="suspended"></span><span id="SUSPENDED"></span>**Suspended** (5)


</dt> <dd>

The Job is stopped, but can be restarted in a seamless manner.

</dd> <dt>

<span id="Shutting_Down"></span><span id="shutting_down"></span><span id="SHUTTING_DOWN"></span>

<span id="Shutting_Down"></span><span id="shutting_down"></span><span id="SHUTTING_DOWN"></span>**Shutting Down** (6)


</dt> <dd>

The job is moving to a **Completed**, **Terminated**, or **Killed** state.

</dd> <dt>

<span id="Completed"></span><span id="completed"></span><span id="COMPLETED"></span>

<span id="Completed"></span><span id="completed"></span><span id="COMPLETED"></span>**Completed** (7)


</dt> <dd>

The job has completed normally.

</dd> <dt>

<span id="Terminated"></span><span id="terminated"></span><span id="TERMINATED"></span>

<span id="Terminated"></span><span id="terminated"></span><span id="TERMINATED"></span>**Terminated** (8)


</dt> <dd>

The job has been stopped by a **Terminate** state change request. The job and all its underlying processes are ended and can be restarted (this is job-specific) only as a new job.

</dd> <dt>

<span id="Killed"></span><span id="killed"></span><span id="KILLED"></span>

<span id="Killed"></span><span id="killed"></span><span id="KILLED"></span>**Killed** (9)


</dt> <dd>

The job has been stopped by a **Kill** state change request. Underlying processes might have been left running, and cleanup might be required to free up resources.

</dd> <dt>

<span id="Exception"></span><span id="exception"></span><span id="EXCEPTION"></span>

<span id="Exception"></span><span id="exception"></span><span id="EXCEPTION"></span>**Exception** (10)


</dt> <dd>

The Job is in an abnormal state that might be indicative of an error condition. Actual status might be displayed though job-specific objects.

</dd> <dt>

<span id="Service"></span><span id="service"></span><span id="SERVICE"></span>

<span id="Service"></span><span id="service"></span><span id="SERVICE"></span>**Service** (11)


</dt> <dd>

The Job is in a vendor-specific state that supports problem discovery, or resolution, or both.

</dd> <dt>

<span id="Query_Pending"></span><span id="query_pending"></span><span id="QUERY_PENDING"></span>

<span id="Query_Pending"></span><span id="query_pending"></span><span id="QUERY_PENDING"></span>**Query Pending** (12)


</dt> <dd>

The Job is waiting for a client to resolve a query.

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

</dd> </dl>

</dd> <dt>

**JobStatus**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**ModelCorrespondence**](https://msdn.microsoft.com/library/aa393650) ("[**CIM\_ManagedSystemElement**](cim-managedsystemelement.md).**OperationalStatus**")
</dt> </dl>

A free-form string that represents the job status. This property is inherited from [**CIM\_Job**](https://msdn.microsoft.com/library/aa387873).

</dd> <dt>

**LocalOrUtcTime**
</dt> <dd> <dl> <dt>

Data type: **uint16**
</dt> <dt>

Access type: Read/write
</dt> </dl>

This property is inherited from [**CIM\_Job**](https://msdn.microsoft.com/library/aa387873).

The possible values are.

<dt>

<span id="Local_Time"></span><span id="local_time"></span><span id="LOCAL_TIME"></span>

<span id="Local_Time"></span><span id="local_time"></span><span id="LOCAL_TIME"></span>**Local Time** (1)


</dt> <dd>

Local time.

</dd> <dt>

<span id="UTC_Time"></span><span id="utc_time"></span><span id="UTC_TIME"></span>

<span id="UTC_Time"></span><span id="utc_time"></span><span id="UTC_TIME"></span>**UTC Time** (2)


</dt> <dd>

UTC time.

</dd> </dl>

</dd> <dt>

**Name**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**Required**](https://msdn.microsoft.com/library/aa393650)
</dt> </dl>

The user-friendly name for this instance of a job. In addition, the user-friendly name can be used as a property for a search or query. (Note: the **Name** property does not have to be unique within a namespace.) This property is inherited from [**CIM\_ConcreteJob**](https://msdn.microsoft.com/library/cc136808).

</dd> <dt>

**NetworkJobType**
</dt> <dd> <dl> <dt>

Data type: **uint16**
</dt> <dt>

Access type: Read-only
</dt> </dl>

The type of job.

<dt>

<span id="NvspWmiJobTypeInvalid"></span><span id="nvspwmijobtypeinvalid"></span><span id="NVSPWMIJOBTYPEINVALID"></span>

**NvspWmiJobTypeInvalid** (0)


</dt> <dd></dd> <dt>

<span id="NvspWmiJobTypeSetupSwitch"></span><span id="nvspwmijobtypesetupswitch"></span><span id="NVSPWMIJOBTYPESETUPSWITCH"></span>

**NvspWmiJobTypeSetupSwitch** (1)


</dt> <dd></dd> <dt>

<span id="NvspWmiJobTypeTeardownSwitch"></span><span id="nvspwmijobtypeteardownswitch"></span><span id="NVSPWMIJOBTYPETEARDOWNSWITCH"></span>

**NvspWmiJobTypeTeardownSwitch** (2)


</dt> <dd></dd> </dl>

</dd> <dt>

**Notify**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read/write
</dt> </dl>

The user that is notified upon job completion or failure. This property is inherited from [**CIM\_Job**](https://msdn.microsoft.com/library/aa387873).

</dd> <dt>

**OperationalStatus**
</dt> <dd> <dl> <dt>

Data type: **uint16** array
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**ArrayType**](https://msdn.microsoft.com/library/aa393650) ("Indexed"), [**ModelCorrespondence**](https://msdn.microsoft.com/library/aa393650) ("[**CIM\_ManagedSystemElement**](cim-managedsystemelement.md).**StatusDescriptions**")
</dt> </dl>

The current statuses of the object. This property is inherited from [**CIM\_ManagedSystemElement**](https://msdn.microsoft.com/library/aa387898) and each array element is always set to 2 (OK).

<dt>

<span id="OK"></span><span id="ok"></span>

<span id="OK"></span><span id="ok"></span>**OK** (2)


</dt> <dd>

Indicates full functionality without errors.

</dd> </dl>

</dd> <dt>

**OtherRecoveryAction**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**ModelCorrespondence**](https://msdn.microsoft.com/library/aa393650) ("[**CIM\_Job**](cim-job.md).**RecoveryAction**")
</dt> </dl>

This property is inherited from [**CIM\_Job**](https://msdn.microsoft.com/library/aa387873).

</dd> <dt>

**Owner**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**ModelCorrespondence**](https://msdn.microsoft.com/library/aa393650) ("CIM\_OwningJobElement")
</dt> </dl>

The user who submitted the job. This property is inherited from [**CIM\_Job**](https://msdn.microsoft.com/library/aa387873).

</dd> <dt>

**PercentComplete**
</dt> <dd> <dl> <dt>

Data type: **uint16**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**Units**](https://msdn.microsoft.com/library/aa393650) ("Percent"), [**MinValue**](https://msdn.microsoft.com/library/aa393650) (0), [**MaxValue**](https://msdn.microsoft.com/library/aa393650) (101)
</dt> </dl>

This property is inherited from [**CIM\_Job**](https://msdn.microsoft.com/library/aa387873).

</dd> <dt>

**Priority**
</dt> <dd> <dl> <dt>

Data type: **uint32**
</dt> <dt>

Access type: Read/write
</dt> </dl>

The importance of a job's execution. This property is inherited from [**CIM\_Job**](https://msdn.microsoft.com/library/aa387873).

</dd> <dt>

**RecoveryAction**
</dt> <dd> <dl> <dt>

Data type: **uint16**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**ModelCorrespondence**](https://msdn.microsoft.com/library/aa393650) ("[**CIM\_Job**](cim-job.md).**OtherRecoveryAction**")
</dt> </dl>

This property is inherited from [**CIM\_Job**](https://msdn.microsoft.com/library/aa387873).

The possible values are.

<dt>

<span id="Unknown"></span><span id="unknown"></span><span id="UNKNOWN"></span>

<span id="Unknown"></span><span id="unknown"></span><span id="UNKNOWN"></span>**Unknown** (0)


</dt> <dd>

Unknown.

</dd> <dt>

<span id="Other"></span><span id="other"></span><span id="OTHER"></span>

<span id="Other"></span><span id="other"></span><span id="OTHER"></span>**Other** (1)


</dt> <dd>

Take the action specified in the **OtherRecoveryAction** property.

</dd> <dt>

<span id="Do_Not_Continue"></span><span id="do_not_continue"></span><span id="DO_NOT_CONTINUE"></span>

<span id="Do_Not_Continue"></span><span id="do_not_continue"></span><span id="DO_NOT_CONTINUE"></span>**Do Not Continue** (2)


</dt> <dd>

Stop the job and update its status.

</dd> <dt>

<span id="Continue_With_Next_Job"></span><span id="continue_with_next_job"></span><span id="CONTINUE_WITH_NEXT_JOB"></span>

<span id="Continue_With_Next_Job"></span><span id="continue_with_next_job"></span><span id="CONTINUE_WITH_NEXT_JOB"></span>**Continue With Next Job** (3)


</dt> <dd>

Run the next job in the queue.

</dd> <dt>

<span id="Re-run_Job"></span><span id="re-run_job"></span><span id="RE-RUN_JOB"></span>

<span id="Re-run_Job"></span><span id="re-run_job"></span><span id="RE-RUN_JOB"></span>**Re-run Job** (4)


</dt> <dd>

Re-run job.

</dd> <dt>

<span id="Run_Recovery_Job"></span><span id="run_recovery_job"></span><span id="RUN_RECOVERY_JOB"></span>

<span id="Run_Recovery_Job"></span><span id="run_recovery_job"></span><span id="RUN_RECOVERY_JOB"></span>**Run Recovery Job** (5)


</dt> <dd>

Run the recovery job.

</dd> </dl>

</dd> <dt>

**RunDay**
</dt> <dd> <dl> <dt>

Data type: **sint8**
</dt> <dt>

Access type: Read/write
</dt> <dt>

Qualifiers: [**MinValue**](https://msdn.microsoft.com/library/aa393650) (-31), [**MaxValue**](https://msdn.microsoft.com/library/aa393650) (31), [**ModelCorrespondence**](https://msdn.microsoft.com/library/aa393650) ("[**CIM\_Job**](cim-job.md).**RunMonth**", "**CIM\_Job**.**RunDayOfWeek**", "**CIM\_Job**.**RunStartInterval**")
</dt> </dl>

This property is inherited from [**CIM\_Job**](https://msdn.microsoft.com/library/aa387873).

</dd> <dt>

**RunDayOfWeek**
</dt> <dd> <dl> <dt>

Data type: **sint8**
</dt> <dt>

Access type: Read/write
</dt> <dt>

Qualifiers: [**ModelCorrespondence**](https://msdn.microsoft.com/library/aa393650) ("[**CIM\_Job**](cim-job.md).**RunMonth**", "**CIM\_Job**.**RunDay**", "**CIM\_Job**.**RunStartInterval**")
</dt> </dl>

This property is inherited from [**CIM\_Job**](https://msdn.microsoft.com/library/aa387873).

The possible values are.

<dt>

<span id="-Saturday"></span><span id="-saturday"></span><span id="-SATURDAY"></span>

<span id="-Saturday"></span><span id="-saturday"></span><span id="-SATURDAY"></span>**-Saturday** (-7)


</dt> <dd>

The job is processed on the last Saturday on or before the day specified by **RunDay**.

</dd> <dt>

<span id="-Friday"></span><span id="-friday"></span><span id="-FRIDAY"></span>

<span id="-Friday"></span><span id="-friday"></span><span id="-FRIDAY"></span>**-Friday** (-6)


</dt> <dd>

The job is processed on the last Friday on or before the day specified by **RunDay**.

</dd> <dt>

<span id="-Thursday"></span><span id="-thursday"></span><span id="-THURSDAY"></span>

<span id="-Thursday"></span><span id="-thursday"></span><span id="-THURSDAY"></span>**-Thursday** (-5)


</dt> <dd>

The job is processed on the last Thursday on or before the day specified by **RunDay**.

</dd> <dt>

<span id="-Wednesday"></span><span id="-wednesday"></span><span id="-WEDNESDAY"></span>

<span id="-Wednesday"></span><span id="-wednesday"></span><span id="-WEDNESDAY"></span>**-Wednesday** (-4)


</dt> <dd>

The job is processed on the last Wednesday on or before the day specified by **RunDay**.

</dd> <dt>

<span id="-Tuesday"></span><span id="-tuesday"></span><span id="-TUESDAY"></span>

<span id="-Tuesday"></span><span id="-tuesday"></span><span id="-TUESDAY"></span>**-Tuesday** (-3)


</dt> <dd>

The job is processed on the last Tuesday on or before the day specified by **RunDay**.

</dd> <dt>

<span id="-Monday"></span><span id="-monday"></span><span id="-MONDAY"></span>

<span id="-Monday"></span><span id="-monday"></span><span id="-MONDAY"></span>**-Monday** (-2)


</dt> <dd>

The job is processed on the last Monday on or before the day specified by **RunDay**.

</dd> <dt>

<span id="-Sunday"></span><span id="-sunday"></span><span id="-SUNDAY"></span>

<span id="-Sunday"></span><span id="-sunday"></span><span id="-SUNDAY"></span>**-Sunday** (-1)


</dt> <dd>

The job is processed on the last Sunday on or before the day specified by **RunDay**.

</dd> <dt>

<span id="ExactDayOfMonth"></span><span id="exactdayofmonth"></span><span id="EXACTDAYOFMONTH"></span>

<span id="ExactDayOfMonth"></span><span id="exactdayofmonth"></span><span id="EXACTDAYOFMONTH"></span>**ExactDayOfMonth** (0)


</dt> <dd>

**RunDay** indicates the day of the month when the job is processed.

</dd> <dt>

<span id="Sunday"></span><span id="sunday"></span><span id="SUNDAY"></span>

<span id="Sunday"></span><span id="sunday"></span><span id="SUNDAY"></span>**Sunday** (1)


</dt> <dd>

The job is processed on the first Sunday on or after the day specified by **RunDay**.

</dd> <dt>

<span id="Monday"></span><span id="monday"></span><span id="MONDAY"></span>

<span id="Monday"></span><span id="monday"></span><span id="MONDAY"></span>**Monday** (2)


</dt> <dd>

The job is processed on the first Monday on or after the day specified by **RunDay**.

</dd> <dt>

<span id="Tuesday"></span><span id="tuesday"></span><span id="TUESDAY"></span>

<span id="Tuesday"></span><span id="tuesday"></span><span id="TUESDAY"></span>**Tuesday** (3)


</dt> <dd>

The job is processed on the first Tuesday on or after the day specified by **RunDay**.

</dd> <dt>

<span id="Wednesday"></span><span id="wednesday"></span><span id="WEDNESDAY"></span>

<span id="Wednesday"></span><span id="wednesday"></span><span id="WEDNESDAY"></span>**Wednesday** (4)


</dt> <dd>

The job is processed on the first Wednesday on or after the day specified by **RunDay**.

</dd> <dt>

<span id="Thursday"></span><span id="thursday"></span><span id="THURSDAY"></span>

<span id="Thursday"></span><span id="thursday"></span><span id="THURSDAY"></span>**Thursday** (5)


</dt> <dd>

The job is processed on the first Thursday on or after the day specified by **RunDay**.

</dd> <dt>

<span id="Friday"></span><span id="friday"></span><span id="FRIDAY"></span>

<span id="Friday"></span><span id="friday"></span><span id="FRIDAY"></span>**Friday** (6)


</dt> <dd>

The job is processed on the first Friday on or after the day specified by **RunDay**.

</dd> <dt>

<span id="Saturday"></span><span id="saturday"></span><span id="SATURDAY"></span>

<span id="Saturday"></span><span id="saturday"></span><span id="SATURDAY"></span>**Saturday** (7)


</dt> <dd>

The job is processed on the first Saturday on or after the day specified by **RunDay**.

</dd> </dl>

</dd> <dt>

**RunMonth**
</dt> <dd> <dl> <dt>

Data type: **uint8**
</dt> <dt>

Access type: Read/write
</dt> <dt>

Qualifiers: [**ModelCorrespondence**](https://msdn.microsoft.com/library/aa393650) ("[**CIM\_Job**](cim-job.md).**RunDay**", "**CIM\_Job**.**RunDayOfWeek**", "**CIM\_Job**.**RunStartInterval**")
</dt> </dl>

This property is inherited from [**CIM\_Job**](https://msdn.microsoft.com/library/aa387873).

The possible values are.

<dt>

<span id="January"></span><span id="january"></span><span id="JANUARY"></span>

**January** (0)


</dt> <dd></dd> <dt>

<span id="February"></span><span id="february"></span><span id="FEBRUARY"></span>

**February** (1)


</dt> <dd></dd> <dt>

<span id="March"></span><span id="march"></span><span id="MARCH"></span>

**March** (2)


</dt> <dd></dd> <dt>

<span id="April"></span><span id="april"></span><span id="APRIL"></span>

**April** (3)


</dt> <dd></dd> <dt>

<span id="May"></span><span id="may"></span><span id="MAY"></span>

**May** (4)


</dt> <dd></dd> <dt>

<span id="June"></span><span id="june"></span><span id="JUNE"></span>

**June** (5)


</dt> <dd></dd> <dt>

<span id="July"></span><span id="july"></span><span id="JULY"></span>

**July** (6)


</dt> <dd></dd> <dt>

<span id="August"></span><span id="august"></span><span id="AUGUST"></span>

**August** (7)


</dt> <dd></dd> <dt>

<span id="September"></span><span id="september"></span><span id="SEPTEMBER"></span>

**September** (8)


</dt> <dd></dd> <dt>

<span id="October"></span><span id="october"></span><span id="OCTOBER"></span>

**October** (9)


</dt> <dd></dd> <dt>

<span id="November"></span><span id="november"></span><span id="NOVEMBER"></span>

**November** (10)


</dt> <dd></dd> <dt>

<span id="December"></span><span id="december"></span><span id="DECEMBER"></span>

**December** (11)


</dt> <dd></dd> </dl>

</dd> <dt>

**RunStartInterval**
</dt> <dd> <dl> <dt>

Data type: **datetime**
</dt> <dt>

Access type: Read/write
</dt> <dt>

Qualifiers: [**SubType**](https://msdn.microsoft.com/library/aa393651) ("Interval"), [**ModelCorrespondence**](https://msdn.microsoft.com/library/aa393650) ("[**CIM\_Job**](cim-job.md).**RunMonth**", "**CIM\_Job**.**RunDay**", "**CIM\_Job**.**RunDayOfWeek**", "**CIM\_Job**.**RunStartInterval**")
</dt> </dl>

This property is inherited from [**CIM\_Job**](https://msdn.microsoft.com/library/aa387873).

</dd> <dt>

**ScheduledStartTime**
</dt> <dd> <dl> <dt>

Data type: **datetime**
</dt> <dt>

Access type: Read/write
</dt> <dt>

Qualifiers: [**Deprecated**](https://msdn.microsoft.com/library/aa393651) ("[**CIM\_Job**](cim-job.md).**RunMonth**", "**CIM\_Job**.**RunDay**", "**CIM\_Job**.**RunDayOfWeek**", "**CIM\_Job**.**RunStartInterval**")
</dt> </dl>

This property is inherited from [**CIM\_Job**](https://msdn.microsoft.com/library/aa387873).

</dd> <dt>

**StartTime**
</dt> <dd> <dl> <dt>

Data type: **datetime**
</dt> <dt>

Access type: Read-only
</dt> </dl>

The time that the job began. This property is inherited from [**CIM\_Job**](https://msdn.microsoft.com/library/aa387873).

</dd> <dt>

**Status**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**Deprecated**](https://msdn.microsoft.com/library/aa393651) ("[**CIM\_ManagedSystemElement**](cim-managedsystemelement.md).**OperationalStatus**"), [**MaxLen**](https://msdn.microsoft.com/library/aa393650) (10)
</dt> </dl>

This property is inherited from [**CIM\_ManagedSystemElement**](https://msdn.microsoft.com/library/aa387898) but it is not used.

</dd> <dt>

**StatusDescriptions**
</dt> <dd> <dl> <dt>

Data type: **string** array
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**ArrayType**](https://msdn.microsoft.com/library/aa393650) ("Indexed"), [**ModelCorrespondence**](https://msdn.microsoft.com/library/aa393650) ("[**CIM\_ManagedSystemElement**](cim-managedsystemelement.md).**OperationalStatus**")
</dt> </dl>

Strings that describe the various **OperationalStatus** property array values. This property is inherited from [**CIM\_ManagedSystemElement**](https://msdn.microsoft.com/library/aa387898) and each array element is always set to "OK".

</dd> <dt>

**TimeBeforeRemoval**
</dt> <dd> <dl> <dt>

Data type: **datetime**
</dt> <dt>

Access type: Read/write
</dt> <dt>

Qualifiers: [**Required**](https://msdn.microsoft.com/library/aa393650), [**SubType**](https://msdn.microsoft.com/library/aa393651) ("Interval")
</dt> </dl>

The amount of time that the job is retained after it has finished executing, either succeeding or failing in that execution. The job must remain in existence for some period of time regardless of the value of the **DeleteOnCompletion** property. The default is five minutes. This property is inherited from [**CIM\_ConcreteJob**](https://msdn.microsoft.com/library/cc136808) and is always set to "00000000000500.000000:000".

</dd> <dt>

**TimeOfLastStateChange**
</dt> <dd> <dl> <dt>

Data type: **datetime**
</dt> <dt>

Access type: Read-only
</dt> </dl>

The date or time when the state of the job last changed. If the state of the job has not changed and this property is populated, then it must be set to a 0 interval value. If a state change was requested, but rejected or not yet processed, the property must not be updated. This property is inherited from [**CIM\_ConcreteJob**](https://msdn.microsoft.com/library/cc136808).

</dd> <dt>

**TimeSubmitted**
</dt> <dd> <dl> <dt>

Data type: **datetime**
</dt> <dt>

Access type: Read-only
</dt> </dl>

The time that the job was submitted. This property is inherited from [**CIM\_Job**](https://msdn.microsoft.com/library/aa387873).

</dd> <dt>

**UntilTime**
</dt> <dd> <dl> <dt>

Data type: **datetime**
</dt> <dt>

Access type: Read/write
</dt> <dt>

Qualifiers: [**ModelCorrespondence**](https://msdn.microsoft.com/library/aa393650) ("[**CIM\_Job**](cim-job.md).**LocalOrUtcTime**")
</dt> </dl>

The time at which the job is invalid or should be stopped. This property is inherited from [**CIM\_Job**](https://msdn.microsoft.com/library/aa387873).

</dd> </dl>

## Remarks

Access to the **Msvm\_NetworkJob** class might be restricted by UAC Filtering. For more information, see [User Account Control and WMI](https://msdn.microsoft.com/library/aa826699).

## Requirements



|                                     |                                                                                                      |
|-------------------------------------|------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | None supported<br/>                                                                            |
| Minimum supported server<br/> | Windows Server 2008<br/>                                                                       |
| End of client support<br/>    | None supported<br/>                                                                            |
| End of server support<br/>    | Windows Server 2012 R2<br/>                                                                    |
| Namespace<br/>                | Root\\Virtualization<br/>                                                                      |
| MOF<br/>                      | <dl> <dt>WindowsVirtualization.mof</dt> </dl> |



## See also

<dl> <dt>

[**CIM\_ConcreteJob**](cim-concretejob.md)
</dt> <dt>

[**CIM\_ConcreteJob**](https://msdn.microsoft.com/library/cc136808)
</dt> <dt>

[Networking Classes](networking-classes.md)
</dt> </dl>

 

 




