---
Description: The fax service provider (FSP) function prototypes use the LPWSTR data type for string parameters. FSP DLLs must be compiled for Unicode. If the FSP is not compiled for Unicode, the function calls fail because the FSP DLL receives only Unicode strings.
ms.assetid: e3703165-8f14-4d11-aa88-fcbeb0a4989e
title: Converting String Parameters
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# Converting String Parameters

The fax service provider (FSP) function prototypes use the **LPWSTR** data type for string parameters. FSP DLLs must be compiled for Unicode. If the FSP is not compiled for Unicode, the function calls fail because the FSP DLL receives only Unicode strings.

 

 


