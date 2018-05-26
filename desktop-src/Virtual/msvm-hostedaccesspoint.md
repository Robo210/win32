---
title: Msvm\_HostedAccessPoint class
description: An association that connects a virtual switch service to a switch port inside of the Microsoft Hyper-V platform.
ms.assetid: 8f1def3f-ac54-4bca-ae5e-811b685a44bc
keywords:
- Msvm_HostedAccessPoint class Hyper-V
- Msvm_HostedAccessPoint class Hyper-V , described
topic_type:
- apiref
api_name:
- Msvm_HostedAccessPoint
- Msvm_HostedAccessPoint.Antecedent
- Msvm_HostedAccessPoint.Dependent
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

# Msvm\_HostedAccessPoint class

An association that connects a virtual switch service to a switch port inside of the Microsoft Hyper-V platform.

The following syntax is simplified Managed Object Format (MOF) code, and it includes all of the inherited properties.

## Syntax

``` syntax
[Association, Dynamic, Provider("VmmsWmiInstanceAndMethodProvider"), AMENDMENT]
class Msvm_HostedAccessPoint : CIM_HostedAccessPoint
{
  Msvm_VirtualSwitch REF Antecedent;
  Msvm_SwitchPort    REF Dependent;
};
```

## Members

The **Msvm\_HostedAccessPoint** class has these types of members:

-   [Properties](#properties)

### Properties

The **Msvm\_HostedAccessPoint** class has these properties.

<dl> <dt>

**Antecedent**
</dt> <dd> <dl> <dt>

Data type: **[**Msvm\_VirtualSwitch**](msvm-virtualswitch.md)**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**Override**](https://msdn.microsoft.com/library/aa393650) ("Antecedent"), [**Min**](https://msdn.microsoft.com/library/aa393650) (1), [**Max**](https://msdn.microsoft.com/library/aa393650) (1)
</dt> </dl>

A reference to the virtual switch.

</dd> <dt>

**Dependent**
</dt> <dd> <dl> <dt>

Data type: **[**Msvm\_SwitchPort**](msvm-switchport.md)**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**Override**](https://msdn.microsoft.com/library/aa393650) ("Dependent"), [**Weak**](https://msdn.microsoft.com/library/aa393650)
</dt> </dl>

A reference to the switch port hosted by the virtual switch.

</dd> </dl>

## Remarks

Access to the **Msvm\_HostedAccessPoint** class might be restricted by UAC Filtering. For more information, see [User Account Control and WMI](https://msdn.microsoft.com/library/aa826699).

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

[**CIM\_HostedAccessPoint**](cim-hostedaccesspoint.md)
</dt> <dt>

[**CIM\_HostedAccessPoint**](https://msdn.microsoft.com/library/aa387858)
</dt> <dt>

[Networking Classes](networking-classes.md)
</dt> </dl>

 

 




