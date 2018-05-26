---
title: WM\_DWMSENDICONICTHUMBNAIL message
description: Instructs a window to provide a static bitmap to use as a thumbnail representation of that window.
ms.assetid: 476c2542-f4d0-4777-93d3-bf50da26d94f
keywords:
- WM_DWMSENDICONICTHUMBNAIL message Desktop Window Manager
topic_type:
- apiref
api_name:
- WM_DWMSENDICONICTHUMBNAIL
api_location:
- Dwmapi.h
api_type:
- HeaderDef
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# WM\_DWMSENDICONICTHUMBNAIL message

Instructs a window to provide a static bitmap to use as a thumbnail representation of that window.

## Parameters

<dl> <dt>

*wParam* 
</dt> <dd>

Not used.

</dd> <dt>

*lParam* 
</dt> <dd>

The [**HIWORD**](https://msdn.microsoft.com/library/windows/desktop/ms632657) of this value is the maximum x-coordinate of the thumbnail. The [**LOWORD**](https://msdn.microsoft.com/library/windows/desktop/ms632659) is the maximum y-coordinate. If a thumbnail has a dimension that exceeds one or both of these values, the DWM does not accept the thumbnail.

</dd> </dl>

## Return value

If an application processes this message, it should return zero.

## Remarks

DWM sends this message to a window if all of the following situations are true:

-   DWM is displaying an iconic representation of the window.
-   The [**DWMWA\_HAS\_ICONIC\_BITMAP**](/windows/win32/Dwmapi/ne-dwmapi-dwmwindowattribute?branch=master) attribute is set on the window.
-   The window did not set a cached bitmap.
-   There is room in the cache for another bitmap.

The window that receives this message should respond by generating a bitmap that is not larger than the size that is requested in the message parameters. The window then calls the [**DwmSetIconicThumbnail**](/windows/win32/Dwmapi/nf-dwmapi-dwmseticonicthumbnail?branch=master) function to override the default thumbnail. If the window does not supply a bitmap in a given amount of time, DWM uses its own default iconic representation for the window.

The window must belong to the calling process.

## Examples

The following code example shows how to respond to the **WM\_DWMSENDICONICTHUMBNAIL** message. The example calls [**DwmSetIconicThumbnail**](/windows/win32/Dwmapi/nf-dwmapi-dwmseticonicthumbnail?branch=master), with a handle to a customized, device-indepedent bitmap to use as the windows' representation.


```C++
        case WM_DWMSENDICONICTHUMBNAIL:
        {    
            // This window is being asked to provide its iconic bitmap. This indicates
            // a thumbnail is being drawn.
            hbm = CreateDIB(HIWORD(lParam), LOWORD(lParam)); 
            if (hbm)
            {
                hr = DwmSetIconicThumbnail(hwnd, hbm, 0);
                DeleteObject(hbm);
            }
        }
        break;
```



For the complete example, see the [Customize an Iconic Thumbnail and a Live Preview Bitmap](dwm-sample-customizethumbnail.md) sample.

## Requirements



|                                     |                                                                                     |
|-------------------------------------|-------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 7 \[desktop apps only\]<br/>                                          |
| Minimum supported server<br/> | Windows Server 2008 R2 \[desktop apps only\]<br/>                             |
| Header<br/>                   | <dl> <dt>Dwmapi.h</dt> </dl> |



## See also

<dl> <dt>

[**DwmInvalidateIconicBitmaps**](/windows/win32/Dwmapi/nf-dwmapi-dwminvalidateiconicbitmaps?branch=master)
</dt> <dt>

[**WM\_DWMSENDICONICLIVEPREVIEWBITMAP**](wm-dwmsendiconiclivepreviewbitmap.md)
</dt> </dl>

 

 




