---
audience: end-user
title: 購読サービスアクティビティの使用
description: 購読サービスワークフローアクティビティの使用方法を学ぶ
exl-id: 0e7c2e9a-3301-4988-ae0e-d901df5b84db
source-git-commit: 362f657c689ce13c6c1fadc381d43e15c32d4d05
workflow-type: tm+mt
source-wordcount: '992'
ht-degree: 13%

---

# 購読サービス {#subscriptipon-services}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="購読サービスアクティビティ"
>abstract="新しい購読サービスワークフローアクティビティを使用して、サービスの購読を管理します。 母集団を購読または購読解除でき、外部ファイルから複数の購読を更新することもできます。 オプションとして、確認メッセージを送信して購読者に通知することもできます。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=ja" text="詳しくは、リリースノートを参照してください。"


>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription"
>title="購読サービスアクティビティ"
>abstract="購読サービス アクティビティを使用すると、1 回のアクションで複数のプロファイルのサービスへの購読やサービスの購読解除を行えます。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_general"
>title="購読サービスの一般パラメーター"
>abstract="目的のサービスを選択し、実行するアクション（購読または購読解除）を選択します。 をオンにします **確認メッセージを送信** オプションをオンにすると、選択したサービスを購読または購読解除したことを母集団に通知できます。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_outboundtransition"
>title="アウトバウンドトランジションを生成"
>abstract="「**アウトバウンドトランジションを生成**」オプションを切り替えて、アクティビティの後にトランジションを追加します。"

この **購読サービス** アクティビティはです **データ管理** アクティビティ。 これにより、トランジションで指定された母集団の情報サービスに対する購読を作成または削除できます。

## 購読サービスアクティビティの設定 {#subscription-services-configuration}

次の手順に従って、 **購読サービス** アクティビティ：

1. を追加 **購読サービス** ワークフローへのアクティビティ。 このアクティビティは、プロファイルをターゲット設定した後や、識別されたデータを含むファイルをインポートした後に使用できます。

1. 次のいずれかのオプションを使用して、購読を管理するサービスを選択します。

   * **[!UICONTROL 特定のサービスを選択]**：を使用してサービスを手動で選択 **[!UICONTROL サービス]** フィールド。

   * **[!UICONTROL インバウンドトランジションから]**：インバウンドトランジションで指定されたサービスを使用します。 例えば、管理対象のサービスを 1 行ごとに指定したファイルをインポートできます。その後、操作を実行するサービスが、プロファイルごとに動的に選択されます。

   ![](../assets/workflow-subscription-service.png)

1. 実行する操作を選択します。 **登録** または **購読解除**.

   インバウンドトランジションでサービスが定義されている場合は、この操作を取得する方法を選択できます。

   * **特定の操作タイプを選択**：実行する操作を手動で選択します（**登録** または **購読解除**）

   * **インバウンドトランジションのパスから操作タイプを選択**：各レコードに対して実行する操作を指定するインバウンドデータの列を選択します。 例えば、「operation」列の各行に対して実行する操作を指定するファイルを読み込むことができます。

     >[!NOTE]
     >
     >ここで選択できるのは、ブールまたは整数のフィールドのみです。 実行する操作を含むデータが、この形式と一致することを確認します。 例えば、ファイルを読み込みアクティビティからデータを読み込む場合、で操作を含む列の形式が正しく設定されていることを確認してください。 **[!UICONTROL ファイルをロード]** アクティビティ。 例については、こちらを参照してください。 [この節](#uc2).

   ![](../assets/workflow-subscription-service-inbound.png)

1. 選択したサービスを購読または購読解除したことを受信者に通知するには、 **[!UICONTROL 確認メッセージの送信]** オプションをオンにします。 この通知のコンテンツは、情報サービスに関連付けられた配信テンプレートで定義されます。

1. インバウンドトランジションのデータを使用する場合、 **[!UICONTROL 追加情報]** セクションが表示され、各レコードの購読のデータと起源を指定できます。 このセクションは空のままにすることができます。この場合、ワークフローの実行時に日付や接触チャネルは設定されません。

   * インバウンドデータに、サービスに対するプロファイルの購読日を示す列が含まれている場合は、 **[!UICONTROL 日付]** フィールド。

   * が含まれる **[!UICONTROL 接触チャネルパス]** フィールドで、サブスクリプションのオリジンを定義します。 をチェックすることで、受信データのいずれかのフィールドに設定するか、選択した定数値に設定できます。 **[!UICONTROL 定数を原点として設定]** オプション。

   ![](../assets/workflow-subscription-service-additional.png)

1. アクティビティの後にアウトバウンドトランジションを追加するには、 **[!UICONTROL アウトバウンドトランジションを生成]** オプションをオンにします。

## 例 {#example}

### 特定のサービスへのオーディエンスの購読 {#uc1}

以下のワークフローは、オーディエンスを既存のサービスに登録する方法を示しています。

![](../assets/workflow-subscription-service-uc1.png)

* A **[!UICONTROL オーディエンスを作成]** アクティビティは、既存のオーディエンスをターゲットにします。

* A **[!UICONTROL 購読サービス]** アクティビティでは、プロファイルを購読する必要があるサービスを選択できます。

### ファイルからの複数の購読ステータスの更新 {#uc2}

次のワークフローは、プロファイルを含むファイルをインポートし、ファイルで指定された複数のサービスに対するプロファイルの購読を更新する方法を示しています。

![](../assets/workflow-subscription-service-uc2.png)

* A **[!UICONTROL ファイルをロード]** アクティビティは、データを含む CSV ファイルを読み込み、読み込んだ列の構造を定義します。 「サービス」列と「操作」列では、更新するサービスと実行する操作（購読または購読解除）を指定します。

  ```
  Lastname,firstname,city,birthdate,email,service,operation
  Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,yoga,sub
  Mars,Daniel,London,17/11/1999,danny.mars@example.com,running,sub
  Smith,Clara,Roma,08/02/1979,clara.smith@example.com,running,unsub
  Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,yoga,sub
  Durance,Alison,San Francisco,15/12/2000,allison.durance@example.com,running,unsub
  ```

  この操作は、ファイル内で「sub」または「unsub」と指定されています。実行する操作を認識するために、**ブール値**&#x200B;または&#x200B;**整数**&#x200B;値が必要です。「0」が購読登録解除、「1」が購読登録です。この要件に一致させるには、サンプルファイル設定画面の「operation」列の詳細で値の再マッピングを実行する必要があります。

  ![](../assets/workflow-subscription-service-uc2-mapping.png)

  「0」と「1」が既に操作の識別に使用されているファイルでは、再マッピングの必要はありません。列がとして処理されていることを確認するだけです **ブール値** または **整数** サンプルファイル列

* A **[!UICONTROL 紐付け]** アクティビティは、ファイルのデータをAdobe Campaign データベースのプロファイルディメンションに属すると識別します。 この **電子メール** ファイルのフィールドは、 **電子メール** プロファイルリソースのフィールド。

  ![](../assets/workflow-subscription-service-uc2-enrichment.png)

* An **[!UICONTROL エンリッチメント]** アクティビティは、「サービス（nms）」テーブルへのリンクを作成し、アップロードされたファイルの「サービス」列とデータベースの「サービスの内部名」フィールドの間に単純な結合を作成します。

  ![](../assets/workflow-subscription-service-uc2-enrichment.png)

* A **[!UICONTROL 重複排除]** に基づく **電子メール** フィールドは重複を識別します。 重複がある場合、サービスへの購読登録はすべてのデータで失敗するので、重複を排除することが重要です。

  ![](../assets/workflow-subscription-service-uc2-dedup.png)

* A **[!UICONTROL 購読サービス]** は、で作成されたリンクを介して、トランジションから派生したものとして更新するサービスを識別します。 **[!UICONTROL 紐付け]** アクティビティ。

  この **[!UICONTROL 操作タイプ]** は、から来たものと識別されます **操作** ファイルのフィールド。 ここで選択できるのは、ブール値フィールドまたは整数フィールドのみです。実行する操作を含むファイルの列がリストに表示されない場合は、列の形式を正しく設定していることを確認してください **[!UICONTROL ファイルをロード]** アクティビティ（この例で前述）。

  ![](../assets/workflow-subscription-service-uc2-subscription.png)