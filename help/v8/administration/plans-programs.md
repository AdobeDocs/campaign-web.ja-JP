---
audience: end-user
title: プランとプログラム
description: Adobe Campaignでプランとプログラムを作成および設定する方法について説明します
exl-id: 0307bcb7-7ab5-4226-bad1-cb7cf10e97fc
source-git-commit: bb61fdb34fecb4131d4069965cda8a3a5099b6bc
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# プランとプログラム {#plan-and-programs}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="プランとプログラム"
>abstract="Campaign web ユーザーインターフェイスで、マーケティングプランおよびプログラムのフォルダー階層を設定できるようになりました。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=ja" text="リリースノートを参照してください"

Adobe Campaignでは、マーケティングプランおよびプログラムのフォルダー階層を設定できます。

より適切に整理するために、Adobeでは次の階層をお勧めします。計画 `>` プログラム `>` キャンペーン

* A **計画** 複数のプログラムを含めることができます。 一定期間の戦略目標を定義します。
* A **プログラム** キャンペーン、ワークフロー、ランディングページなど、他のプログラムも含めることができます。
* A **campaign** には、配信、ワークフロー、ランディングページが含まれる場合があります。

## プランの作成と設定 {#create-plan}

プランを作成するには、フォルダータイプを持つフォルダーを作成する必要があります **[!UICONTROL プラン]** [フォルダー作成の詳細情報](create-manage-folder.md).

![](assets/plan_create.png){zoomable="yes"}

に移動します **[!UICONTROL フォルダー設定]** 管理する計画を持っています。

![](assets/plan_settings.png){zoomable="yes"}

以下を定義できます。 **[!UICONTROL カスタムオプション]**、および計画のスケジュール日を設定します。

![](assets/plan_options.png){zoomable="yes"}

を管理するには  **[!UICONTROL カスタムオプション]**:

1. を参照してください。 **[!UICONTROL スキーマ]**
1. を選択します。 **[!UICONTROL 編集可能]** フィルターのスキーマ
1. アイコンをクリックする **[!UICONTROL カスタム詳細の編集]**

![](assets/plan_edit.png){zoomable="yes"}

次の設定を行うことができます。

![](assets/plan_customfields.png){zoomable="yes"}

## プログラムの作成と設定

プランでプログラムを作成するには、次を行います（[プラン作成の詳細情報](#create-plan)）を選択し、フォルダータイプのフォルダーを作成する必要があります **[!UICONTROL プログラム]** [フォルダー作成の詳細情報](create-manage-folder.md).

![](assets/program_create.png){zoomable="yes"}

に移動します **[!UICONTROL フォルダー設定]** 管理するプログラムの。

![](assets/program_settings.png){zoomable="yes"}

以下を定義できます。 **[!UICONTROL カスタムオプション]**、およびプログラムのスケジュール日を設定します。

![](assets/program_options.png){zoomable="yes"}

を管理するには  **[!UICONTROL カスタムオプション]**:

1. を参照してください。 **[!UICONTROL スキーマ]**
1. を選択します。 **[!UICONTROL 編集可能]** フィルターのスキーマ
1. アイコンをクリックする **[!UICONTROL カスタム詳細の編集]**

![](assets/program_edit.png){zoomable="yes"}

これらを設定できます。

![](assets/program_customfields.png){zoomable="yes"}

## キャンペーンをプログラムにリンクする方法

キャンペーンをプログラムにリンクするには、次の 2 つの方法があります。

### 方法#1：既にプログラムがあり、そのプログラムにリンクされたキャンペーンを作成する必要があります

新しいキャンペーンをプログラムにリンクするには、プログラムでキャンペーンを直接作成します。

![](assets/program_campaign_create.png){zoomable="yes"}

この **[!UICONTROL フォルダー]** 設定は、プログラムへのパスと共に自動的に入力されます。

![](assets/program_campaign_folder.png){zoomable="yes"}

### 方法#2 既にキャンペーンがあり、既存のプログラムにリンクしたい場合

に移動します **[!UICONTROL 設定]** プログラムにリンクするキャンペーンのボタン：

![](assets/campaign_settings.png){zoomable="yes"}

その中で **[!UICONTROL プロパティ]**&#x200B;を選択し、 **[!UICONTROL フォルダー]** アイコン **[!UICONTROL フォルダー]** 設定（を選択するために使用） **[!UICONTROL プログラム]** フォルダー。

![](assets/campaign_folder.png){zoomable="yes"}

を選択 **[!UICONTROL プログラム]** フォルダーを開き、クリックします。 **[!UICONTROL 確認]** ボタン、次にオン **[!UICONTROL 保存して閉じる]** ボタン。

![](assets/campaign_linked.png){zoomable="yes"}

キャンペーンがプログラムにリストされました。

![](assets/campaign_in_program.png){zoomable="yes"}
