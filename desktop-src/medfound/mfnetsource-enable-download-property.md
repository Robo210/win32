---
Description: Specifies whether all download protocols are enabled.
ms.assetid: c178693f-44ea-481e-b7f2-2ec94eea1994
title: MFNETSOURCE\_ENABLE\_DOWNLOAD property
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# MFNETSOURCE\_ENABLE\_DOWNLOAD property

Specifies whether all download protocols are enabled.



Data type

PROPVARIANT type (vt)

PROPVARIANT member

Boolean (**LONG**)

VT\_I4

**lVal**



## Remarks

The constant **MFNETSOURCE\_ENABLE\_DOWNLOAD** defines the GUID for this property key. The property identifier (PID) is zero.

Applications can use this property to configure the network source. To set the property, pass an **IPropertyStore** pointer to the [Configuring a Media Source](configuring-a-media-source.md).

## Requirements



|                                     |                                                                                    |
|-------------------------------------|------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista \[desktop apps only\]<br/>                                     |
| Minimum supported server<br/> | Windows Server 2008 \[desktop apps only\]<br/>                               |
| Header<br/>                   | <dl> <dt>Mfidl.h</dt> </dl> |



## See also

<dl> <dt>

[Media Foundation Properties](media-foundation-properties.md)
</dt> <dt>

[Networking in Media Foundation](networking-in-media-foundation.md)
</dt> <dt>

[Supported Protocols](supported-protocols.md)
</dt> </dl>

 

 



