---
title: ダークモードに切り替え
description: Adobe Campaign E メールデザイナーでのダークモードの使用方法について説明します。
feature: Email Design
topic: Content Management
role: User
level: Beginner, Intermediate
keywords: ダークモード, メール, カラー, エディター
hide: true
hidefromtoc: true
source-git-commit: b85a78cf89586679630398f5f3c7d732a59711fd
workflow-type: tm+mt
source-wordcount: '1515'
ht-degree: 100%

---

# ダークモードコンテンツの管理 {#dark-mode}

>[!CONTEXTUALHELP]
>id="ac_edition_darkmode"
>title="ダークモードに切り替え"
>abstract="ダークモードに切り替えると、レンダリング方法のプレビューや、特定のカスタム設定の定義ができます。<br>最終的なレンダリングは、受信者のメールクライアントに応じて異なります。すべてのメールクライアントがカスタムダークモードをサポートしているわけではありません。"

>[!CONTEXTUALHELP]
>id="ac_edition_darkmode_preview"
>title="ダークモードに切り替え"
>abstract="ダークモードに切り替えると、サポートされているメールクライアントでどのようにレンダリングされるかをプレビューできます。 <br>最終的なレンダリングは、受信者のメールクライアントに応じて異なります。すべてのメールクライアントがダークモードをサポートしているわけではありません。"

メールをデザインする際に、[!DNL Adobe Campaign] [E メールデザイナー](get-started-email-designer.md)を使用すると、**[!UICONTROL ダークモード]**&#x200B;ビューに切り替えることができます。

この<!--Email Designer -->ダークモードビューでは、ダークモードがオンの場合にサポートしているメールクライアントに表示される特定のカスタム設定を定義することもできます。

## ダークモードとは {#what-is-dark-mode}

様々なメールクライアントでダークモードがレンダリングされる方法は複雑です。まず、ダークモードを定義します。

ダークモードを使用すると、サポートしているメールクライアントとアプリで、メールの背景を暗くし、テキスト、ボタン、他の UI 要素を明るい色で表示できます。目への負担を軽減し、バッテリー寿命を短縮し、低照度環境での読みやすさを向上させて、より快適な視聴エクスペリエンスを実現します。

これは、主要なオペレーティングシステムとアプリ<!-- (Apple Mail, Gmail, Outlook, Twitter, Slack)-->全体で高まるトレンドとして、すべてのユーザーにとってコンテンツが読みやすく視覚的に魅力的であることを確保するために、最新のメールデザインでは重要な考慮事項になっています。

## ガードレール {#guardrails}

ダークモードのレンダリングに関する期待は、様々なメールクライアントによって適用方法が大きく異なる可能性があるので、慎重に考慮する必要があります。

<!--The dark mode final rendering depends on the recipient's email client. It is not possible to guarantee that your email will look the same in dark mode across all devices.-->

[!DNL Adobe Campaign] E メールデザイナーでダークモードを使用する前に、メインのメールクライアントでの処理方法を理解することが重要です。区別するケースには、次の 3 つがあります。

<!--
* Check out the list of [email clients supporting dark mode](https://www.caniemail.com/search/?s=dark){target="_blank"}

* Learn more on Dark mode in this [Litmus blog post](https://www.litmus.com/blog/the-ultimate-guide-to-dark-mode-for-email-marketers){target="_blank"}
-->

### ダークモードをサポートしていないクライアント {#not-supporting}

次のような一部のメールクライアントでは、この機能をまったくサポートしていません。

* Yahoo! メール
* AOL

E メールデザイナーでダークモードのカスタム設定を定義したかどうかに関係なく、これらのメールクライアントではダークモードのレンダリングを表示しません。<!--Regardless of whether the interface is in light or dark mode, your email will render the same.-->

### 独自のダークモードを適用しているクライアント {#default-support}

一部のメールクライアントでは、受信したすべてのメールに対して、独自のデフォルトのダークモードが体系的に適用されます。色、背景、画像など はメールクライアント固有のダークモード設定で自動的に調整されるので、外部からの変更はできません。

<!--It is important to note that less than 25% of email clients offer customization options for dark mode. Clients such as Gmail implement their own dark mode rendering, which is not subject to external modification.-->

これらのクライアントの例：

* Gmail（デスクトップ web メール、iOS、Android、モバイル web メール）
* Outlook Windows
* Outlook Windows メール

この場合、E メールデザイナーでカスタムダークモード設定を定義すると、これらの設定はメールクライアントの設定で上書きされます。

これらのメールクライアントはダークモードを処理しますが、特定のダークモードデザインはレンダリングされないことを理解することが重要です。

### カスタムダークモードをサポートしているクライアント {#custom-support}

他のメールクライアントには、`@media (prefers-color-scheme: dark)` クエリを使用してカスタムダークモードをレンダリングするオプションが用意されています。これは、[!DNL Journey Optimizer] E メールデザイナーで使用される方法です。

このオプションを処理する主なクライアントのリストを以下に示します。

* Apple メール macOS
* Apple メール iOS
* Outloook macOS
* Outlook.com
* Outloook iOS
* Outloook Android

この場合、E メールデザイナーで定義した特定の設定が表示されます。

>[!NOTE]
>
>E メールデザイナーでカスタムダークモード設定を定義する方法について詳しくは、[この節](#define-custom-dark-mode)を参照してください。

ただし、メールクライアントごとに制限が一部適用される場合があります。例えば、Apple メール 16（macOS 13）などの一部のクライアントでは、メールのコンテンツに画像が存在している場合、ダークモードは生成されません。

最適な結果を得るには、ターゲットにしているメールクライアントでコンテンツをテストします。各クライアントの最終結果にできるだけ近いシミュレーションを表示するには、E メールデザイナーで「[メールレンダリング](../preview-test/email-rendering.md)」オプションを使用します。

## E メールデザイナーでのダークモード {#dark-mode-email-designer}

E メールデザイナーでのダークモードに関しては、考慮すべき 2 つの側面があります。

* サポートされているほとんどのメールクライアントで、デフォルトのダークモードがどのようにレンダリングされるかをプレビューできます。[詳細情報](#preview-dark-mode)

* [カスタムダークモードをサポートしている](#custom-support)メールクライアントのデフォルト設定を上書きする場合は、編集中のメールのカスタム設定を定義できます。[詳細情報](#define-custom-dark-mode)

### デフォルトのダークモードのプレビュー {#preview-dark-mode}

E メールデザイナーでダークモードにアクセスし、デフォルトのダークモード設定のプレビューを取得するには、次の手順に従います。

1. E メールデザイナーのホームページで、「**[!UICONTROL ゼロからデザイン]**」オプションを選択します。[詳細情報](create-email-content.md)

1. [構造](create-email-content.md)と[コンテンツコンポーネント](content-components.md)をコンテンツに追加します。

1. 中央のキャンバスの右上で、切替スイッチを&#x200B;**[!UICONTROL ダークモード]**&#x200B;に切り替えます。

   ![](assets/light-mode-toggle.png)

1. デフォルトのダークモードのプレビューが表示されます。

   ![](assets/dark-mode-default.png)

デフォルトでは、E メールデザイナーのダークモードのプレビューには、画像とアイコンを除くすべての要素に「フルカラー反転」カラースキームが適用されます。

つまり、明るい要素と暗い要素の領域を検出して反転させることで、明るい背景は暗く、暗いテキストは明るくなり、暗い背景は明るく、明るいテキストは暗くなります。

>[!CAUTION]
>
>最終的なレンダリングは、受信者のメールクライアントによって異なる場合があります。各メールクライアントの最終結果にできるだけ近いシミュレーションを表示するには、「[メールレンダリング](../preview-test/email-rendering.md)」オプションを使用します。

### カスタムダークモードの定義 {#define-custom-dark-mode}

>[!CONTEXTUALHELP]
>id="ac_edition_darkmode_image"
>title="特定の画像をダークモードで使用"
>abstract="ダークモードがオンの場合に表示される別の画像を選択できます。 <br>ダークモードで使用する特定の画像を追加しても、すべてのメールクライアントで正しくレンダリングされるとは限りません。 すべてのメールクライアントがカスタムダークモードをサポートしているわけではありません。"

**[!UICONTROL ダークモード]**&#x200B;に切り替えたら、受信者のメールクライアントでダークモードが有効になっている場合にのみ表示されるコンテンツの特定のスタイル要素の編集を選択できます（その機能がサポートされている場合）。

>[!WARNING]
>
>ダークモードの最終的なレンダリングは、各メールクライアントに応じて異なるので、結果はクライアントごとに異なる場合があります。[詳細情報](#guardrails)

<!--
>[!WARNING]
>
>Not all email clients support dark mode. Moreover, some email clients only apply their own default dark mode for all emails that are received. In both cases, the custom settings that you defined in the Email Designer cannot be rendered.-->

E メールデザイナーのカスタムダークモードのスタイル設定を活用するには、Journey Optimizer では<!-- `@media (prefers-color-scheme: dark)` method--> `@media (prefers-color-scheme: dark)` CSS クエリを使用します。このクエリでは、ユーザーのメールクライアントがダークモードに設定されているかどうかを検出し、メールで定義したダークテーマのデザインが適用されます。

カスタムダークモードの設定を定義するには、次の手順に従います。

1. E メールデザイナーで&#x200B;**[!UICONTROL ダークモード]**&#x200B;プレビューに切り替えます。[詳細情報](#preview-dark-mode)

1. テキスト、背景、ボタンなどのスタイル設定の色属性を編集します。

1. 画像やアイコンの色は変更できませんが、特定のアセットはダークモード用にのみ定義できます。

   これを行うには、任意の画像を選択します。**[!UICONTROL 設定]**&#x200B;パネルの専用切替スイッチを使用して&#x200B;**[!UICONTROL ダークモード]**&#x200B;に切り替え、別のアセットを選択します。

   ![](assets/dark-mode-image.png)

   <!--![](assets/dark-mode-custom.png)-->

1. いつでも&#x200B;**[!UICONTROL ライブビューに切り替えて]**、様々なデバイスサイズでコンテンツがどのようにレンダリングされる可能性があるかを確認できます。このビューから、画面上部のダークモード切替スイッチを選択すると、様々なデバイスをまたいでコンテンツのダークモードバージョンをプレビューできます。

   ![](assets/dark-mode-live-view.png){width="80%" align="center"}

   >[!CAUTION]
   >
   >ライブビューは、様々なデバイスサイズをまたいでレンダリングがどのように表示される可能性があるかを比較するのにデザインされた汎用プレビューです。最終的なレンダリングは、受信者のメールクライアントによって異なる場合があります。

1. ダークモードの変更に満足したら、「**[!UICONTROL コンテンツをシミュレート]**」をクリックします。

   ![](assets/dark-mode-simulate.png)

1. 「**[!UICONTROL メールをレンダリング]**」を選択し、Litmus アカウントに接続します。様々なメールクライアントでの最終的なダークモードレンダリングを確認できます。詳しくは、[メールのレンダリング](../preview-test/email-rendering.md)を参照してください。

   >[!WARNING]
   >
   >シミュレーションではダークモードでのメールの表示に非常に近いですが、メールサービスプロバイダーやデバイスレベルの設定の違いにより、実際のレンダリングは異なる場合があります。

## ベストプラクティス {#best-practices}

主要なメールクライアント間でダークモードの採用が増加するにつれて、[カスタムダークモード](#define-custom-dark-mode)を使用しているかどうかに関係なく、明るい環境と暗い環境の両方でメールがどのようにレンダリングされるかを考慮することが重要になります。

ダークモードでは、色、背景、画像が変更される可能性があり、場合によってはデザインの選択が上書きされることもあります。 視覚的な一貫性、アクセシビリティ、ブランドの整合性を確保するには、次に示すベストプラクティスに従ってください。

**画像とロゴの最適化**

* ロゴやアイコンを透明な背景の PNG として保存し、ダークモードで白いボックスが表示されないようにします。

* 白色の背景または明るい背景がハードコードされた画像は回避します。

* 透明度がオプションでない場合は、不自然な色の反転を防ぐために、デザインでは単色の背景に画像を配置します。

**背景に対する考慮事項**

* ライトモードとダークモードの両方で読みやすくするには、テキストと背景色の間に十分なコントラストを確保します。

* 重要なコンテンツについては、背景色にのみ依存することは回避します。一部のクライアントでは、ダークモードで背景色を上書きすることがあるので、重要な情報が表示されていることを確認します。

<!--**Inline critical styles**

Inline CSS helps maintain more control over styling, as some clients strip external styles in dark mode.-->

**ダークモードでのアクセス可能なコンテンツのデザイン**

<!--KEEP dark mode accessibility best practices IN ONE SINGLE LOCATION - for now listed on this page.
If needed, it can be moved to the Design accessible content page:
The best practices for designing accesible content in dark mode are listed in [this section](accessible-content.md#dark-mode).-->

* 色覚異常のある人物でも簡単に区別できる色の組み合わせを使用します。

* 明るい背景と暗い背景の両方に対してコントラストを確保するのに、ミッドトーンパレットを使用します。

* 読みやすさを向上させ、Web コンテンツアクセシビリティガイドライン（WCAG）標準を満たすには、コントラストの高いアクセシブルな色の組み合わせを使用します。WebAIM のコントラストチェッカーなどのツールを使用して、色のコントラストを検証します。

* 読みやすさに影響する場合があるので、細いフォントは回避します。ブランドに細いフォントが必要な場合は、ダークモードで太字にします。

* 純粋な白色に純粋な黒色を重ねると、目への負担の原因となる場合があり、一部のメールクライアントにより自動的に反転される可能性があるので、これを回避します。

* ダークモードがサポートされていない場合は、アクセスできるフォールバックスタイル設定を指定します。

**ダークモード環境でのメールのテスト**

* 問題を早期に発見するには、反転したカラースキームを使用する E メールデザイナーの[ダークモードのプレビュー](#preview-dark-mode)を使用します。

* Litmus を活用した「[メールレンダリング](../preview-test/email-rendering.md)」オプションを使用して、主要なメールクライアント（Apple メール、Gmail、Outlook）でデザインをシミュレートし、ダークモードでの色と画像の動作を確認します。
