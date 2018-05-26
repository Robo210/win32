---
title: Title Attribute (Stroke)(VML)
description: Title Attribute (Stroke)(VML)
ms.assetid: 47cdec4a-9b35-47d7-a44d-e128c6c8a812
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# Title Attribute (Stroke)(VML)

This topic describes VML, a feature that is deprecated as of Windows Internet Explorer 9. Webpages and applications that rely on VML should be [migrated to SVG](http://go.microsoft.com/fwlink/p/?LinkID=236964) or other widely supported standards.

> [!Note]  
> As of December 2011, this topic has been archived. As a result, it is no longer actively maintained. For more information, see [Archived Content](https://msdn.microsoft.com/library/hh772377). For information, recommendations, and guidance regarding the current version of Windows Internet Explorer, see [Internet Explorer Developer Center](http://go.microsoft.com/fwlink/p/?linkid=204313).

 

Defines the title of a stroke image. Read/write. **String**.

**Applies To**

[Stroke](msdn-online-vml-stroke-element.md)

**Tag Syntax**

&lt;v: *element* title=" *expression* "&gt;

**Script Syntax**

*element* .title="*expression*"

*expression*=*element*.title

**Remarks**

If this attribute has a value, then the stroke image is *embedded*. The actual value of the attribute is the text to be displayed with the picture when the mouse pointer moves over the image.

If the **HRef** tag is used, then **Title** is ignored.

This attribute is used by Microsoft Office but is not used by Microsoft Internet Explorer.

**Microsoft Office Extensions Attribute**

 

 



