---
title: 列挙の管理
description: 列挙の操作方法を学ぶ
exl-id: d2a30fef-2cc4-49af-9f5d-d42c6396a8ab
source-git-commit: 8fccae9906d7a04ec1e8e10ad7be60f597a43492
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 19%

---

# 列挙の管理 {#enumerations}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn3"
>title="列挙の作成"
>abstract="Adobe Campaign web ユーザーインターフェイスから列挙を直接作成できるようになりました。 列挙は、フィールドへの入力をシステムが推奨する値のリストです。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=ja" text="リリースノートを参照してください"


>[!CONTEXTUALHELP]
>id="acw_enumerations_list"
>title="列挙"
>abstract="列挙とは、フィールドへの入力候補としてシステムによって表示される値のリストです。列挙を利用することでフィールドの値を統一することができ、データ入力時やクエリでの利用に便利です。"

>[!CONTEXTUALHELP]
>id="acw_enumerations_properties"
>title="プロパティ"
>abstract="名前、内部名、タイプなどの列挙のプロパティを定義します。 **[!UICONTROL クローズド]** 列挙には、**[!UICONTROL 列挙]** メニューからのみ変更できる値の固定リストがあります。 **[!UICONTROL 開く]** 列挙を使用すると、ユーザーはこの列挙に基づいてフィールドに新しい値を直接追加できます。 **[!UICONTROL システム]** 列挙は、システムフィールドに関連付けられています。 **[!UICONTROL 顔文字]** 列挙を使用して、顔文字リストを更新します。"

>[!CONTEXTUALHELP]
>id="acw_enumerations_values"
>title="定義済みリストの値のリスト"
>abstract="列挙に値を追加するには、「**[!UICONTROL 値を追加]**」ボタンをクリックして、必要に応じて設定します。"

## 列挙とは {#about}

列挙とは、フィールドへの入力候補としてシステムによって表示される値のリストです。列挙を使用してこれらのフィールドの値を標準化し、データ入力やクエリ内での使用に役立てます。 値のリストはドロップダウンリストとして表示され、値を選択すると、その値がフィールドに入力されます。また、このドロップダウンリストには予測入力機能があり、最初の数文字を入力すると続きが自動的に補完されます。

このタイプのフィールドの値は、左側のナビゲーションペインの **[!UICONTROL 管理]**/**[!UICONTROL 列挙]** メニューを使用して定義します。

![](assets/enumeration-list.png)

## 列挙の作成 {#create}

列挙を作成するには、次の手順に従います。

1. **[!UICONTROL 列挙]** メニューに移動し、「**[!UICONTROL 列挙を作成]** ボタンをクリックします。

1. 列挙の **[!UICONTROL ラベル]** と **[!UICONTROL 内部名]** を入力します。

   ![](assets/enumeration-create.png)

1. 列挙 **[!UICONTROL タイプ]** を選択します。

   * **[!UICONTROL クローズド]** 列挙には、**[!UICONTROL 列挙]** メニューからのみ変更できる値の固定リストがあります。
   * **[!UICONTROL 開く]** 列挙を使用すると、ユーザーはこの列挙に基づいてフィールドに新しい値を直接追加できます。
   * **[!UICONTROL システム]** 列挙は、システムフィールドに関連付けられています。
   * **[!UICONTROL 顔文字]** 列挙を使用して、顔文字リストを更新します。

1. 「**[!UICONTROL 作成]**」をクリックします。列挙の詳細が表示され、リストに値を追加できます。

   ![](assets/enumeration-details.png)

1. 値を追加するには、「**[!UICONTROL 値を追加]**」ボタンをクリックし、必要に応じて設定します。

   * **[!UICONTROL ラベル]**：定義済みリストに表示されるラベル。
   * **[!UICONTROL 内部名]**：値の内部名（システム列挙の場合）。
   * **[!UICONTROL U+（内部名）]** （顔文字の定義済みリスト）：顔文字の Unicode コード（顔文字の定義済みリスト用）。

   ![](assets/enumeration-emoticon.png)

1. 変更内容を保存します。定義済みリストが使用されている画面で更新されるようになりました。

## ユースケース：定義済み値を列挙に追加する {#uc}

デフォルトでは、プロファイルの詳細画面の「接触チャネル」フィールドを使用すると、ユーザーは任意の値を自由に入力できます。

![](assets/enumeration-uc-profile.png)

ユーザーがフィールドに値を入力するたびに、その値が「接触チャネル」列挙に自動的に追加され、値リストに時間の経過と共に冗長な値、一貫性のない値、エラーが発生する可能性があります。

![](assets/enumeration-uc-choice.png)

データの一貫性を確保し、フィールド入力時にユーザーをガイドするために、事前定義済みの値のセットを定義できます。 次の手順に従います。

1. **[!UICONTROL 列挙]** メニューに移動し、「接触チャネル」列挙を開きます。

2. ユーザーが入力した値のリストを確認し、クリーンアップします。 値の横にある「。..」ボタンをクリックすると、値を削除できます。 リストに含まれる不一致が多すぎる場合は、列挙全体を削除して、最初から再作成します。

   ![](assets/enumeration-uc-clean.png)

3. 事前定義済みの値を追加します。 これを行うには、「**[!UICONTROL 値を追加]**」ボタンをクリックし、ユーザーが選択する事前定義済みの値を入力します。

   ![](assets/enumeration-uc-create.png)

4. 一貫性を確保するには、定義済みリストのタイプを **[!UICONTROL クローズド]** に切り替えて、ユーザーを事前定義済みの値に制限します。
柔軟性が必要な場合は、新しいユーザーエントリを許可するために **[!UICONTROL 開く]** のままにします。

5. プロファイルの詳細画面に戻ります。 「生成元」フィールドに、選択する事前定義済みの値が表示されるようになりました。

   ![](assets/enumeration-uc-populated.png)
