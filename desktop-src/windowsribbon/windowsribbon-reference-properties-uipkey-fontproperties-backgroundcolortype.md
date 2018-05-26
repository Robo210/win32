---
title: UI\_PKEY\_FontProperties\_BackgroundColorType
description: Identifies the UI\_PKEY\_FontProperties\_BackgroundColorType property.
ms.assetid: d93f4d9f-3d35-4066-be94-f6b6b4302bff
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# UI\_PKEY\_FontProperties\_BackgroundColorType

Identifies the UI\_PKEY\_FontProperties\_BackgroundColorType property.

```
propertyDescription
   name = UI_PKEY_FontProperties_BackgroundColorType
   shellPKey = UI_PKEY_FontProperties_BackgroundColorType
   formatID = 00000311-7363-696e-8441798acf5aebb7
   propID = 311
   typeInfo
      type = UI_SWATCHCOLORTYPE
```

## Remarks

UI\_PKEY\_FontProperties\_BackgroundColorType is used by an application, in conjunction with [UI\_PKEY\_FontProperties\_BackgroundColor](https://msdn.microsoft.com/library/windows/desktop/dd371207), to query **Text highlight color** gallery settings.

The property value is from the [**UI\_SWATCHCOLORTYPE**](https://msdn.microsoft.com/library/windows/desktop/dd371583) enumeration.

The default value is `UI_SWATCHCOLORTYPE_RGB`.

The following table describes the property values.



|                                |                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
|--------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `UI_SWATCHCOLORTYPE_NOCOLOR`   | Application should query the appropriate system metric for the color value typically the current Windows theme **window background color** that is retrieved with GetSysColor(COLOR\_WINDOW).                                                                                                                                                                                                                                                                 |
| `UI_SWATCHCOLORTYPE_AUTOMATIC` | Not supported by the [**FontControl**](windowsribbon-element-fontcontrol.md).                                                                                                                                                                                                                                                                                                                                                                                |
| `UI_SWATCHCOLORTYPE_RGB`       | Application should query [UI\_PKEY\_FontProperties\_BackgroundColor](https://msdn.microsoft.com/library/windows/desktop/dd371207) for the color value. The color value of [UI\_PKEY\_FontProperties\_BackgroundColor](https://msdn.microsoft.com/library/windows/desktop/dd371207) is displayed on the **Text highlight color** button and selected in the **Text highlight color** gallery.<br/> |



 

UI\_PKEY\_FontProperties\_BackgroundColorType is passed to the [**IUICommandHandler::Execute**](https://msdn.microsoft.com/library/windows/desktop/dd371489) callback method when a color swatch is selected in a [**FontControl**](windowsribbon-element-fontcontrol.md) **Text highlight color** gallery.

> [!Note]  
> It is highly recommended that the application only set an initial **Text highlight color** value and not re-set this value when the cursor is repositioned within a document. The last selection should be maintained to avoid the need to re-select the desired color.

 

## Related topics

<dl> <dt>

[Font Control Properties](windowsribbon-reference-properties-fontcontrol.md)
</dt> <dt>

[**UI\_SWATCHCOLORTYPE**](https://msdn.microsoft.com/library/windows/desktop/dd371583)
</dt> <dt>

[Font Control](windowsribbon-controls-fontcontrol.md)
</dt> </dl>

 

 




