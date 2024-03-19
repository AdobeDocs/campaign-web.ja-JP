---
audience: end-user
title: データソースを変更ワークフローアクティビティの使用
description: データソースを変更ワークフローアクティビティの使用方法を説明します
source-git-commit: 980c19561c9f82a22a59b626d95d72981781af54
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 11%

---

# データソースを変更 {#change-data-source}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="ワークフローでのデータソースの変更"
>abstract="「データソースのターゲティングを変更」アクティビティを使用すると、ワークフローの作業用テーブルで使用されるデータソースを変更できます。 このアクティビティでは、様々なデータベース間でデータを管理し、パフォーマンスを向上させることで、より柔軟にデータを管理できます。"
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/release-notes/release-notes" text="リリースノートを参照してください"

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_data_source"
>title="データソースを変更"
>abstract="The **データソースを変更** 「 」アクティビティを使用すると、ワークフローの作業用テーブルに別のデータソースを選択できます。"

The **データソースを変更** アクティビティは **ターゲティング** アクティビティ。 このアクティビティを使用すると、ワークフローの作業用テーブルで使用されるデータソースを変更できます。 これにより、様々なデータベースをまたいでデータを管理し、パフォーマンスを向上させることで、より柔軟性を実現します。

ワークフローでは、トランジションを通じて 1 つのアクティビティから別のアクティビティに転送されたデータは、一時的な **作業用テーブル**. デフォルトでは、作業用テーブルは、処理されたデータのソースと同じデータベースに作成されます。 例えば、Cloud データベースに格納されている「Profiles」テーブルに対してクエリを実行する場合、同じ Cloud データベースに作業用テーブルが作成されます。

場合によっては、データが現在のデータベースで使用できないか、単一操作を実行するのに十分な効率がないことがあります。 したがって、ワークフローに別のデータベースを使用してこのような操作を実行させる必要がある場合は、 **[!UICONTROL データソースを変更]** アクティビティ。

Campaign のアーキテクチャについて詳しくは、 [Campaign v8（クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/architecture/architecture.html)

<!--

Let's say you want to send to your  VIP customers a unique offer code that they can redeem on your online store. To do this, you need to:

1. Query VIP customers on the "Profiles" table located on the Cloud database,
1. Retrieve an offer code for each targeted profile through API calls,
1. Update each profile with the assigned offer code,
1. Send an email to the profiles with their offer code.

In this situation, it is recommended to execute the offer code assignment operation on the local database, which is better suited for unitary operations. To do this, you need to add a **[!UICONTROL Change data source]** activity before the operation in order to execute it on the Campaign local database.

Before executing the operation, the working table is copied to the local database so that the operation can run there. Once done, the system detects that the profiles that we want to update are on another location. The data is therefore automatically copied back to the Cloud database where the "Profiles" table is located.
-->

## データソースを変更アクティビティを設定する {#configure}

**ディメンションを変更**&#x200B;アクティビティを設定するには、次の手順に従います。

![](../assets/workflow-change-data-source-add.png)

1. を追加します。 **データソースを変更** アクティビティをワークフローに追加します。

1. 作業用テーブルの移動先となるデータソースを定義します。

   * **[!UICONTROL デフォルトの Campaign データベース (PostgreSQL)]**：デフォルトの Campaign ローカルデータベースを使用します。
   * **[!UICONTROL FDA 外部アカウント]**: Federated Data Access 機能を使用して、Adobe Campaignに接続された外部 Cloud データベースを使用します。

     >[!AVAILABILITY]
     >
     >Campaign の設定と外部システムへの接続は、上級ユーザーに制限され、クライアントコンソールからのみ使用できます。[詳細情報](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html?lang=ja){target="_blank"}

1. 新しいデータソースを使用して目的の操作を実行するようにワークフローを設定します。

<!--
## Example {#example}

The workflow belows illustrates the use case detailed earlier, i.e. sending VIP customers offer codes that they can redeem on our online store.

-->
