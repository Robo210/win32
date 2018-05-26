---
title: VML RotationAngle Attribute
description: VML RotationAngle Attribute
ms.assetid: d5432512-1ac2-497b-a415-cec3c1217120
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# VML RotationAngle Attribute

This topic describes VML, a feature that is deprecated as of Windows Internet Explorer 9. Webpages and applications that rely on VML should be [migrated to SVG](http://go.microsoft.com/fwlink/p/?LinkID=236964) or other widely supported standards.

> [!Note]  
> As of December 2011, this topic has been archived. As a result, it is no longer actively maintained. For more information, see [Archived Content](https://msdn.microsoft.com/library/hh772377). For information, recommendations, and guidance regarding the current version of Windows Internet Explorer, see [Internet Explorer Developer Center](http://go.microsoft.com/fwlink/p/?linkid=204313).

 

Specifies the rotation of the object about the x and y -axes. Read/write. **VgVector2D**.

**Applies To**

[Extrusion](msdn-online-vml-extrusion-element.md)

**Tag Syntax**

&lt;o: *element* rotationangle=" *expression* "&gt;

**Script Syntax**

*element* .rotationangle="*expression*"

*expression*=*element*.rotationangle

**Remarks**

The rotation of the object is defined by a rotation angle about the y-axis followed by the rotation angle about the x-axis.The z-axis angle is controlled by the value of the shape's standard HTML Style **Rotation** attribute. The default value is 0,0.

*Microsoft Office Extensions Attribute*

 

 



