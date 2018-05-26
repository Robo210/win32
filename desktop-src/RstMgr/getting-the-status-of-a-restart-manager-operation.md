---
title: Getting the Status of a Restart Manager Operation
description: When many applications and services must be shut down or restarted, the Restart Manager operation can take an extended period of time. The following method can be used to obtain the status of the current operation.
ms.assetid: 0df9de1f-df37-46a5-8010-6c8b34429376
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# Getting the Status of a Restart Manager Operation

When many applications and services must be shut down or restarted, the Restart Manager operation can take an extended period of time. The following method can be used to obtain the status of the current operation.

**To get the status of the current Restart Manager operation**

1.  The installer should implement a [**RM\_WRITE\_STATUS\_CALLBACK**](/windows/win32/RestartManager/nc-restartmanager-rm_write_status_callback?branch=master) function that determines the status of the applications that have been shut down or restarted. The function can provide the information to the user interface or log.
2.  The installer passes the pointer to the [**RM\_WRITE\_STATUS\_CALLBACK**](/windows/win32/RestartManager/nc-restartmanager-rm_write_status_callback?branch=master) function when calling the [**RmShutdown**](/windows/win32/RestartManager/nf-restartmanager-rmshutdown?branch=master) or [**RmRestart**](/windows/win32/RestartManager/nf-restartmanager-rmrestart?branch=master) function.

 

 



