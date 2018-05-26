---
title: Property Structure Construction Functions
description: The property structure construction functions are used by applications and resource DLLs to build property lists, parameter blocks, and property tables.
audience: developer
author: REDMOND\\markl
manager: REDMOND\\markl
ms.assetid: f2a4be50-be24-4eac-9651-ea1b6fc97fe8
ms.prod: windows-server-dev
ms.technology: failover-clustering
ms.tgt_platform: multiple
keywords:
- property structure construction functions Failover Cluster
- cluster utility functions Failover Cluster ,property structure construction functions
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
---

# Property Structure Construction Functions

The property structure construction functions are used by applications and [resource DLLs](resource-dlls.md) to build [property lists](property-lists.md), [parameter blocks](parameter-blocks.md), and [property tables](property-tables.md).

## In this section

<dl> <dt>

[*ResUtilDupParameterBlock*](/windows/previous-versions/ResApi/nc-resapi-presutil_dup_parameter_block?branch=master)
</dt> <dd>

Performs a member-wise copy of the data from one [parameter block](parameter-blocks.md) to another.

</dd> <dt>

[*ResUtilFreeParameterBlock*](/windows/previous-versions/ResApi/nc-resapi-presutil_free_parameter_block?branch=master)
</dt> <dd>

Deallocates memory that has been allocated for a [parameter block](parameter-blocks.md) by [*ResUtilDupParameterBlock*](/windows/previous-versions/ResApi/nc-resapi-presutil_dup_parameter_block?branch=master).

</dd> <dt>

[*ResUtilPropertyListFromParameterBlock*](/windows/previous-versions/ResApi/nc-resapi-presutil_property_list_from_parameter_block?branch=master)
</dt> <dd>

Constructs a [property list](property-lists.md) from a [property table](property-tables.md) and a [parameter block](parameter-blocks.md).

</dd> <dt>

[*ResUtilVerifyPrivatePropertyList*](/windows/previous-versions/ResApi/nc-resapi-presutil_verify_private_property_list?branch=master)
</dt> <dd>

Verifies that a [property list](property-lists.md) is correctly formatted.

</dd> <dt>

[*ResUtilVerifyPropertyTable*](/windows/previous-versions/ResApi/nc-resapi-presutil_verify_property_table?branch=master)
</dt> <dd>

Uses a [property table](property-tables.md) to verify that a [property list](property-lists.md) is correctly formatted.

</dd> </dl>

## Related topics

<dl> <dt>

[Failover Cluster Utility Functions](cluster-utility-functions.md)
</dt> </dl>

 

 



