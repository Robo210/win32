---
Description: Raised by a media stream after a call to IMFMediaSourceStart causes a seek in the stream. A media stream raises this event when the media source raises the MESourceSeeked event.
ms.assetid: df06df16-711d-4262-b049-fb29f25934de
title: MEStreamSeeked event
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# MEStreamSeeked event

Raised by a media stream after a call to [**IMFMediaSource::Start**](/windows/win32/mfidl/nf-mfidl-imfmediasource-start?branch=master) causes a seek in the stream. A media stream raises this event when the media source raises the [MESourceSeeked](mesourceseeked.md) event.

## Event values

Possible values retrieved from [**IMFMediaEvent::GetValue**](/windows/win32/mfobjects/nf-mfobjects-imfmediaevent-getvalue?branch=master) include the following.



| VARTYPE           | Description                                                        |
|-------------------|--------------------------------------------------------------------|
| VT\_I8<br/> | New starting time, in 100-nanosecond units.<br/> <br/> |



## Requirements



|                                     |                                                                                                          |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista \[desktop apps only\]<br/>                                                           |
| Minimum supported server<br/> | Windows Server 2008 \[desktop apps only\]<br/>                                                     |
| Header<br/>                   | <dl> <dt>Mfobjects.h (include Mfidl.h)</dt> </dl> |



## See also

<dl> <dt>

[Media Foundation Events](media-foundation-events.md)
</dt> </dl>

 

 



