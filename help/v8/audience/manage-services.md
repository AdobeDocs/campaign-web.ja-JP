---
audience: end-user
title: 購読サービスの操作
description: Adobe Campaign web で購読サービスにアクセス、購読サービスを作成および管理する方法について説明します
badge: label="限定提供（LA）"
exl-id: 95b2f2f9-5478-4fdb-9201-9c5bcb7f60b2
source-git-commit: d003de806a188b1b5c20a55ee1e308d5af1a19ea
workflow-type: tm+mt
source-wordcount: '951'
ht-degree: 90%

---

# 購読サービスの作成と管理 {#manage-services}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="サービスの作成と管理"
>abstract="Adobe Campaign を使用すると、ニュースレターなどのサービスの作成と監視を行ったり、これらのサービスの購読または購読解除を確認したりできます。購読はメールおよび SMS 配信にのみ当てはまります。"

Adobe Campaign Web を使用して、ニュースレターなどのサービスを管理および作成し、それらのサービスの購読または購読解除を確認します。

>[!NOTE]
>
>購読はメールおよび SMS 配信にのみ当てはまります。

複数のサービスを並行して定義できます。例えば、web サイトの特定の商品カテゴリ、テーマまたは分野に関するニュースレター、様々なタイプのアラートメッセージやリアルタイム通知の購読などです。

購読と購読解除の管理について詳しくは、[Campaign v8（クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/subscriptions.html?lang=ja){target="_blank"}を参照してください。

## 購読サービスへのアクセス {#access-services}

お使いのプラットフォームで利用可能な購読サービスにアクセスするには、次の手順に従います。

1. 左側のナビゲーションパネルの&#x200B;**[!UICONTROL 購読サービス]**&#x200B;メニューを参照します。

   ![](assets/service-list.png)

1. 既存のすべての購読サービスのリストが表示されます。サービスを検索してチャネルやフォルダーでフィルタリングすることも、[クエリモデラー](../query/query-modeler-overview.md)を使用してルールを追加することもできます。

   ![](assets/service-filters.png)

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

   ![](assets/service-create-button.png)

1. **[!UICONTROL E メール]**&#x200B;か **[!UICONTROL SMS]** のどちらかのチャネルを選択します。

1. サービスプロパティで、ラベルを入力し、必要に応じて&#x200B;**[!UICONTROL 追加オプション]**&#x200B;を定義します。

   ![](assets/service-create-properties.png)

1. デフォルトでは、サービスは&#x200B;**[!UICONTROL サービスと購読]**&#x200B;フォルダーに保存されます。目的の場所を参照して変更できます。[詳しくは、フォルダーの操作方法を参照してください](../get-started/permissions.md#folders)

1. デフォルトでは、購読は無制限です。「**[!UICONTROL 無制限の有効期間]**」オプションを無効にして、サービスの有効期間を定義できます。

   次の例では、20 日後には次のようになります。
   * このサービスを購読できる受信者はいなくなります。
   * このサービスのすべてのサブスクライバーは、20 日後に自動的に登録解除されます。[詳細情報](#automatic-unsubscription)

   ![](assets/service-create-validity-period.png)

1. ユーザーがサービスを登録または登録解除する際に、確認メッセージを送信できます。ユースケースに従って、そのメッセージに使用するテンプレートを選択します。これらのテンプレートは、**[!UICONTROL 購読]**&#x200B;ターゲットマッピングを使用して設定する必要があります。[詳細情報](#create-confirmation-message)

   ![](assets/service-create-confirmation-msg.png)

1. 「**[!UICONTROL 保存してレビュー]**」をクリックします。新しいサービスが&#x200B;**[!UICONTROL 購読サービス]**&#x200B;リストに追加されました。

次が可能になりました。

* このサービスにサブスクライバーを追加し、受信者を登録解除します。[詳細情報](../msg/send-to-subscribers.md)

* このサービスのサブスクライバーにメッセージを送信します。[詳細情報](../msg/send-to-subscribers.md)

## 確認メッセージの作成 {#create-confirmation-message}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_delivery_template"
>title="購読配信テンプレートを選択"
>abstract="サービスを購読するユーザーに確認メッセージを送信するには、 **[!UICONTROL 購読]** ターゲットマッピング（定義済みのターゲットなし）"


>[!CONTEXTUALHELP]
>id="acw_unsubscriptions_delivery_template"
>title="購読解除配信テンプレートを選択"
>abstract="サービスを購読解除したユーザーに確認メッセージを送信するには、 **[!UICONTROL 購読]** ターゲットマッピング（定義済みのターゲットなし）"

サービスを登録または登録解除するユーザーに確認メッセージを送信するには、**[!UICONTROL 購読]**&#x200B;ターゲットマッピング（定義済みのターゲットなし）を使用して配信テンプレートを作成する必要があります。それには、次の手順に従います。

1. 購読確認用の配信テンプレートを作成します。[詳しくは、テンプレートの作成方法を参照してください](../msg/delivery-template.md)

1. この配信のオーディエンスを選択しないでください。代わりに、配信&#x200B;**[!UICONTROL 設定]**&#x200B;にアクセスし、「[オーディエンス](../advanced-settings/delivery-settings.md#audience)」タブに移動して、**[!UICONTROL 購読]**&#x200B;ターゲットマッピングをリストから選択します。

   ![](assets/service-confirmation-template-mapping.png)

   >[!NOTE]
   >
   >**[!UICONTROL 購読]**&#x200B;ターゲットマッピングを選択しない場合、サブスクライバーには確認メッセージが届きません。ターゲットマッピングは、Campaign v8 コンソールで定義されます。詳しくは、[Adobe Campaign v8 ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=ja){target="_blank"}を参照してください。

1. 配信テンプレートのコンテンツを編集し、保存して閉じます。

   ![](assets/service-confirmation-template.png)

   >[!NOTE]
   >
   >配信チャネルおよび配信コンテンツの定義方法の詳細情報については、[メールチャネル](../email/create-email.md)および [SMS チャネル](../sms/create-sms.md)の節を参照してください。

1. 上記の手順を繰り返して、登録解除の確認用の配信テンプレートを作成します。

[サブスクリプションサービスの作成](#create-service)の際に、これらのメッセージを選択できるようになりました。そのサービスを購入または登録解除するユーザーには、選択した確認メッセージが表示されます。

## サブスクリプションサービスをモニター {#logs-and-reports}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_totalnumber_subscribers"
>title="サブスクライバーの合計数"
>abstract="「**計算**」をクリックして、このサービスのサブスクライバーの合計数を取得します。"

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

   ![](assets/service-logs-subscribers-count.png)

1. サービスダッシュボードで、「**[!UICONTROL ログ]**」を選択して、このサービスのサブスクライバーのリストを表示します。

   サブスクライバーの合計数、各受信者の名前およびアドレス、購読または登録解除のタイミングを確認できます。また、フィルタリングすることもできます。

   ![](assets/service-logs.png)

1. サービスダッシュボードで、「**[!UICONTROL レポート]**」を選択します。次の指標を確認します。

   * **[!UICONTROL サブスクライバーの合計数]**&#x200B;が表示されます。

   * 選択した期間の購入および登録解除の数を表示できます。ドロップダウンリストを使用して、時間範囲を変更します。

     ![](assets/service-reports.png)

   * **[!UICONTROL サブスクリプションの全体的な変化]**&#x200B;グラフは、購入、登録解除、数値の変化、ロイヤルティの割合を含む、期間別の分類を表示します。<!--what is Registered?-->

1. 「**[!UICONTROL リロード]**」ボタンを使用して、トラッキングワークフローの実行およびスケジュールから最後の値を取得します。
