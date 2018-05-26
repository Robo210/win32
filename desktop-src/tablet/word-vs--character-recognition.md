---
Description: By setting the Factoid property to None, the character recognizer recognizes handwriting on a character-by-character basis.
ms.assetid: 4dacceab-032e-4b9b-858f-67961fd587b5
title: Word vs. Character Recognition
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# Word vs. Character Recognition

By setting the [Factoid](frlrfMicrosoftInkInkEditClassFactoidTopic) property to **None**, the character recognizer recognizes handwriting on a character-by-character basis.

The [RecoTimeout](frlrfMicrosoftInkInkEditClassRecoTimeoutTopic) ([**RecoTimeout**](/windows/win32/inked/?branch=master) in Automation) property specifies the number of milliseconds of delay between the last [Stroke](frlrfMicrosoftInkStrokeClassTopic) and the end of handwriting input. You can increase this value to recognize text before entire words or sentences are written. You can also force the recognition of ink immediately by using the [Recognize](frlrfMicrosoftInkInkEditClassRecognizeTopic) method.

 

 


