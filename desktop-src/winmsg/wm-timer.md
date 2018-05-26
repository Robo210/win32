---
Description: Posted to the installing threads message queue when a timer expires. The message is posted by the GetMessage or PeekMessage function.
ms.assetid: 419e3f05-35ec-4e48-b24d-ab98df687b20
title: WM\_TIMER message
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# WM\_TIMER message

Posted to the installing thread's message queue when a timer expires. The message is posted by the [**GetMessage**](/windows/win32/Winuser/nf-engextcpp-extexception-getmessage?branch=master) or [**PeekMessage**](/windows/win32/Winuser/nf-winuser-peekmessagea?branch=master) function.


```C++
#define WM_TIMER                        0x0113
```



## Parameters

<dl> <dt>

*wParam* \[in\]
</dt> <dd>

The timer identifier.

</dd> <dt>

*lParam* \[in\]
</dt> <dd>

A pointer to an application-defined callback function that was passed to the [**SetTimer**](/windows/win32/Winuser/nf-ndis-ndismsettimer?branch=master) function when the timer was installed.

</dd> </dl>

## Return value

Type: **LRESULT**

An application should return zero if it processes this message.

## Remarks

You can process the message by providing a **WM\_TIMER** case in the window procedure. Otherwise, [**DispatchMessage**](/windows/win32/Winuser/nf-winuser-dispatchmessage?branch=master) will call the [*TimerProc*](/windows/win32/Winuser/nc-winuser-timerproc?branch=master) callback function specified in the call to the [**SetTimer**](/windows/win32/Winuser/nf-ndis-ndismsettimer?branch=master) function used to install the timer.

The **WM\_TIMER** message is a low-priority message. The [**GetMessage**](/windows/win32/Winuser/nf-engextcpp-extexception-getmessage?branch=master) and [**PeekMessage**](/windows/win32/Winuser/nf-winuser-peekmessagea?branch=master) functions post this message only when no other higher-priority messages are in the thread's message queue.

## Requirements



|                                     |                                                                                                          |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 2000 Professional \[desktop apps only\]<br/>                                               |
| Minimum supported server<br/> | Windows 2000 Server \[desktop apps only\]<br/>                                                     |
| Header<br/>                   | <dl> <dt>Winuser.h (include Windows.h)</dt> </dl> |



## See also

<dl> <dt>

**Reference**
</dt> <dt>

[**GetMessage**](/windows/win32/Winuser/nf-engextcpp-extexception-getmessage?branch=master)
</dt> <dt>

[**PeekMessage**](/windows/win32/Winuser/nf-winuser-peekmessagea?branch=master)
</dt> <dt>

[**SetTimer**](/windows/win32/Winuser/nf-ndis-ndismsettimer?branch=master)
</dt> <dt>

[**TimerProc**](/windows/win32/Winuser/nc-winuser-timerproc?branch=master)
</dt> <dt>

**Conceptual**
</dt> <dt>

[Timers](timers.md)
</dt> </dl>

 

 



