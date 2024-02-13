---
audience: end-user
title: Adobe Experience Manager as a Cloud Service でのアセットの管理
description: Adobe Experience Manager as a Cloud Service でコンテンツを管理する方法を説明します
badge: label="限定提供（LA）"
source-git-commit: 6fd2fa72e482883802c96f0888ea79f2b16b7152
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 11%

---

# でテンプレートを管理 [!DNL Adobe Experience Manager as a Cloud service]{#aem-assets}

## [!DNL Adobe Experience Manager as a Cloud service] の基本を学ぶ{#create-aem}

Adobe Campaign Web インターフェイスがAdobe Experience Managerと統合されると、Adobe Experience Managerプラットフォーム内で直接、E メール配信コンテンツやフォームを効率的に管理できます。

![](assets/do-not-localize/book.png)[Adobe Experience Manager as a Cloud Service の詳細](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/sites/authoring/getting-started/quick-start.html?lang=en)

## でテンプレートを作成します。 [!DNL Adobe Experience Manager as a Cloud service]{#create-aem-template}

1. 次の場所に移動： [!DNL Adobe Experience Manager] オーサーインスタンスを作成し、ページの左上隅にある「Adobeエクスペリエンス」をクリックします。 選択 **[!UICONTROL Sites]** を選択します。

1. アクセス **[!UICONTROL キャンペーン/ブランド名/メイン領域/ページ名]**.

1. クリック **[!UICONTROL 作成]** を選択し、 **[!UICONTROL ページ]** をドロップダウンメニューから選択します。

   ![](assets/aem_1.png)

1. を選択します。 **[!UICONTROL Adobe Campaign Email]** ニュースレターをテンプレート化し、名前を付けます。

   ![](assets/aem_2.png)

1. Adobe Campaignのパーソナライゼーションフィールドなどのコンポーネントを追加して、E メールコンテンツをカスタマイズします。 [詳細情報](https://experienceleague.adobe.com/docs/experience-manager-65/content/sites/authoring/aem-adobe-campaign/campaign.html?lang=en#editing-email-content)

1. E メールの準備が整ったら、 **[!UICONTROL ページ情報]** メニューとクリック **[!UICONTROL ワークフローを開始]**.

   ![](assets/aem_3.png)

1. 最初のドロップダウンで、「 」を選択します。 **[!UICONTROL Adobe Campaignを承認]** ワークフローモデルとして、をクリックします。 **[!UICONTROL ワークフローを開始]**.

1. ページの上部に、次の内容の免責事項が表示されます。 `This page is subject to the workflow Approve for Adobe Campaign`. クリック **[!UICONTROL 完了]** 免責事項の横にあるレビューを確認し、をクリックします。 **[!UICONTROL OK]**.

   ![](assets/aem_4.png)

1. クリック **[!UICONTROL 完了]** 再び選択し、 **[!UICONTROL ニュースレターの承認]** （内） **[!UICONTROL 次のステップ]** 」ドロップダウンリストから選択できます。

これでニュースレターが準備でき、Adobe Campaign で同期されました。

## Adobe Experience Manager as a Cloud Service テンプレートのインポート{#aem-templates-perso}

Experience ManagerテンプレートをAdobe Campaign Web でコンテンツテンプレートとして使用できるようになったら、パーソナライゼーションを含め、E メールに必要なコンテンツを特定して組み込むことができます。

1. Campaign Web で、 **[!UICONTROL 配信]** メニュー、クリック **[!UICONTROL 配信を作成]**.

1. E メールのテンプレートウィンドウで、組み込みの **[!UICONTROL AEMコンテンツを含む E メール配信]** テンプレート。

   ![](assets/aem_5.png)

1. を入力します。 **[!UICONTROL ラベル]** 配信の場合は、必要に応じて、追加のオプションを設定します。

   * **[!UICONTROL 内部名]**：配信に一意の ID を割り当てます。

   * **[!UICONTROL フォルダー]**：配信を特定のフォルダーに保存します。

   * **[!UICONTROL 配信コード]**：このフィールドを使用すると、独自の命名規則に基づいて配信を整理できます。

   * **[!UICONTROL 説明]**：配信の説明を指定します。

   * **[!UICONTROL 特性]**：分類目的での電子メールの特性を指定します。

1. 次の項目を定義： **[!UICONTROL 対象ユーザ]** を電子メールに送信します。 [詳細情報](../email/create-email.md#define-audience)

1. クリック **[!UICONTROL コンテンツを編集]**.

1. 次から： **[!UICONTROL コンテンツを編集]** メニュー、クリック **[!UICONTROL AEMコンテンツを選択]**.

   ![](assets/aem_6.png)

1. AEMテンプレートを参照し、Campaign Web にインポートするテンプレートを選択します。

   ![](assets/aem_8.png)

1. テンプレートに直接Adobe Experience Managerで変更が加えられた場合は、 **[!UICONTROL AEMコンテンツを更新]** を追加して、テンプレートの最新バージョンを取得します。

1. Experience Managerと Campaign 間のリンケージを削除したり、E メールデザイナーでExperience Managerテンプレートをさらにパーソナライズするには、 **[!UICONTROL AEMコンテンツのリンク解除]**.

   ![](assets/aem_9.png)

1. パーソナライズされたコンテンツをテンプレートに追加した場合は、Experience Managerの **[!UICONTROL コンテンツをシミュレート]** をクリックし、テストプロファイルを使用して、メッセージでの表示をプレビューします。

[プレビューおよびテストプロファイルの詳細を説明します](../preview-test/preview-content.md)

1. メッセージのプレビューを表示すると、パーソナライズされた要素は、選択したテストプロファイルの対応するデータに自動的に置き換えられます。

   必要に応じて、 **[!UICONTROL テストプロファイルの管理]** 」ボタンをクリックします。

これで、配信を送信する準備が整いました。
