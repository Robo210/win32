---
title: ICM\_DRAW\_FLUSH message
description: The ICM\_DRAW\_FLUSH message notifies a rendering driver to render the contents of any image buffers that are waiting to be drawn. You can send this message explicitly or by using the ICDrawFlush macro.
ms.assetid: c29ed751-c773-4476-98fe-6edef3ff0cf4
keywords:
- ICM_DRAW_FLUSH message Windows Multimedia
topic_type:
- apiref
api_name:
- ICM_DRAW_FLUSH
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# ICM\_DRAW\_FLUSH message

The **ICM\_DRAW\_FLUSH** message notifies a rendering driver to render the contents of any image buffers that are waiting to be drawn. You can send this message explicitly or by using the [**ICDrawFlush**](/windows/win32/Vfw/nf-vfw-icdrawflush?branch=master) macro.


```C++
ICM_DRAW_FLUSH 
wParam = 0; 
lParam = 0; 
```



## Return Value

Returns ICERR\_OK if successful or an error otherwise.

## Remarks

This message is used only by hardware that performs its own asynchronous decompression, timing, and drawing.

## Requirements



|                                     |                                                                                  |
|-------------------------------------|----------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 2000 Professional \[desktop apps only\]<br/>                       |
| Minimum supported server<br/> | Windows 2000 Server \[desktop apps only\]<br/>                             |
| Header<br/>                   | <dl> <dt>Vfw.h</dt> </dl> |



## See also

<dl> <dt>

[Video Compression Manager](video-compression-manager.md)
</dt> <dt>

[Video Compression Messages](video-compression-messages.md)
</dt> </dl>

 

 




