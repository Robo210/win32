---
Description: An ellipse is specified by its bounding rectangle. The following illustration shows an ellipse along with its bounding rectangle.
ms.assetid: 45e80501-4d64-480b-a7c7-3af52c00a0aa
title: Ellipses and Arcs
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# Ellipses and Arcs

An ellipse is specified by its bounding rectangle. The following illustration shows an ellipse along with its bounding rectangle.

![illustration of an ellipse enclosed within a bounding rectangle](images/aboutgdip02-art05.png)

To draw an ellipse, you need a [**Graphics**](/windows/win32/gdiplusgraphics/nl-gdiplusgraphics-graphics?branch=master) object and a [**Pen**](/windows/win32/gdipluspen/nl-gdipluspen-pen?branch=master) object. The **Graphics** object provides the [DrawEllipse](/windows/win32/gdiplusgraphics/nf-gdiplusgraphics-graphics-drawellipse(in const pen,in const rect &)?branch=master) method, and the **Pen** object stores attributes of the ellipse, such as line width and color. The address of the **Pen** object is passed as one of the arguments to the DrawEllipse method. The remaining arguments passed to the DrawEllipse method specify the bounding rectangle for the ellipse. The following example draws an ellipse; the bounding rectangle has a width of 160, a height of 80, and an upper-left corner of (100, 50).


```
myGraphics.DrawEllipse(&amp;myPen, 100, 50, 160, 80);
```



[DrawEllipse](/windows/win32/gdiplusgraphics/nf-gdiplusgraphics-graphics-drawellipse(in const pen,in const rect &)?branch=master) is an overloaded method of the [**Graphics**](/windows/win32/gdiplusgraphics/nl-gdiplusgraphics-graphics?branch=master) class, so there are several ways you can supply it with arguments. For example, you can construct a [**Rect**](/windows/win32/gdiplustypes/nl-gdiplustypes-rect?branch=master) object and pass a reference to the **Rect** object as an argument to the DrawEllipse method.


```
Rect myRect(100, 50, 160, 80);
myGraphics.DrawEllipse(&amp;myPen, myRect);
```



An arc is a portion of an ellipse. To draw an arc, you call the [DrawArc](/windows/win32/gdiplusgraphics/nf-gdiplusgraphics-graphics-drawarc(in const pen,in const rect &,in real,in real)?branch=master) method of the [**Graphics**](/windows/win32/gdiplusgraphics/nl-gdiplusgraphics-graphics?branch=master) class. The parameters of the DrawArc method are the same as the parameters of the [DrawEllipse](/windows/win32/gdiplusgraphics/nf-gdiplusgraphics-graphics-drawellipse(in const pen,in const rect &)?branch=master) method, except that DrawArc requires a starting angle and sweep angle. The following example draws an arc with a starting angle of 30 degrees and a sweep angle of 180 degrees.


```
myGraphics.DrawArc(&amp;myPen, 100, 50, 160, 80, 30, 180);
```



The following illustration shows the arc, the ellipse, and the bounding rectangle.

![illustration of an ellipse within a bounding rectangle; the lower left half of the ellipse is drawn in red](images/aboutgdip02-art06.png)

 

 


