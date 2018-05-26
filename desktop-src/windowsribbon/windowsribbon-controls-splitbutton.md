---
title: Split Button
description: The Split Button is a composite control with which the user can select a default value bound to a primary button, or select from a list of mutually exclusive values displayed in a drop-down list bound to a secondary button.
ms.assetid: 0939b3be-fa88-4864-8096-a664ab2e97b5
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# Split Button

The Split Button is a composite control with which the user can select a default value bound to a primary button, or select from a list of mutually exclusive values displayed in a drop-down list bound to a secondary button.

-   [Introduction](#introduction)
-   [Split Button Properties](#split-button-properties)
-   [Related topics](#related-topics)

## Introduction

This control is useful for exposing closely related items in cases where an obvious default is available and where the individual items can be represented by an image, text, or both.

The following screen shot illustrates the Ribbon Split Button.

![screen shot of a splitbutton control in a sample ribbon.](images/controls/splitbutton.png)

## Split Button Properties

The Ribbon framework defines a collection of [property keys](windowsribbon-reference-properties.md) for the Split Button control.

Typically, a Split Button property is updated in the ribbon UI by invalidating the Command associated with the control through a call to the [**IUIFramework::InvalidateUICommand**](https://msdn.microsoft.com/library/windows/desktop/dd371375) method. The invalidation event is handled, and the property updates defined, by the [**IUICommandHandler::UpdateProperty**](https://msdn.microsoft.com/library/windows/desktop/dd371494) callback method.

The [**IUICommandHandler::UpdateProperty**](https://msdn.microsoft.com/library/windows/desktop/dd371494) callback method is not executed, and the application queried for an updated property value, until the property is required by the framework. For example, when a tab is activated and a control revealed in the ribbon UI, or when a tooltip is displayed.

> [!Note]  
> In some cases, a property can be retrieved through the [**IUIFramework::GetUICommandProperty**](https://msdn.microsoft.com/library/windows/desktop/dd371370) method and set with the [**IUIFramework::SetUICommandProperty**](https://msdn.microsoft.com/library/windows/desktop/dd371478) method.

 

The following table lists the property keys that are associated with the Split Button control.



<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th>Property Key</th>
<th>Notes</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>[UI_PKEY_Enabled](windowsribbon-reference-properties-uipkey-enabled.md)</td>
<td>Supports [<strong>IUIFramework::GetUICommandProperty</strong>](https://msdn.microsoft.com/library/windows/desktop/dd371370) and [<strong>IUIFramework::SetUICommandProperty</strong>](https://msdn.microsoft.com/library/windows/desktop/dd371478).<br/> If all child items are disabled, the framework sets [UI_PKEY_Enabled](windowsribbon-reference-properties-uipkey-enabled.md) to false (0). Otherwise, if one or more child items are enabled, UI_PKEY_Enabled is set to true (-1).
<blockquote>
[!Important]<br />
The [UI_PKEY_Enabled](windowsribbon-reference-properties-uipkey-enabled.md) property for the Split Button control should be invalidated after one or more child items are enabled or disabled. This ensures that the framework queries the updated property value and refreshes the state of the Split Button control in the ribbon UI.
</blockquote>
<br/> <br/></td>
</tr>
<tr class="even">
<td>[UI_PKEY_Keytip](windowsribbon-reference-properties-uipkey-keytip.md)</td>
<td>Can only be updated through invalidation.</td>
</tr>
<tr class="odd">
<td>[UI_PKEY_TooltipDescription](windowsribbon-reference-properties-uipkey-tooltipdescription.md)</td>
<td>Can only be updated through invalidation.</td>
</tr>
<tr class="even">
<td>[UI_PKEY_TooltipTitle](windowsribbon-reference-properties-uipkey-tooltiptitle.md)</td>
<td>Can only be updated through invalidation.</td>
</tr>
</tbody>
</table>



 

## Related topics

<dl> <dt>

[Windows Ribbon Framework Control Library](windowsribbon-controls-entry.md)
</dt> <dt>

[**SplitButton markup element**](windowsribbon-element-splitbutton.md)
</dt> </dl>

 

 




