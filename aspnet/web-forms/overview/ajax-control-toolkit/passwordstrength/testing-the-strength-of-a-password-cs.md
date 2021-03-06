---
uid: web-forms/overview/ajax-control-toolkit/passwordstrength/testing-the-strength-of-a-password-cs
title: "測試密碼 (C#) 的強度 |Microsoft 文件"
author: wenz
description: "密碼是必要幾乎任何地方，如此延遲使用者傾向於選擇簡單的密碼，這很容易中斷。 在 ASP PasswordStrength 控制項。N..."
ms.author: aspnetcontent
manager: wpickett
ms.date: 06/02/2008
ms.topic: article
ms.assetid: cb4afbae-9b8f-483d-9729-476d4b9f85fc
ms.technology: dotnet-webforms
ms.prod: .net-framework
msc.legacyurl: /web-forms/overview/ajax-control-toolkit/passwordstrength/testing-the-strength-of-a-password-cs
msc.type: authoredcontent
ms.openlocfilehash: eda7baae1833b074ba34d8f10fa434df14cc592e
ms.sourcegitcommit: 9a9483aceb34591c97451997036a9120c3fe2baf
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/10/2017
---
<a name="testing-the-strength-of-a-password-c"></a>測試的強度的密碼 (C#)
====================
由[Christian Wenz](https://github.com/wenz)

[下載程式碼](http://download.microsoft.com/download/9/3/f/93f8daea-bebd-4821-833b-95205389c7d0/PasswordStrength0.cs.zip)或[下載 PDF](http://download.microsoft.com/download/2/d/c/2dc10e34-6983-41d4-9c08-f78f5387d32b/passwordstrength0CS.pdf)

> 密碼是必要幾乎任何地方，如此延遲使用者傾向於選擇簡單的密碼，這很容易中斷。 在 ASP.NET AJAX Control Toolkit PasswordStrength 控制項可以檢查密碼妥當。


## <a name="overview"></a>概觀

密碼是必要幾乎任何地方，如此延遲使用者傾向於選擇簡單的密碼，這很容易中斷。 `PasswordStrength` ASP.NET AJAX Control Toolkit 中的控制項可以檢查密碼是否妥當。

## <a name="steps"></a>步驟

`PasswordStrength`控制項延伸文字方塊中，並檢查是否夠好中它的密碼。 它提供豐富的選項，透過屬性;以下是只是某些它們：

- `MinimumNumericCharacters`密碼所需的數字字元數目下限
- `MinimumSymbolCharacters`密碼所需的符號字元 （沒有字母和數字） 的最小的數目
- `PreferredPasswordLength`最小密碼長度
- `RequiresUpperAndLowerCaseCharacters`是否必須使用大寫和小寫字元的密碼

`StrengthIndicatorType`提供的資訊如何呈現的強度密碼，以文字 (值`"Text"`) 或做為一種進度列 (值`"BarIndicator"`)。 在`DisplayPosition`屬性，您將設定在出現的資訊。 以下是完整的範例，包括 ASP.NET AJAX`ScriptManager`控制項，`PasswordStrength`控制項和當然文字方塊中，使用者可以在其中輸入密碼。 為了示範，後者的表單欄位為一般文字和密碼欄位，讓您可以查看在開發期間您輸入。

[!code-aspx[Main](testing-the-strength-of-a-password-cs/samples/sample1.aspx)]

執行網頁，並立即輸入： 僅為以視為輸入小寫字母、 大寫字母、 數字和符號之後，密碼。


[![現在，密碼是 （） 好](testing-the-strength-of-a-password-cs/_static/image2.png)](testing-the-strength-of-a-password-cs/_static/image1.png)

密碼 （） 好現在 ([按一下以檢視完整大小的影像](testing-the-strength-of-a-password-cs/_static/image3.png))

>[!div class="step-by-step"]
[下一步](testing-the-strength-of-a-password-vb.md)
