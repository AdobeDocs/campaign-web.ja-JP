---
audience: end-user
title: 最初のメールの送信
description: Campaign web UI での最初のメールの送信方法を学ぶ
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
badge: label="Alpha" type="Positive"
source-git-commit: db3bb5c9805ce5c04ea657cf2d71c5528a9980d3
workflow-type: tm+mt
source-wordcount: '1329'
ht-degree: 92%

---


# 最初のメールの送信 {#first-email}

>[!CONTEXTUALHELP]
>id="acw_homepage_card2"
>title="メールの概要"
>abstract="テンプレートから開始するか、Adobe Campaignの新しい電子メールデザイナーを使用して、コードを 1 行も書かずに電子メールを作成できます。 E メールデザイナーを使用して、コンテンツを作成、プレビューおよびテストし、既存のオーディエンスに E メールをエンドツーエンドで送信する方法を説明します。"


最初のターゲットメールを作成する方法について説明します。このユースケースでは、特定の日にシルバーおよびゴールドのロイヤルティメンバーにメールを送信するようにスケジュールします。

事前定義されたデザインテンプレートに基づき、メールには、顧客プロファイル属性に基づいてパーソナライズされたコンテンツも含まれます。

![](assets/delivery-list.png)

## E メール配信の作成 {#create-email}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_template_selection"
>title="メールテンプレートの選択"
>abstract="メールテンプレートは、タイポロジルール、パーソナライゼーション、ルーティングパラメーターなど、事前定義された設定を含む特定の配信設定です。テンプレートは、Campaign クライアントコンソールで定義されます。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_properties"
>title="メールのプロパティ"
>abstract="プロパティは、配信の名前付けや分類に役立つ一般的な配信パラメーターです。配信が Adobe Campaign v8 コンソールで定義された拡張スキーマに基づいている場合は、いくつかの特定の&#x200B;**カスタムオプション**&#x200B;フィールドを使用できます。"

新しい配信を作成するには、次の手順に従います。

1. 次を参照： **[!UICONTROL 配信]** 左側のパネルのメニューで、  **[!UICONTROL 配信を作成]** 」ボタンをクリックします。

1. 「**[!UICONTROL メール]**」をチャネルとして選択し、テンプレートを選択します。

   >[!NOTE]
   >
   >テンプレートは、後で使用するために保存された、事前設定済みの配信設定です。[詳細情報](../msg/delivery-template.md)

   ![](assets/channel-template.png)

1. 「**[!UICONTROL 配信を作成]**」ボタンをクリックして、確定します。
1. 配信のラベルを入力し、必要に応じて追加のオプションを設定します。

   * **[!UICONTROL 内部名]**：配信に一意の ID を割り当てます。
   * **[!UICONTROL フォルダー]**：配信を特定のフォルダーに保存します。
   * **[!UICONTROL 配信コード]**：このフィールドを使用すると、独自の命名規則に基づいて配信を整理できます。
   * **[!UICONTROL 説明]**：配信の説明を指定します。
   * **[!UICONTROL 特性]**：分類目的でメールの特性を指定します。<!--The content of the list is defined in the delivery template selected when creating the email.-->

   >[!NOTE]
   >
   >特定のカスタムフィールドを使用してスキーマを拡張した場合は、 「**[!UICONTROL カスタムオプション]**」セクションでそれらのフィールドにアクセスできます。

   ![](assets/email-properties.png)

   また、タイポロジルールやターゲットマッピングなどの詳細設定には、配信名の横にあるボタンをクリックしてアクセスできます。これらの設定は、選択したテンプレートで事前に設定されていますが、この特定のメールの必要に応じて編集できます。

## メールコンテンツの作成 {#create-content}

メールコンテンツを設定する方法について詳しくは、[この節](../content/edit-content.md)を参照してください。

このユースケースでは、事前定義されたテンプレートを使用してメールをデザインします。

1. メールコンテンツの作成を開始するには、メール配信を開き、「**[!UICONTROL コンテンツを編集]**」ボタンをクリックします。

   これにより、メールコンテンツを設定し、電子メールデザイナーを使用してデザインできる専用のインターフェイスが表示されます。

   ![](assets/edit-content.png)

1. メールの件名を入力し、式エディターを使用してパーソナライズします。詳しくは、[コンテンツをパーソナライズする方法](../personalization/personalize.md)を参照してください。

   ![](assets/subject-line.png)

1. メールのコンテンツをデザインするには、「**[!UICONTROL メール本文を編集]**」ボタンをクリックします。

   メールコンテンツの作成に使用する方法を選択します。この例では、事前定義済みのデザインテンプレートを使用します。

   ![](assets/select-template.png)

   <!--1. Select the HTML or ZIP file to import then click **[!UICONTROL Next]**.

    If your folder contains assets, choose the instance and folder where they should be stored then click **[!UICONTROL Import]**. (+ link to doc on assets?)

    ![](assets/import-folder.png)-->

1. テンプレートを選択すると、電子メールデザイナーに表示され、必要な編集を加えたり、パーソナライゼーションを追加したりできます。

   例えば、パーソナライゼーションをメールタイトルに追加するには、コンポーネントブロックを選択し、「**[!UICONTROL パーソナライゼーションを追加]**」をクリックします。

   ![](assets/add-perso.png)

1. コンテンツの設定が完了したら、デザインを保存して閉じます。「**[!UICONTROL 保存]**」をクリックして、メール作成画面に戻ります。

   ![](assets/save-content.png)

## オーディエンスを定義 {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="オーディエンスを定義"
>abstract="マーケティングメッセージに最適なオーディエンスを選択します。Campaign v8 インスタンスまたは Adobe Experience Platform で既に定義されている既存のオーディエンスを選択するか、ルールビルダーを使用して新しいオーディエンスを作成できます。「ファイルから選択」に対してはコントロール母集団が有効になっていません。逆も同様です。"

このユースケースでは、既存のオーディエンスにメールを送信します。オーディエンスの操作方法に関する追加手順については、[この節](../audience/about-audiences.md)を参照してください。

1. メールのオーディエンスを選択するには、「**[!UICONTROL オーディエンスを選択]**」ボタンをクリックし、リストから既存のオーディエンスを選択します。

   この例では、シルバーおよびゴールドのロイヤルティポイントレベルに属する顧客をターゲティングする既存のオーディエンスを使用します。

   ![](assets/create-audience.png)

   >[!NOTE]
   >
   >リストで使用可能なオーディエンスは、Campaign v8 インスタンスから、またはインスタンスに宛先／ソースの統合が設定されている場合は Adobe Experience Platform から作成されます。
   >
   >宛先／ソースの統合により、Experience Platform セグメントを Adobe Campaign に送信したり、キャンペーンの配信とトラッキングログを Adobe Experience Platform に送信したりできます。[Campaign と Adobe Experience Platform の連携方法を参照してください](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep.html?lang=ja){target="_blank"}。

1. オーディエンスを選択したら、追加のルールを適用してターゲットを絞り込むことができます。

   またコントロール母集団を設定して、ターゲットとならなかったユーザーと比較してメール受信者の行動を分析することもできます。[詳しくは、コントロール母集団の操作方法を参照してください](../audience/control-group.md)

   ![](assets/audience-selected.png)

## 送信のスケジュール設定 {#schedule}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_schedule"
>title="送信のスケジュール設定"
>abstract="送信の日付と正確な時刻を定義します。マーケティングメッセージに最も適した時間を選択することで、開封率を最大化します。"

メールの送信スケジュールを設定するには、メール配信を開き、「**スケジュール**」セクションを参照します。「**[!UICONTROL スケジュールを有効にする]**」切替スイッチを使用してスケジュールをアクティベートし、送信する日時を設定します。配信を送信すると、実際の送信は、定義したコンタクト日に開始されます。

デフォルトでは、「**[!UICONTROL 送信前に確認を有効にする]**」オプションが有効になっています。このオプションでは、スケジュール設定した日時にメールを送信する前に送信を確定する必要があります。スケジュールを設定した日時にメールを自動的に送信する必要がある場合は、このオプションを無効にします。

![](assets/schedule.png)

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

   <!-- !NOTE
    >
    >Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using mutiple devices or mail providers. Learn on how to preview email rendering-->

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
