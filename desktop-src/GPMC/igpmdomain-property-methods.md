---
title: IGPMDomain Property Methods
description: The property methods of the IGPMDomain interface get the properties that are described in the following table. For a general discussion of property methods, see Interface Property Methods in the Active Directory Service Interfaces (ADSI) documentation.
audience: developer
author: REDMOND\\markl
manager: REDMOND\\markl
ms.assetid: 7d252302-6250-4c84-ad21-4b2bbe229da8
ms.prod: windows-server-dev
ms.technology: group-policy
ms.tgt_platform: multiple
keywords:
- IGPMDomain Property Methods GPMC
topic_type:
- apiref
api_name:
- IGPMDomain Property Methods
- IGPMDomain.Domain
- IGPMDomain.get_Domain
- IGPMDomain.DomainController
- IGPMDomain.get_DomainController
api_location:
- Gpmgmt.dll
api_type:
- COM
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
---

# IGPMDomain Property Methods

The property methods of the [**IGPMDomain**](/windows/previous-versions/Gpmgmt/nn-gpmgmt-igpmdomain?branch=master) interface get the properties that are described in the following table. For a general discussion of property methods, see [Interface Property Methods](https://msdn.microsoft.com/library/aa746378) in the Active Directory Service Interfaces (ADSI) documentation.

## Properties

<dl> <dt>

**Domain**
</dt> <dd> <dl>

Full Domain Name System (DNS) name of the domain, such as example.microsoft.com.

<dt>

Access type: Read-only
</dt> <dt>

Scripting data type: **String**
</dt> <dt>



``` syntax
// C++ method syntax
HRESULT get_Domain(
  [out] BSTR* pVal
);
```


</dt> </dl> </dd> <dt>

**DomainController**
</dt> <dd> <dl>

The domain controller name for the domain. This is the domain controller with which the Group Policy Management Console (GPMC) is communicating. The domain controller is specified by the user in a call to the [**IGPM::GetDomain**](/windows/previous-versions/Gpmgmt/nf-gpmgmt-igpm-getdomain?branch=master) method. The domain controller name is not always a DNS name. Sometimes, the domain controller name is returned in NetBIOS format.

<dt>

Access type: Read-only
</dt> <dt>

Scripting data type: **String**
</dt> <dt>



``` syntax
// C++ method syntax
HRESULT get_DomainController(
  [out] BSTR* pVal
);
```


</dt> </dl> </dd> </dl>

 

## Requirements



|                                     |                                                                                       |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista<br/>                                                              |
| Minimum supported server<br/> | Windows Server 2008<br/>                                                        |
| Header<br/>                   | <dl> <dt>Gpmgmt.h</dt> </dl>   |
| IDL<br/>                      | <dl> <dt>Gpmgmt.idl</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Gpmgmt.dll</dt> </dl> |
| IID<br/>                      | IID\_IGPMDomain is defined as 6B21CC14-5A00-4F44-A738-FEEC8A94C7E3<br/>         |



## See also

<dl> <dt>

[**IGPMDomain**](/windows/previous-versions/Gpmgmt/nn-gpmgmt-igpmdomain?branch=master)
</dt> <dt>

[**IGPMSitesContainer**](/windows/previous-versions/Gpmgmt/nn-gpmgmt-igpmsitescontainer?branch=master)
</dt> <dt>

[**IGPM**](/windows/previous-versions/Gpmgmt/nn-gpmgmt-igpm?branch=master)
</dt> </dl>

 

 




