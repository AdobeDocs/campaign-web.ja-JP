---
title: カスタムフィールド
description: カスタムフィールドの設定方法を学ぶ
source-git-commit: 97769e885145d771685752f6367c5ea00831701d
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 8%

---

# カスタムフィールドの設定 {#custom-fields}

カスタムフィールドは、Adobe Campaign コンソールを通じて標準スキーマに追加される追加の属性です。 詳しくは、[Adobe Campaign v8 ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema.html?lang=ja){target="_blank"}を参照してください。

これらのカスタムフィールドは、プロファイルやテストプロファイルの詳細など、様々な画面に表示されます。

Web ユーザーインターフェイスでは、カスタムフィールドを作成することはできませんが、表示方法を変更できます。 変更は、すべての Campaign ユーザーに適用されます。

>[!NOTE]
>
>カスタムフィールドを変更するには、管理者権限が必要です。

カスタムフィールドは次のスキーマで使用できます。

* 受信者（nms）
* キャンペーン（nms）
* 配信（nms）
* シードアドレス（nms）

カスタムフィールドを設定するには、次の手順に従います。

1. 次の下 **管理**&#x200B;を選択し、 **スキーマ**.

   ![](assets/custom-fields.png){zoomable=&quot;yes&quot;}

1. 目的のスキーマを見つけます（例：）。 **受信者（nms）** スキーマ。

   ![](assets/custom-fields2.png){zoomable=&quot;yes&quot;}

1. 「」をクリックします **その他のアクション** ボタンと選択 **カスタム詳細を編集**.

   ![](assets/custom-fields3.png){zoomable=&quot;yes&quot;}

   この **カスタム詳細を編集** 画面には、すべてのカスタムフィールドとそのタイプが表示されます。

   ![](assets/custom-fields4.png){zoomable=&quot;yes&quot;}

   この画面では、次のアクションを実行できます。

   * 上下の矢印キーを使用して、異なるフィールドの順序を変更します。
   * フィールドを必須にする：をオンにします **必須** ボックス。
   * フィールドを表示または非表示にするには、 **表示可能** ボタン。
   * 表示条件を追加するには、 **次の場合に表示** ボタンをクリックし、使用可能な xtk 関数を使用して xtk 式を記述します。

1. カスタムフィールドを表示する画面に移動します。 この例では、これはプロファイルの詳細画面です。

   ![](assets/custom-fields5.png){zoomable=&quot;yes&quot;}
