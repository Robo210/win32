---
title: Mouse Input Functions
description: .
ms.assetid: a666b25b-a75c-4500-8077-fabe07589a1d
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# Mouse Input Functions

## 

## In this section



<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th>Topic</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>[<strong>_TrackMouseEvent</strong>](/windows/win32/CommCtrl/nf-commctrl-_trackmouseevent?branch=master)<br/></td>
<td>Posts messages when the mouse pointer leaves a window or hovers over a window for a specified amount of time. This function calls [<strong>TrackMouseEvent</strong>](/windows/win32/Winuser/nf-winuser-trackmouseevent?branch=master) if it exists, otherwise it emulates it.<br/></td>
</tr>
<tr class="even">
<td>[<strong>DragDetect</strong>](/windows/win32/Winuser/nf-winuser-dragdetect?branch=master)<br/></td>
<td>Captures the mouse and tracks its movement until the user releases the left button, presses the ESC key, or moves the mouse outside the drag rectangle around the specified point. The width and height of the drag rectangle are specified by the <strong>SM_CXDRAG</strong> and <strong>SM_CYDRAG</strong> values returned by the [<strong>GetSystemMetrics</strong>](https://msdn.microsoft.com/library/windows/desktop/ms724385) function.<br/></td>
</tr>
<tr class="odd">
<td>[<strong>GetCapture</strong>](/windows/win32/Winuser/nf-winuser-getcapture?branch=master)<br/></td>
<td>Retrieves a handle to the window (if any) that has captured the mouse. Only one window at a time can capture the mouse; this window receives mouse input whether or not the cursor is within its borders. <br/></td>
</tr>
<tr class="even">
<td>[<strong>GetDoubleClickTime</strong>](/windows/win32/Winuser/nf-winuser-getdoubleclicktime?branch=master)<br/></td>
<td>Retrieves the current double-click time for the mouse. A double-click is a series of two clicks of the mouse button, the second occurring within a specified time after the first. The double-click time is the maximum number of milliseconds that may occur between the first and second click of a double-click. The maximum double-click time is 5000 milliseconds.<br/></td>
</tr>
<tr class="odd">
<td>[<strong>GetMouseMovePointsEx</strong>](/windows/win32/Winuser/nf-winuser-getmousemovepointsex?branch=master)<br/></td>
<td>Retrieves a history of up to 64 previous coordinates of the mouse or pen.<br/></td>
</tr>
<tr class="even">
<td>[<strong>mouse_event</strong>](/windows/win32/Winuser/nf-winuser-mouse_event?branch=master)<br/></td>
<td>The [<strong>mouse_event</strong>](/windows/win32/Winuser/nf-winuser-mouse_event?branch=master) function synthesizes mouse motion and button clicks.<br/>
<blockquote>
[!Note]<br />
This function has been superseded. Use [<strong>SendInput</strong>](/windows/win32/Winuser/nf-winuser-sendinput?branch=master) instead.
</blockquote>
<br/></td>
</tr>
<tr class="odd">
<td>[<strong>ReleaseCapture</strong>](/windows/win32/Winuser/nf-winuser-releasecapture?branch=master)<br/></td>
<td>Releases the mouse capture from a window in the current thread and restores normal mouse input processing. A window that has captured the mouse receives all mouse input, regardless of the position of the cursor, except when a mouse button is clicked while the cursor hot spot is in the window of another thread. <br/></td>
</tr>
<tr class="even">
<td>[<strong>SetCapture</strong>](/windows/win32/Winuser/nf-winuser-setcapture?branch=master)<br/></td>
<td>Sets the mouse capture to the specified window belonging to the current thread.<br/></td>
</tr>
<tr class="odd">
<td>[<strong>SetDoubleClickTime</strong>](/windows/win32/Winuser/nf-winuser-setdoubleclicktime?branch=master)<br/></td>
<td>Sets the double-click time for the mouse. A double-click is a series of two clicks of a mouse button, the second occurring within a specified time after the first. The double-click time is the maximum number of milliseconds that may occur between the first and second clicks of a double-click. <br/></td>
</tr>
<tr class="even">
<td>[<strong>SwapMouseButton</strong>](/windows/win32/Winuser/nf-winuser-swapmousebutton?branch=master)<br/></td>
<td>Reverses or restores the meaning of the left and right mouse buttons. <br/></td>
</tr>
<tr class="odd">
<td>[<strong>TrackMouseEvent</strong>](/windows/win32/Winuser/nf-winuser-trackmouseevent?branch=master)<br/></td>
<td>Posts messages when the mouse pointer leaves a window or hovers over a window for a specified amount of time.<br/>
<blockquote>
[!Note]<br />
The [<strong>_TrackMouseEvent</strong>](/windows/win32/CommCtrl/nf-commctrl-_trackmouseevent?branch=master) function calls [<strong>TrackMouseEvent</strong>](/windows/win32/Winuser/nf-winuser-trackmouseevent?branch=master) if it exists, otherwise <strong>_TrackMouseEvent</strong> emulates <strong>TrackMouseEvent</strong>.
</blockquote>
<br/></td>
</tr>
</tbody>
</table>



 

 

 




