---
title: Adobe CampaignへのGenStudio for Performance Marketingの取り込み
description: Adobe CampaignでGenStudio for Performance Marketingを使用する方法を学ぶ
feature: Email Design
topic: Content Management, Artificial Intelligence
role: User
level: Beginner, Intermediate
exl-id: c22a44a8-e4e2-453a-9ca2-b80f7c0edc19
source-git-commit: 61e6dcf13fc6a405f5e25328bf336e863701b2fe
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 9%

---

# パフォーマンスマーケティング用の GenStudio の操作 {#genstudio}

>[!CONTEXTUALHELP]
>id="ac_genstudio_button"
>title="GenStudio で作成したテンプレートの使用"
>abstract="GenStudio for Performance Marketing とのシームレスな統合により、Adobe AI テクノロジーで強化された GenStudio テンプレートを簡単に読み込むことができます。"

## GenStudioの概要 {#gs-genstudio}

[Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/ja/docs/genstudio-for-performance-marketing/user-guide/home){target="_blank"} は、生成 AI ファーストのアプリケーションで、マーケティングチームが独自の広告やメールを作成し、ブランド標準を遵守し、企業ポリシーに準拠した、インパクトのあるパーソナライズされたマーケティングキャンペーンを推進できるようにします。 Adobeの AI テクノロジーを活用することで、コンテンツの作成と管理の複雑さを軽減する包括的なツールスイートを提供し、クリエイティブ担当者がイノベーションに集中できるようにします。

>[!AVAILABILITY]
>
>この機能は、メールチャネルでのみ使用できます。

マーケティング効率を高め、ブランドの一貫性を保つために、[!DNL **GenStudio for Performance Marketing**] のエクスペリエンスを [!DNL **Adobe Campaign**] とシームレスに統合できます。 これにより、[!DNL GenStudio] の高度なオーケストレーション機能に加えて、[!DNL Adobe Campaign] の AI 機能を活用したコンテンツ作成が可能になります。

>[!INFO]
>
>詳細については、こちらの [&#x200B; 概要 &#x200B;](https://business.adobe.com/jp/products/genstudio-for-performance-marketing.html#watch-overview){target="_blank"} と [&#x200B; の &#x200B;](https://business.adobe.com/jp/products/genstudio-for-performance-marketing.html#demo){target="_blank"} デモ [!DNL Adobe GenStudio for Performance Marketing] を参照してください。

## Adobe CampaignでのGenStudio機能の使用 {#use-genstudio}

[!DNL GenStudio for Performance Marketing] と [!DNL Adobe Campaign] の統合により、会社のマーケターがより適切に連携してプロセスを合理化できます。

例えば、[!DNL Adobe Campaign] を使用してメールキャンペーンを開発および自動化するテクニカルマーケターは、[!DNL GenStudio] を使用してコンテンツを作成するパフォーマンスマーケターと共同作業できます。

この統合により、両方の組織が連携してオンブランドのコンテンツを [!DNL GenStudio] から [!DNL Adobe Campaign] に簡単に統合し、特定の顧客セグメントをターゲットにして売上を伸ばす魅力的なメールを配信できます。

### Adobe CampaignからGenStudioへのHTML テンプレートの書き出し {#export-from-campaign-to-genstudio}

まず、ブランドのガイドラインを含んだ [!DNL Adobe Campaign] HTML テンプレートを [!DNL GenStudio for Performance Marketing] に書き出すことができます。 以下の手順に従います。

1. [!DNL Adobe Campaign] で、メールのコンテンツにアクセスします。 [詳細情報](../email/create-email.md#create-content)

1. メールDesignerで、「**[!UICONTROL 詳細]**」ボタンから **[!UICONTROL HTMLを書き出]** を選択します。

   ![](assets/genstudio-export-template.png){zoomable="yes"}

1. このHTMLに書き出したテンプレートを [!DNL GenStudio for Performance Marketing] にアップロードします。<!--Make sure you detect the fields that the generative AI uses to insert content in order to create an actionable template.-->

   >[!NOTE]
   >
   >HTML テンプレートを [!DNL GenStudio] にアップロードする方法については、[Adobe GenStudio for Performance Marketing ユーザーガイド &#x200B;](https://experienceleague.adobe.com/ja/docs/genstudio-for-performance-marketing/user-guide/content/templates/use-templates#templates-from-ajo-and-marketo){target="_blank"} 専用の節を参照してください。<!--GenStudio doc to be updated with Campaign-->

1. GenStudioでは、このテンプレートを使用して、AI プロンプトで複数のメールのバリエーションを作成し、保存します。

   >[!NOTE]
   >
   >メールエクスペリエンスを作成する方法については、GenStudio専用の [&#x200B; 節 &#x200B;](https://experienceleague.adobe.com/ja/docs/genstudio-for-performance-marketing/user-guide/create/create-email-experience){target="_blank"} を参照してください。

### Adobe CampaignでのGenStudio エクスペリエンスの活用 {#leverage-genstudio-experiences}

[!DNL GenStudio] に読み込んで作成した [!DNL Adobe Campaign] メールのバリエーションを活用するには、次の手順に従います。

1. [!DNL Adobe Campaign]: [&#x200B; メール配信を作成 &#x200B;](../email/create-email.md)。

1. メール配信ダッシュボードで、「**[!UICONTROL コンテンツを編集]**」ボタンをクリックします。 [詳細情報](../email/create-email.md#create-content)

1. 電子メールDesignerのホームページで、「**[!UICONTROL HTMLを読み込む]** を選択し、「**[!UICONTROL Adobe GenStudio for Performance Marketing]**」ボタンをクリックします。

   ![](assets/genstudio-pem-import-email.png){zoomable="yes"}

1. GenStudioのエクスペリエンスを参照して、コンテンツの作成を開始します。 製品、ペルソナ、ブランド、さらには色など、複数の条件でエクスペリエンスをフィルタリングできます。

   <!--![](assets/genstudio-filter-experiences.png){zoomable="yes"}-->

1. エクスペリエンスを選択し、「**[!UICONTROL 使用]**」をクリックします。

   ![](assets/genstudio-use-experience.png){zoomable="yes"}

1. GenStudio エクスペリエンスを読み込むフォルダーを選択します。

   ![](assets/genstudio-choose-destination.png){zoomable="yes"}

1. 選択したコンテンツが電子メールDesignerに表示されます。

   ![](assets/genstudio-email-content.png){zoomable="yes"}

   >[!NOTE]
   >
   >GenStudioのエクスペリエンス [&#x200B; テンプレートから作成  [!DNL Adobe Campaign]  は &#x200B;](#export-from-ajo-to-genstudio) メールDesignerに直接読み込まれます。 [!DNL Adobe Campaign] テンプレートなしで作成されたGenStudio エクスペリエンスは、[&#x200B; 互換モード &#x200B;](../email/existing-content.md) に読み込まれます。

   [&#x200B; メールコンテンツ編集ツール &#x200B;](../email/create-email-content.md) および [&#x200B; パーソナライゼーションフィールド &#x200B;](../personalization/personalize.md) を使用して、メールを必要に応じて編集します。 コンテンツを保存します。

<!--Detail a use case with A/B testing to import other GenStudio variations and track how your tratments are performing.-->


<!--
## How-to video {#video}

Discover the process of exporting an email template from Adobe Campaign to GenStudio for Performance Marketing, crafting brand-compliant emails using the template in GenStudio, and importing them seamlessly back into Adobe Campaign.

>[!VIDEO](https://video.tv.adobe.com/v/3456038/?quality=12)
TO REPLACE WITH CAMPAIGN VIDEO WHEN/IF RELEASED
-->