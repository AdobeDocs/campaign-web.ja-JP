---
audience: end-user
title: 購読サービスの操作
description: Adobe Campaign Web で購読サービスにアクセス、購読サービスを作成および管理する方法について説明します
exl-id: 95b2f2f9-5478-4fdb-9201-9c5bcb7f60b2
source-git-commit: 12492f1c2464a18a420e6f4dccb62debf0bb3151
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 97%

---

# 購読サービスの作成と管理 {#manage-services}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="サービスの作成と管理"
>abstract="Adobe Campaign を使用すると、ニュースレターなどのサービスの作成と監視を行ったり、これらのサービスの購読または購読解除を確認したりできます。購読はメールおよび SMS 配信のみが対象となります。"

Adobe Campaign Web を使用すると、ニュースレターなどのサービスの管理と作成を行ったり、それらのサービスの購読または登録解除を確認したりできます。

複数のサービスを並行して定義できます。例えば、web サイトの特定の商品カテゴリ、テーマまたは分野に関するニュースレター、様々なタイプのアラートメッセージやリアルタイム通知の購読などです。

>[!NOTE]
>
>購読はメールおよび SMS 配信のみが対象となります。

## 購読サービスへのアクセス {#access-services}

お使いのプラットフォームで利用可能な購読サービスにアクセスするには、次の手順に従います。

1. 左側のナビゲーションパネルの&#x200B;**[!UICONTROL 購読サービス]**&#x200B;メニューを参照します。

   ![](assets/service-list.png){zoomable=&quot;yes&quot;}

1. 既存の全購読サービスのリストが表示されます。サービスを検索してチャネルやフォルダーでフィルタリングすることも、[クエリモデラー](../query/query-modeler-overview.md)を使用してルールを追加することもできます。

   ![](assets/service-filters.png){zoomable=&quot;yes&quot;}

1. 既存のサービスを編集するには、サービス名をクリックします。

1. サービス名の横にある 3 つのドットのアイコンを使用して、サービスを削除したり複製したりできます。<!--so all subscribers are unsubscribed - need to mention?-->

## 最初の購読サービスの作成 {#create-service}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_properties"
>title="サービスプロパティの定義"
>abstract="購読サービスのラベルを入力し、サービスの有効期間などの追加オプションを定義します。"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_confirm"
>title="確認メッセージの選択"
>abstract="ユーザーがサービスを登録または登録解除する際に、確認メッセージを送信できます。そのメッセージに使用するテンプレートを選択します。"

購読サービスを作成するには、次の手順に従います。

1. 「**[!UICONTROL 購読サービスを作成]**」ボタンをクリックします。

   ![](assets/service-create-button.png){zoomable=&quot;yes&quot;}

1. **[!UICONTROL E メール]**&#x200B;か **[!UICONTROL SMS]** のどちらかのチャネルを選択します。

1. サービスプロパティで、ラベルを入力し、必要に応じて&#x200B;**[!UICONTROL 追加オプション]**&#x200B;を定義します。

   ![](assets/service-create-properties.png){zoomable=&quot;yes&quot;}

1. デフォルトでは、サービスは&#x200B;**[!UICONTROL サービスと購読]**&#x200B;フォルダーに保存されます。目的の場所を参照して変更できます。[詳しくは、フォルダーの操作方法を参照してください](../get-started/permissions.md#folders)

1. デフォルトでは、購読は無制限です。

   「**[!UICONTROL 無制限の有効期間]**」オプションを無効にして、サービスの有効期間を定義できます。有効期間が終了した場合：
   * このサービスを購読できる受信者はいません
   * このサービスのすべての購読者は、自動的に登録解除されます

   ![](assets/service-create-validity-period.png){zoomable=&quot;yes&quot;}

1. ユーザーがサービスを登録または登録解除する際に、確認メッセージを送信できます。ユースケースに従って、そのメッセージに使用するテンプレートを選択します。これらのテンプレートは、**[!UICONTROL 購読]**&#x200B;ターゲットマッピングを使用して設定する必要があります。[詳細情報](#create-confirmation-message)

   ![](assets/service-create-confirmation-msg.png){zoomable=&quot;yes&quot;}

1. 「**[!UICONTROL 保存してレビュー]**」をクリックします。新しいサービスが&#x200B;**[!UICONTROL 購読サービス]**&#x200B;リストに追加されました。

次が可能になりました。

* このサービスにサブスクライバーを追加し、受信者を登録解除します。[詳細情報](../msg/send-to-subscribers.md)

* このサービスのサブスクライバーにメッセージを送信します。[詳細情報](../msg/send-to-subscribers.md)

## 確認メッセージの作成 {#create-confirmation-message}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_delivery_template"
>title="購読の配信テンプレートの選択"
>abstract="サービスを購読するユーザーに確認メッセージを送信するには、**[!UICONTROL 購読]**&#x200B;ターゲットマッピング（定義済みのターゲットなし）に基づいて特定の配信テンプレートを選択する必要があります。"


>[!CONTEXTUALHELP]
>id="acw_unsubscriptions_delivery_template"
>title="登録解除の配信テンプレートの選択"
>abstract="サービスを登録解除るユーザーに確認メッセージを送信するには、**[!UICONTROL 購読]**&#x200B;ターゲットマッピング（定義済みのターゲットなし）に基づいて特定の配信テンプレートを選択する必要があります。"

サービスを登録または登録解除するユーザーに確認メッセージを送信するには、**[!UICONTROL 購読]**&#x200B;ターゲットマッピング（定義済みのターゲットなし）を使用して配信テンプレートを作成する必要があります。これをおこなうには、以下の手順に従います。

1. 購読確認用の配信テンプレートを作成します。[詳しくは、テンプレートの作成方法を参照してください](../msg/delivery-template.md)

1. この配信のオーディエンスを選択しないでください。代わりに、配信&#x200B;**[!UICONTROL 設定]**&#x200B;にアクセスし、「[オーディエンス](../advanced-settings/delivery-settings.md#audience)」タブに移動して、**[!UICONTROL 購読]**&#x200B;ターゲットマッピングをリストから選択します。

   ![](assets/service-confirmation-template-mapping.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >**[!UICONTROL 購読]**&#x200B;ターゲットマッピングを選択しない場合、サブスクライバーには確認メッセージが届きません。ターゲットマッピングについて詳しくは、[この節](../audience/targeting-dimensions.md)を参照してください。

1. 配信テンプレートのコンテンツを編集し、保存して閉じます。

   ![](assets/service-confirmation-template.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >配信チャネルおよび配信コンテンツの定義方法の詳細情報については、[メールチャネル](../email/create-email.md)および [SMS チャネル](../sms/create-sms.md)の節を参照してください。

1. 上記の手順を繰り返して、登録解除の確認用の配信テンプレートを作成します。

[サブスクリプションサービスの作成](#create-service)の際に、これらのメッセージを選択できるようになりました。そのサービスを購入または登録解除するユーザーには、選択した確認メッセージが表示されます。

## サブスクリプションサービスをモニター {#logs-and-reports}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_totalnumber_subscribers"
>title="サブスクライバー数"
>abstract="「**計算**」をクリックして、このサービスのサブスクライバーの合計数を取得します。"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_totalnumber_subscribers_report"
>title="サブスクライバーの合計数"
>abstract="主要業績評価指標 (KPI) は、購読者のベースを包括的に表示し、このサービスを購読した個人の総数を示します。"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_overtheperiod_subscribers"
>title="期間中の購読数"
>abstract="ドロップダウンリストを使用して時間範囲を変更し、選択した期間の購読および登録解除の数を表示します。"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_overallevolution_subscribers"
>title="購読の全体的な変化"
>abstract="このグラフは、購読、登録解除、数値の変化、ロイヤルティの割合を含む、期間別の分類を表示します。"

SMS チャンネルおよびメールチャネルに関するサブスクリプションサービスの効果を測定するには、特定のサービスのログとレポートにアクセスします。

1. **[!UICONTROL サブスクリプションサービス]**&#x200B;リストから既存のサービスを選択します。「**[!UICONTROL 計算]**」をクリックして、サブスクライバーの合計数を取得します。

   ![](assets/service-logs-subscribers-count.png){zoomable=&quot;yes&quot;}

1. サービスダッシュボードで、「**[!UICONTROL ログ]**」を選択して、このサービスのサブスクライバーのリストを表示します。

   サブスクライバーの合計数、各受信者の名前およびアドレス、購読または登録解除のタイミングを確認できます。また、フィルタリングすることもできます。

   ![](assets/service-logs.png){zoomable=&quot;yes&quot;}

1. サービスダッシュボードで、「**[!UICONTROL レポート]**」を選択します。次の指標を確認します。

   * **[!UICONTROL サブスクライバーの合計数]**&#x200B;が表示されます。

   * 選択した期間の購入および登録解除の数を表示できます。ドロップダウンリストを使用して、時間範囲を変更します。

     ![](assets/service-reports.png){zoomable=&quot;yes&quot;}

   * **[!UICONTROL サブスクリプションの全体的な変化]**&#x200B;グラフは、購入、登録解除、数値の変化、ロイヤルティの割合を含む、期間別の分類を表示します。<!--what is Registered?-->

1. 「**[!UICONTROL リロード]**」ボタンを使用して、トラッキングワークフローの実行およびスケジュールから最後の値を取得します。
