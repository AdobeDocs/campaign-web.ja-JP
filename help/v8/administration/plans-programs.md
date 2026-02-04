---
audience: end-user
title: プランとプログラム
description: Adobe Campaign でプランとプログラムを作成および設定する方法を学ぶ
exl-id: 0307bcb7-7ab5-4226-bad1-cb7cf10e97fc
source-git-commit: 1a751aed6d5185e700dafb1de2afd88300dfcd79
workflow-type: ht
source-wordcount: '522'
ht-degree: 100%

---

# プランとプログラム {#plan-and-programs}

Adobe Campaign では、マーケティングのプランとプログラムに関するフォルダー階層構造を設定できます。

これらのコンポーネントをより適切に整理するには、アドビではプラン`>`プログラム`>`キャンペーンの階層を使用することをお勧めします。

* **プラン**&#x200B;には複数のプログラムを含めることができます。特定の期間の戦略目標を定義します。
* **プログラム**&#x200B;には、キャンペーン、ワークフロー、ランディングページに加えて、他のプログラムを含めることができます。
* **キャンペーン**&#x200B;には、配信、ワークフロー、ランディングページを含めることができます。

## プランの作成と設定 {#create-plan}

プランを作成するには、フォルダータイプが&#x200B;**[!UICONTROL プラン]**&#x200B;のフォルダーを作成する必要があります。[詳しくは、フォルダーの作成を参照してください](../get-started/work-with-folders.md)。

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

## プログラムの作成と設定

プランにプログラムを作成するには（[詳しくは、プランの作成を参照してください](#create-plan)）、プランに移動し、フォルダータイプが&#x200B;**[!UICONTROL プログラム]**&#x200B;のフォルダーを作成します。[詳しくは、フォルダーの作成を参照してください](../get-started/work-with-folders.md)。

![プログラムのフォルダーの作成を示すスクリーンショット](assets/program_create.png){zoomable="yes"}

プログラムを管理するには、プログラムの&#x200B;**[!UICONTROL フォルダー設定]**&#x200B;に移動します。

![プログラムのフォルダー設定を示すスクリーンショット](assets/program_settings.png){zoomable="yes"}

**[!UICONTROL カスタムオプション]**&#x200B;を定義し、プログラムのスケジュール日を設定します。

![プログラムのカスタムオプションを示すスクリーンショット](assets/program_options.png){zoomable="yes"}

**[!UICONTROL カスタムオプション]**&#x200B;を管理するには：

1. **[!UICONTROL スキーマ]**&#x200B;を参照します。
1. フィルターで&#x200B;**[!UICONTROL 編集可能]**&#x200B;なスキーマを選択します。
1. スキーマをクリックします。

![プログラムのカスタム詳細の編集を示すスクリーンショット](assets/program_edit.png){zoomable="yes"}

1. 「**[!UICONTROL 画面の編集]**」ボタンをクリックします。

   ![](assets/program_edit2.png){zoomable="yes"}

カスタムオプションを設定します。

![プログラムのカスタムフィールドの設定を示すスクリーンショット](assets/program_customfields.png){zoomable="yes"}

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