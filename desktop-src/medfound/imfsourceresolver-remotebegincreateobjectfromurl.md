---
Description: Remotable version of the IMFSourceResolverBeginCreateObjectFromURL method.
ms.assetid: 3c0b0aaf-832b-4708-bed9-6f448770ee77
title: RemoteBeginCreateObjectFromURL
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# RemoteBeginCreateObjectFromURL

Remotable version of the [**IMFSourceResolver::BeginCreateObjectFromURL**](/windows/win32/mfidl/nf-mfidl-imfsourceresolver-begincreateobjectfromurl?branch=master) method.

``` syntax
[call_as(BeginCreateObjectFromURL)]
HRESULT RemoteBeginCreateObjectFromURL(
    LPCWSTR pwszURL,
    DWORD dwFlags,
    IPropertyStore *pProps,
    IMFRemoteAsyncCallback *pCallback
);
```

## Remarks

Applications cannot call this method directly, and objects do not implement this method. The method does not appear in the vtable for the interface. If [**BeginCreateObjectFromURL**](/windows/win32/mfidl/nf-mfidl-imfsourceresolver-begincreateobjectfromurl?branch=master) is called across process boundaries, the Media Foundation proxy/stub DLL translates the call into a call to the remote method and then translates it back.

## Requirements



|                                     |                                                                                                          |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista \[desktop apps \| UWP apps\]<br/>                                                    |
| Minimum supported server<br/> | Windows Server 2008 \[desktop apps \| UWP apps\]<br/>                                              |
| Header<br/>                   | <dl> <dt>Mfobjects.h (include Mfidl.h)</dt> </dl> |
| Library<br/>                  | <dl> <dt>Mfuuid.lib</dt> </dl>                    |



## See also

<dl> <dt>

[**IMFSourceResolver**](/windows/win32/mfidl/nn-mfidl-imfsourceresolver?branch=master)
</dt> </dl>

 

 



