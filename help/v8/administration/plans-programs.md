---
audience: end-user
title: プランとプログラム
description: Adobe Campaign でプランとプログラムを作成および設定する方法を学ぶ
exl-id: 0307bcb7-7ab5-4226-bad1-cb7cf10e97fc
TQID: https://experienceleague.adobe.com/FSiHCjupRlS0zoI9HPdcU--Y2PZot5fQOzWICwmV-oQ
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
  - id: b82389f8-9b5e-4083-8e3b-3cef299fb8b9
    internal-label: Schemas
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 404a5a4f1d793404a326feb07cd6869aa97af664
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 100%
---
# プランとプログラム {#plan-and-programs}

Adobe Campaign では、マーケティングのプランとプログラムに関するフォルダー階層構造を設定できます。

これらのコンポーネントをより適切に整理するには、アドビではプラン`>`プログラム`>`キャンペーンの階層を使用することをお勧めします。

* **プラン**&#x200B;には複数のプログラムを含めることができます。 特定の期間の戦略目標を定義します。
* **プログラム**&#x200B;には、キャンペーン、ワークフロー、ランディングページに加えて、他のプログラムを含めることができます。
* **キャンペーン**&#x200B;には、配信、ワークフロー、ランディングページを含めることができます。

## プランの作成と設定 {#create-plan}

プランを作成するには、フォルダータイプが&#x200B;**[!UICONTROL プラン]**&#x200B;のフォルダーを作成する必要があります。 [詳しくは、フォルダーの作成を参照してください](../get-started/work-with-folders.md)。

![プランのフォルダーの作成を示すスクリーンショット](assets/plan_create.png){zoomable="yes"}

プランを管理するには、プランの&#x200B;**[!UICONTROL フォルダー設定]**&#x200B;に移動します。

![プランのフォルダー設定を示すスクリーンショット](assets/plan_settings.png){zoomable="yes"}

**[!UICONTROL カスタムオプション]**&#x200B;を定義し、プランのスケジュール日を設定します。

![プランのカスタムオプションを示すスクリーンショット](assets/plan_options.png){zoomable="yes"}

**[!UICONTROL カスタムオプション]**&#x200B;を管理するには：

1. **[!UICONTROL スキーマ]**&#x200B;を参照します。
1. フィルターで&#x200B;**[!UICONTROL 編集可能]**&#x200B;なスキーマを選択します。
1. スキーマをクリックします。

![プランのカスタム詳細の編集を示すスクリーンショット](assets/plan_edit.png){zoomable="yes"}

1. 「**[!UICONTROL 画面の編集]**」ボタンをクリックします。

   ![](assets/plan_edit2.png){zoomable="yes"}

カスタムオプションを設定します。

![プランのカスタムフィールドの設定を示すスクリーンショット](assets/plan_customfields.png){zoomable="yes"}

## プログラムの作成と設定 {#create-program}

プログラムは、キャンペーン、配信、ワークフローのリスト表示と同様に、プログラムは左側のナビゲーションメニューから使用できます。 **[!UICONTROL プログラム]**&#x200B;エントリでは、プランの下ではなく、既存のプログラム内にプログラムを作成できます。

プランに最初の上位レベルのプログラムを作成するには、エクスプローラーでプランに移動し（この[節](#create-plan)を参照）、フォルダータイプが&#x200B;**[!UICONTROL プログラム]**&#x200B;のフォルダーを作成します。 [詳しくは、フォルダーの作成を参照してください](../get-started/work-with-folders.md)。

既存のプログラム内にプログラムを作成するには、次の手順に従います。

1. 左側のナビゲーションメニューで&#x200B;**[!UICONTROL プログラム]**&#x200B;エントリに移動します。 このビューには、すべてのプログラムが一覧表示され、検索やフィルタリングを実行できます。 プログラムをクリックすると、エクスプローラービューで開きます。

   ![プログラムのリスト表示を示すスクリーンショット](assets/program_view.png){zoomable="yes"}

1. 「**[!UICONTROL プログラムを作成]**」をクリックし、次のオプションを設定します。

   ![「プログラムを作成」画面を示すスクリーンショット](assets/program_create.png){zoomable="yes"}

   * **[!UICONTROL ラベル]**&#x200B;を入力します。
   * **[!UICONTROL 親フォルダー]**&#x200B;として使用する既存のプログラムを選択します。
   * オプションとして、「**[!UICONTROL スケジュール]**」セクションで&#x200B;**[!UICONTROL 日付範囲]**&#x200B;を設定します。

   >[!TIP]
   >
   >エクスプローラービューからプログラムを作成すると、親フォルダーが現在のプログラムに自動的に設定されます。

1. 「**[!UICONTROL プログラムを作成]**」をもう一度クリックして、変更を保存し、プログラムを作成します。 その後、エクスプローラービューにプログラムが表示されます。 他のフォルダーと同様に、名前変更や削除を行ったり、設定にアクセスしたりできます。 また、このプログラム内でサブプログラムを作成することもできます。

   ![エクスプローラービューでプログラムを示すスクリーンショット](assets/program_explorer.png){zoomable="yes"}

プログラムのカスタムオプションは、プランと同様に設定します。 [プランの作成と設定](#create-plan)を参照してください。

## キャンペーンをプログラムにリンクする方法

キャンペーンをプログラムにリンクするには、次の 2 つの方法があります。

### 方法 1：既にプログラムがあり、このプログラムにリンクされたキャンペーンを作成する場合

新しいキャンペーンをプログラムにリンクするには、プログラム内でキャンペーンを直接作成します。

![プログラム内のキャンペーンの作成を示すスクリーンショット](assets/program_campaign_create.png){zoomable="yes"}

**[!UICONTROL フォルダー]**&#x200B;設定は、プログラムへのパスと共に自動的に入力されます。

![プログラムにリンクされたキャンペーンのフォルダー設定を示すスクリーンショット](assets/program_campaign_folder.png){zoomable="yes"}

### 方法 2：既にキャンペーンがあり、このキャンペーンを既存のプログラムにリンクする場合

プログラムにリンクするキャンペーンの「**[!UICONTROL 設定]**」ボタンに移動します。

![キャンペーンの設定ボタンを示すスクリーンショット](assets/campaign_settings.png){zoomable="yes"}

**[!UICONTROL プログラム]**&#x200B;フォルダーを選択するには、**[!UICONTROL プロパティ]**&#x200B;で&#x200B;**[!UICONTROL フォルダー]**&#x200B;設定の&#x200B;**[!UICONTROL フォルダー]**&#x200B;アイコンをクリックします。

![キャンペーンをプログラムにリンクするフォルダー選択を示すスクリーンショット](assets/campaign_folder.png){zoomable="yes"}

**[!UICONTROL プログラム]**&#x200B;フォルダーを選択し、「**[!UICONTROL 確認]**」ボタンをクリックして、「**[!UICONTROL 保存して閉じる]**」ボタンをクリックします。

![プログラムにリンクされたキャンペーンを示すスクリーンショット](assets/campaign_linked.png){zoomable="yes"}

キャンペーンがプログラムにリストされました。

![プログラム内でリストされたキャンペーンを示すスクリーンショット](assets/campaign_in_program.png){zoomable="yes"}