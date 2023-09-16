---
audience: end-user
title: 最初のメールを送信
description: Campaign web UI での最初のメールの送信方法を学ぶ
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
badge: label="Beta"
source-git-commit: 925f797b79ec1b42a613373f8af1931a8aff3319
workflow-type: tm+mt
source-wordcount: '1352'
ht-degree: 70%

---


# 最初のメールを送信 {#first-email}

>[!CONTEXTUALHELP]
>id="acw_homepage_card2"
>title="E メールコンテンツ用 Gen AI"
>abstract="当社の Gen AI テクノロジーは、高度なアルゴリズムを利用して、高度にエンゲージメントとパーソナライズされたコンテンツを生成します。 Gen AI のインテリジェントなコンテンツ生成により、開封率、クリックスルー率、コンバージョン率の向上を推進します。 競争に先立ち、Gen AI を使用したメールマーケティングゲームをメールコンテンツに活用してください。"

最初のターゲットメールを作成する方法について説明します。このユースケースでは、特定の日にシルバーおよびゴールドのロイヤルティメンバーにメールを送信するようにスケジュールします。

事前定義済みに基づく [デザインテンプレート](../content/email-templates.md)の場合、E メールには、顧客プロファイル属性に基づいてパーソナライズされたコンテンツも含まれます。

## メール配信の作成 {#create-email}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_template_selection"
>title="メールテンプレートの選択"
>abstract="メールテンプレートは、タイポロジルール、パーソナライゼーション、ルーティングパラメーターなど、事前定義された設定を含む特定の配信設定です。テンプレートは、Campaign クライアントコンソールで定義されます。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_properties"
>title="E メールプロパティを定義する"
>abstract="プロパティは、配信の名前付けや分類に役立つ一般的な配信パラメーターです。追加の設定はオプションです。 配信が Adobe Campaign v8 コンソールで定義された拡張スキーマに基づいている場合は、いくつかの特定の&#x200B;**カスタムオプション**&#x200B;フィールドを使用できます。"

スタンドアロンの E メール配信を作成することも、キャンペーンワークフローのコンテキストで E メールを作成することもできます。 以下の手順では、スタンドアロン（ワンショット）E メール配信の手順について説明します。 キャンペーンワークフローのコンテキストで作業している場合、作成手順の詳細は [この節](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

新しいスタンドアロンの E メール配信を作成するには、次の手順に従います。

1. 左側のナビゲーションの&#x200B;**[!UICONTROL 配信]**&#x200B;メニューを参照し、「**[!UICONTROL 配信を作成]**」ボタンをクリックします。

   ![](assets/delivery-list.png)

1. 「**[!UICONTROL メール]**」をチャネルとして選択し、リストからメール配信テンプレートを選択します。

   >[!NOTE]
   >
   >テンプレートは、後で使用するために保存された、事前設定済みの配信設定です。[詳細情報](../msg/delivery-template.md)

   ![](assets/channel-template.png)

1. 「**[!UICONTROL 配信を作成]**」ボタンをクリックして、確定します。
1. 配信のラベルを入力し、必要に応じて追加のオプションを設定します。

   * **[!UICONTROL 内部名]**：配信に一意の ID を割り当てます。
   * **[!UICONTROL フォルダー]**：配信を特定のフォルダーに保存します。
   * **[!UICONTROL 配信コード]**：このフィールドを使用して、独自の命名規則に基づいて配信を整理します。
   * **[!UICONTROL 説明]**：配信の説明を指定します。
   * **[!UICONTROL 特性]**：分類目的でメールの特性を指定します。<!--The content of the list is defined in the delivery template selected when creating the email.-->

   >[!NOTE]
   >
   >特定のカスタムフィールドを使用してスキーマを拡張した場合は、 「**[!UICONTROL カスタムオプション]**」セクションでそれらのフィールドにアクセスできます。

   ![](assets/email-properties.png)

1. また、タイポロジルールやターゲットマッピングなどの詳細設定には、 **[!UICONTROL 設定]** ボタンをクリックします。 これらの設定は、選択したテンプレートで事前に設定されていますが、この特定のメールの必要に応じて編集できます。

## オーディエンスを定義 {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="配信用のオーディエンスを選択"
>abstract="マーケティングメッセージに最適なオーディエンスを選択します。(Campaign v8 インスタンスまたはAdobe Experience Platformで既に定義されている ) 既存のオーディエンスを選択したり、ルールビルダーを使用して新しいオーディエンスを作成したり、オーディエンスを含むファイルをアップロードしたりできます。 コントロール母集団が **ファイルから選択** オプションとその逆。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/add-audience.html" text="メインオーディエンスを選択"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/control-group.html" text="コントロール母集団を設定"

このユースケースでは、既存のオーディエンスにメールを送信します。

オーディエンスの操作方法に関する追加手順については、[この節](../audience/about-audiences.md)を参照してください。

1. メールのオーディエンスを選択するには、「**[!UICONTROL オーディエンスを選択]**」ボタンをクリックし、リストから既存のオーディエンスを選択します。

   この例では、シルバーおよびゴールドのロイヤルティポイントレベルに属する顧客をターゲティングする既存のオーディエンスを使用します。

   ![](assets/create-audience.png)

   >[!NOTE]
   >
   >リストで使用可能なオーディエンスは、Campaign v8 インスタンスから、またはインスタンスに宛先/ソース統合が設定されている場合はAdobe Experience Platformから作成します。 この統合により、Experience PlatformセグメントをAdobe Campaignに送信したり、Campaign の配信とトラッキングログをAdobe Experience Platformに送信したりできます。 Campaign とAdobe Experience Platformの連携の仕組みについては、 [Campaign v8（クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

1. オーディエンスを選択したら、追加のルールを適用してターゲットを絞り込むことができます。

   ![](assets/audience-selected.png)

1. またコントロール母集団を設定して、ターゲットとならなかったユーザーと比較してメール受信者の行動を分析することもできます。[詳しくは、コントロール母集団の操作方法を参照してください](../audience/control-group.md)

## メールコンテンツの定義 {#create-content}

メールコンテンツの作成を開始するには、次の手順に従います。このユースケースでは、事前定義されたメール[配信テンプレート](../msg/delivery-template.md)を使用してメールをデザインします。<!--TBC delivery template or email content template?-->

<!--Detailed instructions on how to configure the email content are available in [this section](../content/edit-content.md).-->

1. メール配信ダッシュボードで、「**[!UICONTROL コンテンツを編集]**」ボタンをクリックします。

   ![](assets/email-edit-content.png)

   これにより、メールコンテンツを設定し、メールデザイナーをアクセスできる専用のインターフェイスが表示されます。[詳細情報](../content/edit-content.md)

   ![](assets/edit-content.png)

1. メールの件名を入力し、式エディターを使用してパーソナライズします。詳しくは、[コンテンツをパーソナライズする方法](../personalization/personalize.md)を参照してください。

   ![](assets/subject-line.png)

1. メールのコンテンツをデザインするには、「**[!UICONTROL メール本文を編集]**」ボタンをクリックします。

   メールコンテンツの作成に使用する方法を選択します。この例では、[事前定義済みのコンテンツテンプレートを使用します](../msg/delivery-template.md)。

   ![](assets/select-template.png)

1. テンプレートを選択すると、[メールデザイナー](../content/create-email-content.md)に表示され、必要な編集を加えたり、パーソナライゼーションを追加したりできます。

   例えば、パーソナライゼーションをメールタイトルに追加するには、コンポーネントブロックを選択し、「**[!UICONTROL パーソナライゼーションを追加]**」をクリックします。

   ![](assets/add-perso.png)

1. コンテンツの設定が完了したら、デザインを保存して閉じます。「**[!UICONTROL 保存]**」をクリックして、メール作成画面に戻ります。

   ![](assets/save-content.png)

## 送信のスケジュール設定 {#schedule}

E メールの送信をスケジュールするには、次の手順に従います。

配信の送信スケジュールの設定方法に関する追加の手順について詳しくは、 [この節](../msg/gs-messages.md#gs-schedule).

1. 次を参照： **[!UICONTROL スケジュール]** 」セクションに入力します。

1. 以下を使用します。 **[!UICONTROL スケジュールを有効にする]** オンに切り替えて有効にします。

1. 送信する日時を設定します。

   ![](assets/schedule.png)

配信を送信すると、実際の送信は、定義した連絡日に開始されます。

## メールのプレビューとテスト {#preview-test}

メールを送信する前に、プレビューおよびテストを行って、期待どおりに動作するかどうかを確認できます。

このユースケースでは、ターゲットプロファイルの一部を偽装して、メールをプレビューし、特定のメールアドレスにテストバージョンを送信します。

メールのプレビューおよびテスト方法に関する追加情報については、 [この節](../preview-test/preview-test.md)を参照してください。

1. メールを確認するには、「**[!UICONTROL 確認して送信]**」をクリックします。これによりメールのプレビューが、設定済みのすべてのプロパティ、オーディエンス、スケジュールと共に表示されます。「変更」ボタンをクリックして、これらの要素を編集できます。

1. メールをプレビューしてテストバージョンを送信するには、「**[!UICONTROL コンテンツをシミュレート]**」ボタンをクリックします。

   ![](assets/review-email.png)

1. 左側で、メールのプレビューに使用するプロファイルを選択します。

   右側のパネルに選択したプロファイルに基づくメールのプレビューが表示されます。 複数のプロファイルを追加した場合は、それぞれを切り替えて対応するメールをプレビューできます。

   ![](assets/preview.png)

   <!--Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using mutiple devices or mail providers. Learn on how to preview email rendering
    -->

1. テストバージョンのメールを送信するには、「**[!UICONTROL テスト]**」ボタンをクリックして、使用するモードを選択します。

   この例では、**[!UICONTROL メインターゲットから代入]**&#x200B;モードを使用して、メールのターゲットとなる一部のプロファイルを別のユーザーとして実行し、特定のメールアドレスにテストバージョンを送信します。

   ![](assets/proof-mode.png)

1. 「**[!UICONTROL アドレスを追加]**」をクリックして、テストバージョンを受け取るメールアドレスを指定します。

   メールアドレスごとに、別のユーザーとして実行するプロファイルを選択します。また、ターゲットからランダムなプロファイルを Adobe Campaign に選択させることもできます。

   ![](assets/proof-test-profile.png)

1. 「**[!UICONTROL テストメールを送信]**」をクリックし、送信を確認します。

   テスト版は、選択したプロファイルに **[Proof x]** という接頭辞を付けて使用し、指定したメールアドレスに送信されます。

   ![](assets/proof-sent.png)

   コンテンツをシミュレート画面の「**[!UICONTROL テストメールログを表示]**」ボタンをクリックすると、送信ステータスの確認や送信済みのテストメールにいつでもアクセスできます。

## メールの送信と監視 {#prepare-send}

メールを確認およびテストした後、準備を開始して送信できます。

1. メールの準備を開始するには、「**[!UICONTROL 準備]**」をクリックします。[詳しくは、メールの準備方法を参照してください](../monitor/prepare-send.md)

   ![](assets/preparation.png)

1. メールを送信する準備が整ったら、「**[!UICONTROL 送信]**」ボタン（送信をスケジュールしている場合は「**[!UICONTROL スケジュールどおりに送信]**」）をクリックして、送信を確認します。

1. 送信プロセス中に、この画面で進行状況をリアルタイムで追跡し、統計を直接表示できます。

   ![](assets/sent-mail.png)

   また、「**[!UICONTROL ログ]**」ボタンをクリックして、送信に関する詳細情報にアクセスできます。[詳しくは、配信ログの監視方法を参照してください](../monitor/delivery-logs.md)

1. メール送信後、「**[!UICONTROL レポート]**」ボタンをクリックすると、専用のレポートにアクセスしてさらに詳しく分析できます。

![](assets/reports.png)
