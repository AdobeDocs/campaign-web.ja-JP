---
audience: end-user
title: Adobe Experience Manager as a Cloud Service でのアセットの管理
description: Adobe Experience Manager as a Cloud Service でのコンテンツの管理方法について説明します
exl-id: 43b186c8-294e-4cbe-b269-e127065515ed
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 37%

---

# [!DNL Adobe Experience Manager as a Cloud Service] でのテンプレートを管理する{#aem-assets}

## [!DNL Adobe Experience Manager as a Cloud Service] の基本を学ぶ{#create-aem}

Adobe Campaign web インターフェイスをAdobe Experience Managerと統合すると、メール配信のコンテンツとフォームをAdobe Experience Manager Platform 内で直接効率的に管理できます。

![](assets/do-not-localize/book.png) [Adobe Experience Manager as a Cloud Serviceの詳細情報 ](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/sites/authoring/getting-started/quick-start.html?lang=ja)

## [!DNL Adobe Experience Manager as a Cloud Service] でテンプレートを作成する{#create-aem-template}

1. [!DNL Adobe Experience Manager] オーサーインスタンスに移動して、ページの左上隅にある「Adobe Experience」をクリックします。 メニューから「**[!UICONTROL Sites]**」を選択します。

1. **[!UICONTROL キャンペーン／ブランド名／メイン領域／ページ名]**&#x200B;にアクセスします。

1. **[!UICONTROL 作成]** をクリックし、ドロップダウンメニューから **[!UICONTROL ページ]** を選択します。

   ![ ドロップダウンメニューの「作成」ボタンと「ページ」オプションを示すスクリーンショット。](assets/aem_1.png)

1. **[!UICONTROL Adobe Campaign メール]** テンプレートを選択し、ニュースレターに名前を付けます。

   ![[ 「Adobe Campaign メール」テンプレートの選択と命名フィールドを示すスクリーンショット。]](assets/aem_2.png)

1. Adobe Campaignのパーソナライゼーションフィールドなどのコンポーネントを追加して、メールコンテンツをカスタマイズします。 [詳細情報](https://experienceleague.adobe.com/docs/experience-manager-65/content/sites/authoring/aem-adobe-campaign/campaign.html?lang=ja#editing-email-content)

1. メールの準備が整ったら、**[!UICONTROL ページ情報]** メニューに移動し、「**[!UICONTROL ワークフローを開始]**」をクリックします。

   ![ 「ページ情報」メニューと「ワークフローを開始」オプションを示したスクリーンショット。](assets/aem_3.png)

1. 最初のドロップダウンから、ワークフローモデルとして **[!UICONTROL Adobe Campaignを承認]** を選択し、「**[!UICONTROL ワークフローを開始]**」をクリックします。

1. ページの上部に `This page is subject to the workflow Approve for Adobe Campaign` という免責事項が表示されます。免責事項の横にある「**[!UICONTROL 完了]**」をクリックしてレビューを確定し、「**[!UICONTROL OK]**」をクリックします。

   ![ 免責事項を示すスクリーンショットと「完了」ボタン。](assets/aem_4.png)

1. もう一度 **[!UICONTROL 完了]** をクリックし、「次の手順 **&#x200B;**&#x200B;ドロップダウンで **[!UICONTROL ニュースレターの承認]** を選択します。

これでニュースレターが準備でき、Adobe Campaign で同期されました。

## Adobe Experience Manager as a Cloud Service テンプレートの読み込み{#aem-templates-perso}

Experience Manager テンプレートが Adobe Campaign Web でコンテンツテンプレートとして使用可能になると、パーソナライゼーションを含むメールに必要なコンテンツを特定して組み込むことができます。

1. Campaign Web で、**[!UICONTROL 配信]**&#x200B;メニューから、「**[!UICONTROL 配信を作成]**」をクリックします。

1. メールテンプレートウィンドウで、組み込みの「**[!UICONTROL AEM コンテンツでメール配信]**」テンプレートを選択します。

   ![ 「AEM コンテンツでメール配信」テンプレートの選択を示したスクリーンショット。](assets/aem_5.png)

1. 配信の **[!UICONTROL ラベル]** を入力し、必要に応じて追加のオプションを設定します。

   * **[!UICONTROL 内部名]**：配信に一意の ID を割り当てます。
   * **[!UICONTROL フォルダー]**：配信を特定のフォルダーに保存します。
   * **[!UICONTROL 配信コード]**：このフィールドを使用すると、独自の命名規則に基づいて配信を整理できます。
   * **[!UICONTROL 説明]**：配信の説明を指定します。
   * **[!UICONTROL 特性]**：分類目的でメールの特性を指定します。

1. メールの **[!UICONTROL オーディエンス]** を定義します。 [詳細情報](../email/create-email.md#define-audience)

1. 「**[!UICONTROL コンテンツを編集]**」をクリックします。

1. **[!UICONTROL コンテンツを編集]**&#x200B;メニューから、「**[!UICONTROL AEM コンテンツを選択]**」をクリックします。

   ![ 「コンテンツを編集」メニューの「AEMコンテンツを選択」オプションを示すスクリーンショット ](assets/aem_6.png)

1. Campaign Web にインポートするAEM テンプレートを選択します。

   ![AEM テンプレートの選択インターフェイスを示すスクリーンショット。](assets/aem_8.png)

1. コンテンツは自動的には同期されません。テンプレートがAdobe Experience Managerで直接変更された場合は、「**[!UICONTROL AEM コンテンツを更新]**」を選択して、テンプレートの最新バージョンに更新します。

1. Experience Managerと Campaign のリンクを解除したり、電子メールデザイナーでExperience Manager テンプレートをさらにパーソナライズしたりするには、「**[!UICONTROL AEM コンテンツのリンクを解除]**」をクリックします。

   ![ 「AEMコンテンツのリンクを解除」オプションを示したスクリーンショット。](assets/aem_9.png)

1. パーソナライズされたコンテンツを Experience Manager テンプレートに追加した場合は、「**[!UICONTROL コンテンツをシミュレート]**」をクリックして、テストプロファイルを使用してメッセージでの表示をプレビューします。

[プレビューおよびテストプロファイルの詳細情報](../preview-test/preview-content.md)

1. メッセージプレビューを表示する際、パーソナライズされた要素は、選択したテストプロファイルからの対応するデータに自動的に置き換えられます。

   必要に応じて、「テストプロファイルを管理 **[!UICONTROL ボタンからテストプロファイルを追加]** ます。

配信の送信準備が整いました。