---
title: Opacity Attribute (Shadow)(VML)
description: Opacity Attribute (Shadow)(VML)
ms.assetid: 394d755c-72cf-46f5-a258-1844b07a97bc
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# Opacity Attribute (Shadow)(VML)

This topic describes VML, a feature that is deprecated as of Windows Internet Explorer 9. Webpages and applications that rely on VML should be [migrated to SVG](http://go.microsoft.com/fwlink/p/?LinkID=236964) or other widely supported standards.

> [!Note]  
> As of December 2011, this topic has been archived. As a result, it is no longer actively maintained. For more information, see [Archived Content](https://msdn.microsoft.com/library/hh772377). For information, recommendations, and guidance regarding the current version of Windows Internet Explorer, see [Internet Explorer Developer Center](http://go.microsoft.com/fwlink/p/?linkid=204313).

 

Determines the transparency of a shadow. Read/write. [VgFraction](msdn-online-vml-vgfraction-data-type.md) .

**Applies To**

[Shadow](msdn-online-vml-shadow-element.md)

**Tag Syntax**

&lt;v: *element* opacity=" *expression* "&gt;

**Script Syntax**

*element* .opacity="*expression*"

*expression*=*element*.opacity

**Remarks**

The default value is 1. A value of 0 will make a completely transparent shadow.

*VML Standard Attribute*

**Example**

The shape has a shadow that is 50% transparent.


```HTML
   <v:shape id="rect01"
   coordorigin="0 0" coordsize="200 200"
   strokecolor= "red" fillcolor="red"
   style="top:20;left:20;width:30;height:30"
   path="m  1,1 l 1,200,200,200, 200,1 x e">
   <v:shadow on="True" opacity="50%"/>
   </v:shape>
```



 

 



