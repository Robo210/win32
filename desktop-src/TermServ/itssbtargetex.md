---
title: ITsSbTargetEx interface
description: Exposes properties that store configuration and state information about a target.
audience: developer
author: REDMOND\\markl
manager: REDMOND\\markl
ms.assetid: 3f0f26fb-e8bc-47eb-8038-e51792ad4376
ms.prod: windows-server-dev
ms.technology: remote-desktop-services
ms.tgt_platform: multiple
keywords:
- ITsSbTargetEx interface Remote Desktop Services
- ITsSbTargetEx interface Remote Desktop Services , described
topic_type:
- apiref
api_name:
- ITsSbTargetEx
api_type:
- COM
ms.date: 05/31/2018
ms.topic: interface
ms.author: windowssdkdev
---

# ITsSbTargetEx interface

Exposes properties that store configuration and state information about a target.

This interface is only available on Windows Server 2012 R2 with [KB3091411](https://support.microsoft.com/kb/3091411) installed. The [**TargetLoad**](itssbtarget-targetload.md) property of the [**ITsSbTarget**](/windows/win32/sbtsv/nn-sbtsv-itssbtarget?branch=master) interface is available starting with Windows Server 2016.

## Members

The **ITsSbTargetEx** interface inherits from [**ITsSbTarget**](/windows/win32/sbtsv/nn-sbtsv-itssbtarget?branch=master). **ITsSbTargetEx** also has these types of members:

-   [Properties](#properties)

### Properties

The **ITsSbTargetEx** interface has these properties.



| Property                                                                      | Access type           | Description                                                                               |
|:------------------------------------------------------------------------------|:----------------------|:------------------------------------------------------------------------------------------|
| [**EnvironmentName**](/windows/win32/sbtsv/nf-sbtsv-itssbtarget-get_environmentname?branch=master)<br/>             | Read/write<br/> | Retrieves or specifies the name of the environment associated with the target.<br/> |
| [**FarmName**](itssbtarget-farmname.md)<br/>                           | Read/write<br/> | Specifies or retrieves the name of the farm to which this target is joined.<br/>    |
| [**IpAddresses**](itssbtarget-ipaddresses.md)<br/>                     | Read/write<br/> | Retrieves or specifies the external IP addresses of the target.<br/>                |
| [**NumPendingConnections**](/windows/win32/sbtsv/nf-sbtsv-itssbtarget-get_numpendingconnections?branch=master)<br/> | Read-only<br/>  | Retrieves the number of pending user connections for the target.<br/>               |
| [**NumSessions**](/windows/win32/sbtsv/nf-sbtsv-itssbtarget-get_numsessions?branch=master)<br/>                     | Read-only<br/>  | Retrieves the number of sessions maintained by broker for the target.<br/>          |
| [**TargetFQDN**](/windows/win32/sbtsv/nf-sbtsv-itssbtarget-get_targetfqdn?branch=master)<br/>                       | Read/write<br/> | Specifies or retrieves the fully qualified domain name of the target.<br/>          |
| [**TargetLoad**](/windows/win32/sbtsv/?branch=master)<br/>                     | Read-only<br/>  | Retrieves the relative load on a target.<br/>                                       |
| [**TargetName**](itssbtarget-targetname.md)<br/>                       | Read/write<br/> | Specifies or retrieves the name of the target.<br/>                                 |
| [**TargetNetbios**](/windows/win32/sbtsv/nf-sbtsv-itssbtarget-get_targetnetbios?branch=master)<br/>                 | Read/write<br/> | Specifies or retrieves the NetBIOS name of the target.<br/>                         |
| [**TargetPropertySet**](/windows/win32/sbtsv/nf-sbtsv-itssbtarget-get_targetpropertyset?branch=master)<br/>         | Read/write<br/> | Specifies or retrieves the property set for the target.<br/>                        |
| [**TargetState**](/windows/win32/sbtsv/nf-sbtsv-itssbtarget-get_targetstate?branch=master)<br/>                     | Read/write<br/> | Specifies or retrieves the target state.<br/>                                       |



 

## Requirements



|                                     |                                                                                  |
|-------------------------------------|----------------------------------------------------------------------------------|
| Minimum supported client<br/> | None supported<br/>                                                        |
| Minimum supported server<br/> | Windows Server 2012 R2<br/>                                                |
| End of server support<br/>    | Windows Server 2012 R2<br/>                                                |
| IID<br/>                      | IID\_ITsSbTargetEx is defined as 74f99987-625d-11e5-bea1-a0481c7e9064<br/> |



## See also

<dl> <dt>

[**ITsSbTarget**](/windows/win32/sbtsv/nn-sbtsv-itssbtarget?branch=master)
</dt> <dt>

[Remote Desktop Virtualization Interfaces](remote-desktop-virtualization-interfaces.md)
</dt> </dl>

 

 




