---
audience: end-user
title: 外部シグナル アクティビティの使用
description: 外部シグナル ワークフローアクティビティの使用方法を学ぶ
source-git-commit: 575219c7bcef303e211f504d13227183933924cc
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 5%

---

# 外部シグナル {#external-signal}

<!--External Signal End-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal"
>title="外部シグナル"
>abstract="この **外部シグナル** アクティビティを使用すると、別のワークフローまたは API 呼び出しからワークフローの実行をトリガーできます。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal_parameters"
>title="外部信号パラメーター"
>abstract="外部信号パラメーター"

>[!CONTEXTUALHELP]
>id="acw_orchestration_end_trigger"
>title="トリガーを終了"
>abstract="トリガーを終了"

この **外部シグナル** アクティビティはです **フロー制御** アクティビティ。 別のワークフローまたは API 呼び出しからワークフローの実行をトリガーできます。

>[!NOTE]
>
>ここでは、を設定するための主な手順を示します **[!UICONTROL 外部シグナル]** campaign web ユーザーインターフェイスのアクティビティと、別のワークフローまたは API 呼び出しからトリガーします。 ワークフローとそのベストプラクティスをトリガーする方法、および Campaign API を使用する方法について詳しくは、を参照してください。 [Campaign v8 （クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/advanced-management/javascript-in-workflows#trigger-example)

次の手順に従って、 **外部シグナル** アクティビティと、その実行をトリガーします。

1. を追加 **外部シグナル** ワークフローへのアクティビティ。

1. ワークフローの設定を完了し、実行を開始します。 この **[!UICONTROL 外部シグナル]** アクティビティは「保留中」と表示され、トリガーされるのを待っています。

   ![](../assets/external-signal-pending.png)

1. 以下の情報を取得します。

   * この **ワークフローの内部名**。ラベルの横に表示されます。

     +++例を表示

     ![](../assets/external-signal-workflow-name.png)

+++

   * この **外部シグナルアクティビティの名前**。ワークフローのに表示されます。 **[!UICONTROL 実行オプション]**.

     +++例を表示

     ![](../assets/external-signal-name.png)

+++

1. ワークフローをトリガーするには、 `PostEvent` JavaScript 関数 この関数を使用すると、選択した値で変数を渡し、それらをトリガーワークフローで活用できます。

   この `PostEvent` 関数は、別のワークフローまたは API 呼び出しから実行できます。

   * をトリガーにするには **[!UICONTROL 外部シグナル]** ワークフローからのアクティビティで、から PostEvent 関数を実行する **[!UICONTROL 初期化スクリプト]** アクティビティのからアクセスできるパネル **[!UICONTROL 実行オプション]**. の場合 **[!UICONTROL JavaScript コード]** アクティビティの場合は、アクティビティのスクリプトから関数を実行します。

     構文は以下のようになります。

     ```
     xtk.workflow.PostEvent("<workflow-internal-name>","<signal-activity-name>","",<variables <variable-name>="<value>"/>, false);
     ```

   +++例を表示

   この例では、内部名が「WKF12345」のワークフローに追加された「signal1」外部シグナルアクティビティをトリガーしています。 また、「customID」という名前の変数を、値「123456」とともに渡します。

   ![](../assets/external-signal-sample.png)

+++

   * をトリガーにするには **[!UICONTROL 外部シグナル]** api 呼び出しからのアクティビティについては、Campaign API ドキュメントで説明されている手順に従ってください。 [静的なの使用方法を学ぶ `PostEvent` メソッド](https://experienceleague.adobe.com/developer/campaign-api/api/sm-workflow-PostEvent.html?lang=ja)
