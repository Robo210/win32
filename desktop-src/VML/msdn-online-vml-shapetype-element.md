---
title: VML ShapeType Element
description: VML ShapeType Element
ms.assetid: 4e0288c9-ab0f-4399-982a-97dcf16f4ec4
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# VML ShapeType Element

This topic describes VML, a feature that is deprecated as of Windows Internet Explorer 9. Webpages and applications that rely on VML should be [migrated to SVG](http://go.microsoft.com/fwlink/p/?LinkID=236964) or other widely supported standards.

> [!Note]  
> As of December 2011, this topic has been archived. As a result, it is no longer actively maintained. For more information, see [Archived Content](https://msdn.microsoft.com/library/hh772377). For information, recommendations, and guidance regarding the current version of Windows Internet Explorer, see [Internet Explorer Developer Center](http://go.microsoft.com/fwlink/p/?linkid=204313).

 

Defines a shape that can be used to create other shapes.

The following attribute modifies a **ShapeType**.



| Attribute                                      | Description                                             |
|------------------------------------------------|---------------------------------------------------------|
| [Master](msdn-online-vml-master-attribute.md) | Determines whether a **ShapeType** is a master element. |



 

**Remarks**

**ShapeType** is identical to the **Shape** element except it cannot reference another **ShapeType** element.

When a **Shape** element makes reference to a **ShapeType**, the **Shape** may duplicate some of the properties that have already been specified in the **ShapeType**. In these cases, the attributes in the **Shape** override those of the **ShapeType**.

The **Type** attribute may not be used with **ShapeType**.

CSS positioning attributes (such as **Top**, **Left**, etc.) are not passed to a **Shape** from a **ShapeType**.

To use this element, create a **ShapeType** with a specific [ID](id-attribute--vml.md) attribute. Then create a **Shape** and reference the **ShapeType** with the **Type** attribute. See the [Type](type-attribute--shape--vml.md) attribute for more information.

 

 



