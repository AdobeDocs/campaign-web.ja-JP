---
audience: end-user
title: 最初のメールの送信
description: Campaign Web UI での最初のメールの送信方法を説明します
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
source-git-commit: 384c7ac2dd2b1d90ba6ff78f59aacce396de91f0
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 67%

---

# 最初のメールの送信 {#first-email}

![](../assets/do-not-localize/badge.png)

このユースケースでは、最初のメールの作成方法を示します。シルバーロイヤルティ顧客とゴールドロイヤルティ顧客に対して特定の日にメールを送信するようスケジュールを設定します。このメールは、事前定義済みテンプレートを使用してデザインされ、プロファイルの属性を使用してパーソナライゼーションを組み込みます。

![](assets/delivery-list.png)

## メールの作成 {#create-email}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_template_selection"
>title="メールテンプレートの選択"
>abstract="テンプレートは、Adobe Campaign v8 コンソールで定義されます。 これは、タイポロジルール、パーソナライゼーション、ルーティングパラメーターなどの事前定義済みパラメーターを含んだ特定の配信設定です。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_properties"
>title="メールのプロパティ"
>abstract="プロパティは、配信の名前付けや分類に役立つ一般的な配信パラメーターです。配信が Adobe Campaign v8 コンソールで定義された拡張スキーマに基づいている場合は、いくつかの特定の&#x200B;**カスタムオプション**&#x200B;フィールドを使用できます。"

1. **[!UICONTROL 配信]**&#x200B;メニューから新しい配信を作成します。

1. を選択します。 **[!UICONTROL 電子メール]** チャネルと使用するテンプレートを選択し、「 **[!UICONTROL 配信を作成]**.

   >[!NOTE]
   >
   >テンプレートとは、再利用するためにテンプレートとして保存された特定の配信設定です。配信テンプレートは、Adobe Campaign コンソールで管理者ユーザーが設定します。[配信テンプレートの使用方法を説明します。](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/create-templates.html){target="_blank"}.

   ![](assets/channel-template.png)

1. メールのラベルを指定し、必要に応じて追加のオプションを設定します。

   * **[!UICONTROL 内部名]**：配信に一意の ID を割り当てます。
   * **[!UICONTROL フォルダー]**：配信を特定のフォルダーに保存します。
   * **[!UICONTROL 配信コード]**：このフィールドを使用すると、独自の命名規則に基づいて配信を整理できます。
   * **[!UICONTROL 説明]**：配信の説明を指定します。
   * **[!UICONTROL 特性]**：分類目的でメールの特性を指定します。<!--The content of the list is defined in the delivery template selected when creating the email.-->
   >[!NOTE]
   >
   >特定のカスタムフィールドを使用してスキーマを拡張した場合は、 「**[!UICONTROL カスタムオプション]**」セクションでそれらのフィールドにアクセスできます。

   ![](assets/email-properties.png)

   さらに、詳細設定（タイポロジルール、ターゲットマッピングなど）が、配信名の横にあるボタンから使用できます。 これらは、メールの作成時に選択したテンプレートで事前に定義されています。必要に応じて編集できます。

## メールコンテンツの作成 {#create-content}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="電子メールデザイナーを使用してメールコンテンツをデザインする方法について説明します。"
>abstract="コンテンツのデザイン方法について説明します"

このユースケースでは、事前定義済みテンプレートを使用してメールをデザインします。 メールコンテンツを設定する方法について詳しくは、[この節](../content/edit-content.md)を参照してください。

1. 「**[!UICONTROL コンテンツを編集]**」ボタンをクリックして、メールコンテンツの作成を開始します。

   この画面では、メールコンテンツを設定し、電子メールデザイナーを使用してデザインできます。

   ![](assets/edit-content.png)

1. メールの件名を指定し、式エディターを使用してパーソナライズします。詳しくは、[コンテンツをパーソナライズする方法](../personalization/personalize.md)を参照してください。

   ![](assets/subject-line.png)

1. 「**[!UICONTROL メール本文を編集]**」ボタンをクリックして、メールのコンテンツを作成およびデザインします。

   メールコンテンツの作成に使用する方法を選択します。この例では、既存のデザインテンプレートを使用します。

   ![](assets/select-template.png)

<!--1. Select the HTML or ZIP file to import then click **[!UICONTROL Next]**.

    If your folder contains assets, choose the instance and folder where they should be stored then click **[!UICONTROL Import]**. (+ link to doc on assets?)

    ![](assets/import-folder.png)-->

1. テンプレートを選択すると、それが電子メールデザイナーに表示されるので、必要に応じて編集したり、パーソナライゼーションを追加したりできます。

   この例では、メールのタイトルにパーソナライゼーションを追加します。それには、コンポーネントブロックを選択し、「**[!UICONTROL パーソナライゼーションを追加]**」をクリックします。

   ![](assets/add-perso.png)

1. コンテンツの準備が整ったら、デザインを保存して閉じ、「 」をクリックします。 **[!UICONTROL 保存]** をクリックして、e メール作成画面に戻ります。

   ![](assets/save-content.png)

## オーディエンスの定義 {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="オーディエンスの定義"
>abstract="マーケティングメッセージに最適なオーディエンスを選択します。Campaign v8 インスタンスで既に定義されている既存のオーディエンスを選択するか、Adobe Experience Platformから選択するか、ルールビルダーを使用して新しいオーディエンスを作成するかを選択できます。"

この使用例では、既存のオーディエンスにメールを送信します。オーディエンスの操作方法に関する追加情報については、[この節](../audience/about-audiences.md)を参照してください。

1. 「**[!UICONTROL オーディエンスを選択]**」ボタンをクリックして、ターゲットにする既存のオーディエンスを選択します。

   この例では、シルバーおよびゴールドのロイヤルティポイントレベルに属する顧客をターゲティングする既存のオーディエンスを使用します。

   ![](assets/create-audience.png)

   >[!NOTE]
   >
   >リストで使用可能なオーディエンスは、Campaign V8 インスタンスから、またはインスタンスで宛先/ソースの統合が設定されている場合はAdobe Experience Platformから作成されます。
   >
   >宛先/ソースの統合により、Experience PlatformセグメントをAdobe Campaignに送信したり、キャンペーンの配信とトラッキングログをAdobe Experience Platformに送信したりできます。 [Campaign とAdobe Experience Platformの連携の仕組み](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep.html){target="_blank"}.

1. オーディエンスを選択したら、追加のルールを使用してターゲットを絞り込むことができます。

   また、コントロール母集団を設定して、ターゲットされていないプロファイルの動作と比較した、メール受信者の行動を分析することもできます。[詳しくは、コントロール母集団の操作方法を参照してください](../audience/control-group.md)

   ![](assets/audience-selected.png)

## 送信のスケジュール設定 {#schedule}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_schedule"
>title="送信のスケジュール設定"
>abstract="送信の日付と正確な時刻を定義します。マーケティングメッセージに最も適した時間を選択することで、開封率を最大化します。"

メールの送信をスケジュールするには、「**[!UICONTROL 有効にする]**」をクリックしてから、送信する日時を指定します。

デフォルトでは、 **[!UICONTROL 送信前の確認]** 」オプションが有効になっている場合、指定した日時に E メールを送信できるように、送信を確定する必要があります。 このオプションを無効にすると、確認を必要とせずにスケジュールされた日時にメールが送信されます。

![](assets/schedule.png)

## メールのプレビューとテスト {#preview-test}

メールの準備が整ったら、送信を開始する前に、プレビューおよびテストできます。

この使用例では、ターゲットプロファイルの一部を偽装しているときに、E メールをプレビューし、特定の E メールアドレスに配達確認を送信します。

メールのプレビューおよびテスト方法に関する追加情報については、 [この節](../preview-test/preview-test.md)を参照してください。

1. クリック **[!UICONTROL 確認して送信]**. メールのプレビューが、設定済みのすべてのプロパティ、オーディエンス、スケジュールと共に表示されます。変更ボタンを使用して、これらの要素を編集できます。

1. 「**[!UICONTROL コンテンツをシミュレート]**」ボタンをクリックして、メールをプレビューし、配達確認を送信します。

   ![](assets/review-email.png)

1. 左側の領域で、メールのプレビューに使用するプロファイルを選択します。

1. 選択したプロファイルに基づいて、メールのプレビューが右側のパネルに表示されます。 複数のプロファイルを追加した場合は、それぞれを切り替えて、対応するメールをプレビューできます。

   ![](assets/preview.png)

   <!-- !NOTE
    >
    >Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using mutiple devices or mail providers. Learn on how to preview email rendering-->

1. E メールの配達確認を送信するには、 **[!UICONTROL テスト]** ボタンをクリックして、配達確認の送信に使用するモードを選択します。

   この例では、「メインターゲットから代替」モードを使用します。つまり、配信のターゲットとなる一部のプロファイルを偽装しながら、特定の E メールアドレスに配達確認を送信します。

   ![](assets/proof-mode.png)

1. 「アドレスを追加」をクリックし、配達確認を受信する電子メールアドレスを指定します。

   各電子メールアドレスに対して、別のユーザーとして実行するターゲットからプロファイルを選択します。 また、Adobe Campaign にターゲットからランダムプロファイルを選択させることもできます。

   ![](assets/proof-test-profile.png)

1. 「**[!UICONTROL テストメールを送信]**」をクリックし、送信を確認します。

   配達確認は、選択したプロファイルを使用して指定した E メールアドレスに、 **[配達確認 x]** プレフィックス

   ![](assets/proof-sent.png)

   送信のステータスを確認し、送信済みの配達確認にいつでもアクセスするには、 **[!UICONTROL テストメールログを表示]** 「コンテンツをシミュレート」画面の「 」ボタン

## メールの送信と監視 {#prepare-send}

メールをレビューおよびテストしたら、準備を開始して送信できます。

1. 「**[!UICONTROL 準備]**」をクリックして、メッセージの準備を開始します。[詳しくは、メールの準備方法を参照してください](../monitor/prepare-send.md)

   ![](assets/preparation.png)

1. E メールを送信する準備が整ったら、「 **[!UICONTROL 送信]** または **[!UICONTROL 予定どおりに送信]** 次に、送信を確定します。

1. E メールの送信が開始されたら、即座に、またはスケジュールされた日に、この画面で E メールの送信を統計と共にリアルタイムで追跡できます。

   ![](assets/sent-mail.png)

   >[!NOTE]
   >
   >また、「**[!UICONTROL ログ]**」ボタンを使用すると、メール送信に関する詳細情報にアクセスできます。[詳しくは、配信ログの監視方法を参照してください](../monitor/delivery-logs.md)

1. メールの送信後、詳細な分析のために専用のレポートにアクセスできます。[レポートの操作方法を説明します。](../reporting/reports.md)
   ![](assets/reports.png)
