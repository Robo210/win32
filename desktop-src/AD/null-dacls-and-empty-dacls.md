---
title: Null DACLs and Empty DACLs
description: The presence of a null discretionary access-control list (DACL) in the nTSecurityDescriptor attribute of any object can create a serious security risk.
audience: developer
author: REDMOND\\markl
manager: REDMOND\\mbaldwin
ms.assetid: 32b786d2-e676-4402-ad22-550de9289494
ms.prod: windows-server-dev
ms.technology: active-directory-domain-services
ms.tgt_platform: multiple
keywords:
- Null DACLs and Empty DACLs AD
- DACLs AD , Null and Empty
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
---

# Null DACLs and Empty DACLs

The presence of a null discretionary access-control list (DACL) in the [**nTSecurityDescriptor**](https://msdn.microsoft.com/library/ms679006) attribute of any object can create a serious security risk. A null DACL grants full access to any user that requests it; normal security checking is not performed with respect to the object. A null DACL should not be confused with an empty DACL. An empty DACL is a properly allocated and initialized DACL containing no access-control entries (ACEs). An empty DACL grants no access to the object it is assigned to.

For more information, see [Null DACLs and Empty DACLs](https://msdn.microsoft.com/library/windows/desktop/aa379286).

 

 



