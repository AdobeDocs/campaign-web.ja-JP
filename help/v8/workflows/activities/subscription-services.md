---
audience: end-user
title: 購読サービスアクティビティの使用
description: 購読サービスのワークフローアクティビティの使用方法について説明します
exl-id: 0e7c2e9a-3301-4988-ae0e-d901df5b84db
source-git-commit: e2579a65130ba580054cd23b1b525a46de2e752a
workflow-type: ht
source-wordcount: '598'
ht-degree: 100%

---

# 購読サービス {#subscriptipon-services}

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription"
>title="購読サービスアクティビティ"
>abstract="購読サービスアクティビティでは、複数のプロファイルのサービスへの購読登録とサービスからの購読登録解除を 1 つのアクションで実行できます。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_general"
>title="購読サービスの一般パラメーター"
>abstract="目的のサービスを選択し、実行するアクション（購読または購読解除）を選択します。「**確認メッセージを送信**」オプションをオンにすると、選択したサービスを購読または登録解除したことを母集団に通知できます。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_outboundtransition"
>title="アウトバウンドトランジションを生成"
>abstract="「**アウトバウンドトランジションを生成**」オプションを切り替えて、アクティビティの後にトランジションを追加します。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_additionalinfo"
>title="追加情報"
>abstract="追加情報"

**購読サービス**&#x200B;アクティビティは、**データ管理**&#x200B;アクティビティです。このアクティビティでは、トランジションで指定された母集団の情報サービスを購読または購読解除できます。

## 購読サービスアクティビティの設定 {#subscription-services-configuration}

**購読サービス**&#x200B;アクティビティを設定するには、次の手順に従います。

1. **購読サービス**&#x200B;アクティビティをワークフローに追加します。このアクティビティは、プロファイルをターゲティングした後、または識別されたデータを含むファイルを読み込んだ後に使用できます。

1. 次のいずれかのオプションを使用して、サブスクリプション管理の対象にするサービスを選択します。

   * **[!UICONTROL 特定のサービスを選択]**：「**[!UICONTROL サービス]**」フィールドを使用してサービスを手動で選択します。

   * **[!UICONTROL インバウンドトランジションから]**：インバウンドトランジションで指定されたサービスを使用します。例えば、管理対象のサービスを 1 行ごとに指定したファイルを読み込むことができます。この場合、操作の対象になるサービスが、プロファイルごとに動的に選択されます。

   ![](../assets/workflow-subscription-service.png)

1. 実行する操作を選択：「**登録**」または「**登録解除**」を選択します。

   インバウンドトランジションでサービスが定義されている場合は、この操作を取得する方法を選択できます。

   * **特定の操作タイプを選択**：実行する操作を手動で選択します（「**購読**」または「**登録解除**」）

   * **インバウンドトランジションのパスから操作タイプを選択**：各レコードに対して実行する操作を指定するインバウンドデータの列を選択します。例えば、「操作」列の行ごとに実行する操作を指定したファイルを読み込むことができます。

     >[!NOTE]
     >
     >ここで選択できるのは、ブール値フィールドまたは整数フィールドのみです。実行する操作を含むデータが、この形式と一致することを確認します。例えば、ファイルを読み込みアクティビティからデータを読み込む場合は、**[!UICONTROL ファイルを読み込み]**&#x200B;アクティビティで操作を含む列の形式が正しく設定されていることを確認します。例について詳しくは、[この節](#uc2)を参照ください。

   ![](../assets/workflow-subscription-service-inbound.png)

1. 選択したサービスを購読または登録解除したことを受信者に通知するには、「**[!UICONTROL 確認メッセージを送信]**」オプションをオンにします。このメッセージのコンテンツは、情報サービスに関連付けられた配信テンプレートで定義されます。

1. インバウンドトランジションのデータを使用する場合は「**[!UICONTROL 追加情報]**」セクションが表示され、各レコードの購読のデータと接触チャネルを指定できます。このセクションは空のままにすることができます。その場合、ワークフローの実行時に日付や接触チャネルは設定されません。

   * インバウンドデータに、サービスに対するプロファイルの購読日を示す列が含まれている場合は、「**[!UICONTROL 日付]**」フィールドで購読日を選択できます。

   * 「**[!UICONTROL 接触チャネルパス]**」フィールドで、購読の接触チャネルを定義します。インバウンドデータのフィールドの 1 つに設定するか、「**[!UICONTROL 接触チャネルとして定数を設定]**」オプションをオンにして任意の定数値に設定できます。

   ![](../assets/workflow-subscription-service-additional.png)

1. アクティビティの後にアウトバウンドトランジションを追加するには、「**[!UICONTROL アウトバウンドトランジションを生成]**」オプションをオンにします。

## 例 {#example}

### 特定のサービスへのオーディエンスの購読登録 {#uc1}

以下のワークフローは、オーディエンスを既存のサービスに購読登録する方法を示します。

![](../assets/workflow-subscription-service-uc1.png)

* **[!UICONTROL オーディエンスを作成]**&#x200B;アクティビティでは、既存のオーディエンスを対象にします。

* **[!UICONTROL 購読サービス]**&#x200B;アクティビティでは、プロファイルを購読登録する必要があるサービスを選択できます。

<!--
### Updating multiple subscription statuses from a file {#uc2}

The workflow below shows how to import a file containing profiles and update their subscription to several services specified in the file.

![](../assets/workflow-subscription-service-uc2.png)

* A **[!UICONTROL Load file]** activity loads a CSV file containing the data and defines the structure of the imported columns. The "service" and "operation" columns specify the service to update and the operation to perform (subscription or unsubscription).

  ```
  Lastname,firstname,city,birthdate,email,service,operation
  Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,yoga,sub
  Mars,Daniel,London,17/11/1999,danny.mars@example.com,running,sub
  Smith,Clara,Roma,08/02/1979,clara.smith@example.com,running,unsub
  Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,yoga,sub
  Durance,Alison,San Francisco,15/12/2000,allison.durance@example.com,running,unsub
  ```

  As you may have noticed, the operation is specified in the file as "sub" or "unsub". The system expects a **Boolean** or **Integer** value to recognize the operation to perform: "0" to unsubscribe and "1" to subscribe. To match this requirement, a remapping of values must be performed in the detail of the "operation" column in the sample file configuration screen.

  ![](../assets/workflow-subscription-service-uc2-mapping.png)

  If your file already uses "0" and "1" to identify the operation, you don't need to remap those values. Only make sure that the column is processed as a **Boolean** or **Integer** in the sample file columns.

* A **[!UICONTROL Reconciliation]** activity identifies the data from the file as belonging to the profile dimension of the Adobe Campaign database. The **email** field of the file is matched to the **email** field of the profile resource.

  ![](../assets/workflow-subscription-service-uc2-enrichment.png)

* An **[!UICONTROL Enrichment]** activity creates a link to the "Services (nms)" table and creates a simple join between the "service" column of the uploaded file, and the services "internal name" field in the database.

    ![](../assets/workflow-subscription-service-uc2-enrichment.png)

* A **[!UICONTROL Deduplication]** based on the **email** field identifies duplicates. It is important to eliminate duplicates since the subscription to a service will fail for all data in case of duplicates.

  ![](../assets/workflow-subscription-service-uc2-dedup.png)
  
* A **[!UICONTROL Subscription Services]** identifies the services to update as coming from the transition, through the link created in the **[!UICONTROL Reconciliation]** activity.

  The **[!UICONTROL Operation type]** is identified as coming from the **operation** field of the file. Only Boolean or Integer fields can be selected here. If the column of your file that contains the operation to perform does not appear in the list, make sure that you have correctly set your column format in the **[!UICONTROL Load file]** activity, as explained earlier in this example.

  ![](../assets/workflow-subscription-service-uc2-subscription.png)-->
