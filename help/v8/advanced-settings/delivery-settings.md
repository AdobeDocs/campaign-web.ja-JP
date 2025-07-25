---
audience: end-user
title: 配信設定の指定
description: Campaign web で配信設定を指定する方法について学ぶ
feature: Email, Push, SMS, Direct Mail, Cross Channel Orchestration
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
source-git-commit: 5835d45ea2a383eed7d280fdd263548ea2e8530d
workflow-type: ht
source-wordcount: '3159'
ht-degree: 100%

---


# 配信設定の指定 {#del-settings}

配信設定は、配信テンプレートで定義される&#x200B;**技術的な配信パラメーター**&#x200B;です。配信ごとに過負荷になる可能性があります。これらの設定は、配信または配信テンプレートの編集時に使用できる「**設定**」ボタンから利用できます。

>[!CAUTION]
>
>これらの設定については、情報提供のみを目的として説明しています。一部のものは、設定や権限によって異なります。それらは、このバージョンの製品では変更できません。

## タイポロジ設定 {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="タイポロジ"
>abstract="タイポロジを使用すると、すべての配信にわたってビジネスプラクティスを標準化できます。タイポロジとは、配信状況を制御、フィルター、および優先順位付けするタイポロジルールの集まりです。タイポロジルール内の条件に一致するプロファイルは、準備フェーズで配信オーディエンスから除外されます。"

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_typology"
>title="配信のタイポロジ設定"
>abstract="タイポロジルールを使用すると、すべての配信にわたってビジネスプラクティスを標準化できます。タイポロジとは、配信状況を制御、フィルター、および優先順位付けするタイポロジルールの集まりです。タイポロジルール内の条件に一致するプロファイルは、準備フェーズで配信オーディエンスから除外されます。"

タイポロジとは、複数のフィルタリングルールを配信に対して一度に簡単に適用するために、準備フェーズ中に実行される&#x200B;**タイポロジルール**&#x200B;のセットです。これを使用すると、マーケターは、配信の送信を制御、フィルタリング、優先順位付けできるので、すべての配信でビジネスプラクティスを標準化できます。[詳しくは、タイポロジとタイポロジルールを作成する方法を参照してください](../administration/typologies.md)

![](assets/delivery-settings-typology.png){zoomable="yes"}

### 頻度パラメーター {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_pressure_parameters"
>title="配信の頻度パラメーター"
>abstract="配信の重み付けは、疲労管理のフレームワーク内で最も優先順位の高い配信を指定できます。最も大きな重みを付けられたメッセージが、最優先されます。"

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_weight"
>title="配信の重み付け"
>abstract="配信の重み付けは、頻度管理のフレームワーク内で最も優先順位の高い配信を指定できます。最も大きな重みを付けられたメッセージが、最優先されます。"

このセクションでは、頻度パラメーターを使用して&#x200B;**しきい値**&#x200B;を定義し、疲労管理ルールを設定できます。これは、特定の期間に 1 つのプロファイルに送信できるメッセージの最大数です。

しきい値に達すると、その後は指定された期間が完了するまで、配信は実施できなくなります。このプロセスにより、メッセージの数がしきい値を超過したプロファイルは配信から自動的に除外されるので、過剰な配信が回避できます。

しきい値は、定数または変数のいずれかです。したがって、ある期間、しきい値はプロファイルによって異なる場合も、同じプロファイルで異なる場合もあります。

「**[!UICONTROL 重み付けタイプ]**」フィールドでは、次の 3 つのオプションを使用できます。

* **[!UICONTROL 定数]**
* **[!UICONTROL 受信者に依存]**
* **[!UICONTROL 各ルールで定義]**

「**[!UICONTROL 配信の重み付け]**」フィールドでは、配信の優先順位を定義できます。各配信には、優先度を表す重みが付けられます。
デフォルトでは、配信の重みは 5 に設定されています。頻度ルールでは、適用先となる配信の重み付けを定義できます。重みの値は、定数を指定するか、受信者ごとに数式で算出します。例えば、受信者の興味に基づいて配信の重みを定義することができます。

「**[!UICONTROL 配信モード]**」フィールドでは、ターゲットの評価モードを選択できます。

次の 3 つのモードを選択できます。

* **[!UICONTROL ターゲットの推定とメッセージのパーソナライゼーション]**
* **[!UICONTROL 暫定ターゲットの推定と承認]**
* **[!UICONTROL ターゲットの評価]**

>[!NOTE]
>
>疲労管理と頻度ルールは、Campaign クライアントコンソールで設定されます。詳しくは、[Campaign v8（クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=ja){target="_blank"}を参照してください。

### 処理能力設定 {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_capacity_settings"
>title="配信用の処理能力設定"
>abstract="メッセージを配信する前に、処理能力ルールを使用して、組織が配信や、その配信によって生成される可能性があるインバウンドメッセージと、購読者に連絡するための通話数などを処理できることを確認します。処理能力ルールは、Adobe Campaign v8 コンソールで定義されます。この画面で、チャネルに関連付けられたルールを選択します。"

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_recipient_importance"
>title="受信者の重要度"
>abstract="受信者の重要度は、処理能力タイポロジルールを超過した場合に維持するプロファイルを決定するために使用される式です。"

このセクションでは、Adobe Campaign v8 コンソールで定義した処理能力ルールを選択できます。このルールは、チャネルに関連付けられています。

「**[!UICONTROL 受信者の重要度]**」フィールドは、処理能力タイポロジルールを超過した場合に維持するプロファイルを決定するために使用される式です。

>[!NOTE]
>
>タイポロジルールは、Campaign クライアントコンソールで設定されます。詳しくは、[Campaign v8（クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/consistency-rules.html?lang=ja){target="_blank"}を参照してください。

## オーディエンス設定 {#audience}

>[!CONTEXTUALHELP]
>id="acw_email_settings_audience"
>title="配信用のオーディエンス設定"
>abstract="利用可能な&#x200B;**ターゲットマッピング**&#x200B;を選択します。ターゲットマッピングは、Adobe Campaign v8 コンソールで定義されます。また、配信用の除外パラメーターを設定することもできます。"

このセクションでは、利用可能な&#x200B;**ターゲットマッピング**&#x200B;を選択できます。ターゲットマッピングは、Adobe Campaign v8 コンソールで定義されます。ターゲットマッピングは、操作で処理されるデータのタイプです。ターゲット母集団 (受信者、契約の受取人、オペレーター、サブスクライバーなど) を定義できます。[ターゲットマッピングの詳細情報を参照してください](../audience/targeting-dimensions.md)。

「**[!UICONTROL 除外]**」フィールドでは、今後連絡を希望しないプロファイルや強制隔離されているプロファイルを除外することを選択できます。[詳細情報](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html?lang=ja){target="_blank"}

## 配信 {#delivery}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery"
>title="配信用のグローバル設定"
>abstract="配信パラメーターは、配信に適用する技術的な設定です。配信およびルーチンモードの変更、メールの BCC の有効化、ウェーブを使用した送信および送信されるメールメッセージの形式の選択を行うことができます。これらのオプションは、エキスパートユーザーのみに制限されます。"

**[!UICONTROL 配信]**&#x200B;パラメーターは、配信に適用する技術的な設定です。

![](assets/delivery-settings-delivery.png){zoomable="yes"}

統合された&#x200B;**[!UICONTROL ルーティング]**&#x200B;用外部アカウントがデフォルトで提供されます。アプリケーションから配信を送信するための技術的なパラメーターが含まれます。

次の&#x200B;**[!UICONTROL 送信]**&#x200B;設定を定義できます。

* **[!UICONTROL 配信の優先順位]**：配信の優先順位レベル（標準、高、低）を設定して、配信の送信順序を変更します。

* **[!UICONTROL メッセージのバッチサイズ]**：1 つの XML 配信パッケージ内でグループ化するメッセージの件数を定義します。このパラメーターが 0 に設定されている場合、メッセージは自動的にグループ化されます。パッケージサイズは、`<delivery size>/1024` という計算に基づいて決定されます（ただし、パッケージあたりのメッセージ件数は最小 8、最大 256）。

  >[!IMPORTANT]
  >
  >既存の配信を複製して配信を作成すると、このパラメーターはリセットされます。

* **[!UICONTROL SMTP 配信をテスト]** (メールチャネル) : このオプションを使用して、SMTP 経由での送信をテストします。メールは SMTP サーバーへの接続まで処理されますが、送信はされません。メールの受信者ごとに、Campaign は SMTP プロバイダーサーバーに接続し、「SMTP RCPT TO」コマンドを実行して、「SMTP DATA」コマンドの前に接続を閉じます。

* **[!UICONTROL BCC でメールを送信]** (メールチャネル) : BCC メールアドレスをメッセージのターゲットに追加するだけで、BCC 経由でメールを外部システムに保存します。詳しくは、[Campaign v8（クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/emails/email-bcc.html?lang=ja){target="_blank"}を参照してください。

「**[!UICONTROL ウェーブの定義]**」セクションで、「**[!UICONTROL 複数のウェーブを使用して送信]**」オプションを選択し、ウェーブを使用して送信される音量を徐々に増やします。これにより、メッセージがスパムとしてマークされず、また 1 日あたりのメッセージ数を制限できます。ウェーブを使用すると、一度に大量のメッセージを送信するのではなく、配信をいくつかのバッチに分割できます。[詳細情報](send-using-waves.md)

また、メールの場合は、以下で詳しく説明されているように、送信されるメッセージの&#x200B;**[!UICONTROL メール形式]**&#x200B;を変更することもできます。

* **[!UICONTROL 受信者の環境設定を使用]** (デフォルトモード) : メールの形式は、受信者プロファイルに保存されたデータに従って定義されます。受信者が特定の形式でメールを受信することを希望していれば、メッセージはその形式で送信されます。このフィールドに何も入力されていない場合は、マルチパート/オルタナティブメールが送信されます (以下を参照)。

* **[!UICONTROL 受信者のメールクライアントに最適なフォーマットを選択させる]** : メールには、テキストと HTML の両方の形式が含まれます。受信時に表示されるメッセージ形式は、受信者のメールソフトウェアの設定に応じて切り替わります（マルチパート／オルタナティブ）。

  >[!IMPORTANT]
  >
  >このオプションを指定すると、両方のバージョンのドキュメントがメッセージに含められます。したがって、メールサイズが大きくなり、配信の順位に影響があります。

* **[!UICONTROL すべてのメッセージをテキスト形式で送信]** : メールはテキスト形式で送信されます。HTML 形式は送信されませんが、受信者がメールをクリックした場合にのみミラーページに使用されます。

## Web 分析 {#web-analytics}

>[!CONTEXTUALHELP]
>id="acw_email_settings_webanalytics"
>title="配信用の web 分析設定"
>abstract="Web 分析アカウントを選択します。このアカウントは、Campaign クライアントコンソールで設定されます。使用している分析ツールと共有するタグを定義することもできます。"

このセクションでは、web 分析アカウントを選択できます。このアカウントは、Campaign クライアントコンソールで設定されます。

使用している分析ツールと共有するタグを定義することもできます。

>[!NOTE]
>
>Web 分析機能は、Campaign クライアントコンソールで設定されます。詳しくは、[Campaign v8（クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aa.html?lang=ja#external-account-ac){target="_blank"}を参照してください。

## 再試行 {#retries}

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_retries"
>title="再試行の最大数"
>abstract="一時的なエラーが原因でメッセージ送信が失敗した場合は、配信期間が終了するまで再試行されます。"

<!--Currently not visible in UI > ??-->

ソフトまたは無視のエラーによって一時的に配信できなかったメッセージは、自動再試行の対象となります。デフォルトでは、配信の初日に最低 1 時間の間隔をおいて 24 時間に 5 回の再試行がスケジュールされます。

## 承認 (メールチャネル) {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="配信の承認モード"
>abstract="承認モードを選択します。配信の準備中に警告が発生した場合、配信を設定して、配信を実行するかどうかを定義できます。"

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_approval"
>title="配信の承認モード"
>abstract="このテンプレートに基づく配信の承認モードを選択します。配信の準備中に警告が発生した場合、配信を設定して、配信を実行するかどうかを定義できます。"

メール配信の準備中に警告が発生した場合、配信を設定して、配信を実行するかどうかを定義できます。デフォルトでは、分析フェーズの最後に、メールの送信をユーザーが確認する必要があります (**手動**&#x200B;検証)。

別の承認モードは、該当するフィールドで選択できます。使用可能なモードは次のとおりです。

* **[!UICONTROL 手動]**：分析フェーズの最後に、配信の送信開始をユーザーが確認する必要があります。
* **[!UICONTROL 半自動]**：分析フェーズで警告メッセージが送信されなかった場合には送信が自動的に開始されます。
* **[!UICONTROL 自動]**：分析が終了した時点で、その結果にかかわらず送信が自動的に開始されます。

## 有効性 {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_validity"
>title="設定の有効性"
>abstract="「**配信期間**」フィールドには、グローバルでおこなう配信再試行の期限を入力できます。Adobe Campaign は、開始日にメッセージの送信を開始した後、エラーのみを返すメッセージについて、設定された定期的な再試行を、有効期限日に達するまで実行します。<br>「**リソースの有効期間**」フィールドは、ミラーページや画像などのアップロードされたリソースに使用されます。制限に達すると、リソースは使用できなくなります。"

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_resources_validity"
>title="リソースの有効期間"
>abstract="「**リソースの有効期間**」フィールドは、ミラーページや画像などのアップロードされたリソースに使用されます。これらのリソースは限られた時間のみ有効です。制限に達すると、リソースは使用できなくなります。"

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_duration"
>title="配信期間"
>abstract="「**配信期間**」フィールドには、グローバルでおこなう配信再試行の期限を入力できます。Adobe Campaign は、開始日にメッセージの送信を開始した後、エラーのみを返すメッセージについて、設定された定期的な再試行を、有効期限日に達するまで実行します。"

<!--
>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Resources validity limit"
>abstract="The Validity limit field is used for uploaded resources, such as the mirror page or images. These resources are valid for a limited time: once the limit is reached, resources are no longer available."
-->

### 有効期間 {#validity-period}

「**[!UICONTROL 配信期間]**」フィールドには、グローバルでおこなう配信再試行の期限を入力できます。Adobe Campaign は、開始日にメッセージの送信を開始した後、エラーのみを返すメッセージについて、設定された定期的な再試行を、有効期限日に達するまで実行します。

日付を指定することもできます。そのためには、「**[!UICONTROL 有効期限を明示的に設定]**」を選択します。この場合、配信および有効期限日に時刻を指定することもできます。デフォルト値は現在時刻ですが、入力フィールドを使用して直接変更できます。

「**[!UICONTROL リソースの有効期限]**」フィールドは、主にミラーページや画像のアップロードされたリソースに使用されます。ディスク容量を節約するために、このページ上のリソースは限られた時間のみ有効です。この制限を超えると、これらのリソースは使用できなくなります。

![](assets/delivery-settings-validity.png){zoomable="yes"}

<!--Change screenshot to be consistent with prod > not sure which version is correct-->

配信の有効期間について詳しくは、[Campaign v8（クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=ja#validity-period){target="_blank"}を参照してください。

### ミラーページ管理 (メールチャネル) {#mirror}

ミラーページは、web ブラウザーでオンラインアクセス可能な HTML ページです。そのコンテンツはメールと同一です。デフォルトでは、メールのコンテンツにリンクが挿入されている場合にミラーページが生成されます。

デフォルトモードのほかに、次のオプションも選択できます。

* **[!UICONTROL ミラーページを強制的に生成]** : このモードを使用すると、メールにミラーページへのリンクが挿入されていなくても、ミラーページを生成します。
* **[!UICONTROL ミラーページを生成しない]** : このモードを使用すると、メールにリンクが存在する場合でも、ミラーページを生成しないようにすることができます。
* **[!UICONTROL メッセージ識別子のみを使用してアクセス可能なミラーページを生成]**：メールコンテンツにミラーページのリンクが存在しない場合、このオプションを使用して、クライアントコンソールから配信ログウィンドウでミラーページのコンテンツにアクセスできるようにします。

### トラッキング {#tracking}

<!--
>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Validity period"
>abstract="This option defines the duration for which the tracking is activated on the URLs."
-->

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_tracking_validity"
>title="有効期間"
>abstract="有効期間には、メッセージ URL に対してトラッキングがアクティブになっている期間を設定します。"

**[!UICONTROL トラッキング]**&#x200B;パラメーターは、関連するセクションで定義されています。選択できるオプションは次のとおりです。

* **[!UICONTROL トラッキングの有効期限]**：URL に対してトラッキングがアクティブになっている期間を変更するのに使用できます。
* **[!UICONTROL 期限切れ URL の代替 URL]**：フォールバック Web ページへの URL を入力します。トラッキングの有効期限が切れると表示されます。

## 配達確認設定 {#test-setttings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_testsettings"
>title="配信用の配達確認設定の定義"
>abstract="除外パラメーターを選択し、配達確認のラベルをカスタマイズします。"

<!--Test to be replaced with Proof everywhere - currently not consistent within UI > changed to Proof to reflect UI here but not consistent in documentation either-->

このセクションでは、除外パラメーターを設定できます。次のオプションを使用できます。

* **[!UICONTROL 重複を保持]** : 複数のターゲティング条件を満たすプロファイルに対して複数の配信を許可できます。
* **[!UICONTROL ブロックリスト登録済みアドレスを保持]**：購読解除（オプトアウト）後など、配信のターゲットでなくなったプロファイルをターゲットから除外できます。
* **[!UICONTROL 強制隔離されたアドレスを保持]**：プロファイルで指定されているアドレスからの応答がないターゲットを除外できます。

また、配達確認のラベルをカスタマイズすることもできます。

* **[!UICONTROL 配達確認の配信コードを保持]**&#x200B;を使用すると、関連する配信用に定義されたのと同じ配信コードを、配達確認に関連付けることができます。
* デフォルトでは、配達確認の件名の先頭に接頭辞「PROOF #」が付きます（「#」は配達確認の番号）。この接頭辞は「**[!UICONTROL ラベルの接頭辞]**」フィールドで変更できます。

## SMS 設定（SMS チャネル） {#sms-tab}

>[!CONTEXTUALHELP]
>id="acw_sms_delivery_settings"
>title="SMS 配信設定"
>abstract="SMS 配信パラメーターは、SMS 配信に適用する技術的な設定です。送信者のアドレス、サービスパラメーター、送信モードなどを定義できます。これらのオプションは、エキスパートユーザーのみに制限されます。"

SMS 配信パラメーターは、SMS 配信に適用する技術的な設定です。送信者のアドレス、サービスパラメーター、送信モードなどを定義できます。これらのオプションは、エキスパートユーザーのみに制限されます。

<!--

* **[!UICONTROL Sender address]**

  The field is limited to 21 characters by the SMPP specification, but some providers may allow longer values. Note also that very strict restrictions may be applied in some countries (length, content, allowed characters, …), so you may need to double-check that the content you place here is legal. Be especially careful when using personalized fields.


  This optional field allows you to override the sender address (oADC). Its content is placed in the *source_addr* field of the SUBMIT_SM PDU.

  Although the SMPP specification limits this field to 21 characters, some providers may support longer values. Be aware that certain countries impose strict regulations on sender addresses (regarding length, content, allowed characters, etc.), so always verify that your input complies with local requirements. Use extra caution when working with personalized fields.

  If this field is left empty, the value of the Source number field defined in the external account will be used instead. If both values are empty, the *source_addr* field will be left empty.

-->

* **[!UICONTROL サービスタイプ]**：

  このパラメーターは、プロバイダーにそのまま渡されます。

* **[!UICONTROL サービスまたはプログラム ID]**

  >[!NOTE]
  >
  >このフィールドの使用はお勧めしません。クライアントコンソールで使用できるオプションの SMPP パラメーターにより、より柔軟な実装が可能になります。
  >
  >このフィールドは、オプションの SMPP パラメーターと同時に使用できません。

  一致する外部アカウント設定と組み合わせることで、各 MT で 1 つのオプションパラメーターを送信できます。このフィールドは、TLV の値のパートを定義します。

* **[!UICONTROL 送信モード]**

  このフィールドでは、送信する SMS のタイプ（通常メッセージまたは Flash メッセージか、モバイルデバイスまたは SIM カードに保存する必要があるか）を定義します。この設定は、SUBMIT_SM PDU の dest_addr_subunit オプションフィールドに送信されます。

   * 「**Flash**」の場合、値を 1 に設定します。画面にすぐに表示され、保存されない Flash SMS を送信します。
   * 「**通常**」の場合、値を 0 に設定します。標準の SMS を送信します。
   * 「**携帯電話に保存**」の場合、値を 2 に設定します。SMS を内部メモリに保存するようデバイスに指示します。
   * 「**ターミナルに保存**」の場合、値を 3 に設定します。SMS を SIM カードに保存するようデバイスに指示します。

* **[!UICONTROL 優先度、通信タイプ]**

  これらのフィールドは、拡張 SMPP コネクタでは無視されます。

* **[!UICONTROL メッセージあたりの SMS の最大数]**

  この設定は、メッセージペイロードオプションが無効な場合にのみ有効です（詳しくは、外部アカウント設定を参照してください）。メッセージにこの値より多くの SMS が必要な場合は、エラーがトリガーされます。

  SMS プロトコルでは、メッセージを最大 255 個の部分に分割できますが、一部のモバイルデバイスでは、10 個を超える部分のメッセージを再構築することが困難な場合があります（制限はデバイスモデルによって異なります）。信頼性を高めるには、メッセージの部分を 5 個以下に制限することをお勧めします。

  Adobe Campaign でのパーソナライズされたメッセージの動作によって、メッセージのサイズが異なる場合があります。長いメッセージの数が多いと、送信コストが増加する可能性があるので、適切な制限を使用すると費用を管理するのに役立ちます。

  この値を 0 に設定すると、制限が無効になります。

## メール配信の SMTP 設定 {#smtp}

>[!CONTEXTUALHELP]
>id="acw_email_settings_smtp"
>title="SMTP パラメーター"
>abstract="メール配信に、追加 SMTP パラメーターを追加できます。"

メール配信に、追加 SMTP パラメーターを追加できます。この操作は、配信設定の「SMTP」タブで実行できます。

![](assets/smtp_tab.png){zoomable="yes"}

### 文字エンコーディング {#character-encoding}

「**[!UICONTROL 文字エンコーディング]**」セクションでは、特定のエンコーディングを設定できます。デフォルトのエンコーディングは UTF-8 で、ほとんどの文字に対して機能します。ただし、一部のメールプロバイダーでは、UTF-8 標準エンコーディングをサポートしていない場合、特殊文字が正しく表示されない可能性があります。

例えば、日本語の文字を含むメールを送信する場合は、日本のオーディエンスがすべてを正しく表示できるように、これらの文字専用のエンコーディングを使用することをお勧めします。

これを行うには、「**[!UICONTROL メッセージに使用されているエンコーディングを強制]**」切替スイッチをアクティブ化し、特殊文字をサポートするリストから適切なエンコーディングを選択します。

![](assets/smtp_encoding.png){zoomable="yes"}

### バウンスメール {#bounce-emails}

配信設定の「**[!UICONTROL SMTP]**」タブでは、バウンスメール管理を設定することもできます。

* **[!UICONTROL エラーアドレス]**：「**[!UICONTROL プラットフォームに定義されたデフォルトのエラーアドレスを使用]**」切替スイッチをアクティブ化する場合は、バウンスメールがプラットフォームのデフォルトエラーボックスに受信されます。アクティブ化しない場合は、配信用の専用エラーアドレスを定義できます。

* **[!UICONTROL バウンスアドレス]**：未処理のバウンスメールの転送先となる別のアドレスを定義することもできます。バウンスメールの発生理由をアプリケーションで自動判定できない場合は、このアドレスを使用することで調査できます。

これら 2 つのフィールドは、[この節](../personalization/gs-personalization.md)の説明に従ってパーソナライズできます。

![](assets/smtp_bounce.png){zoomable="yes"}

### 追加の SMTP ヘッダー {#smtp-headers}

配信設定の「SMTP」タブで、メール配信に **[!UICONTROL SMTP ヘッダー]**&#x200B;を追加できます。

このウィンドウで入力するスクリプトは、name:value の形式で 1 行ごとに 1 つのヘッダーを参照する必要があります。

値は必要に応じて自動的にエンコードされます。

![](assets/smtp_headers.png){zoomable="yes"}


>[!IMPORTANT]
>
>スクリプトを追加すると、挿入する SMTP ヘッダーを追加できます。これは高度な知識を持つユーザー向けに用意されています。スクリプトの構文は、このコンテンツタイプの要件を満たしている必要があります（不要なスペースや空行を含まないなど）。

## 変数の追加 {#variables-delivery}

>[!CONTEXTUALHELP]
>id="acw_delivery_settings_variable"
>title="変数"
>abstract="配信に変数を追加できます。これは、トラッキングやパーソナライゼーションに役立ちます。これらの変数には、配信コンテンツとワークフローの両方からアクセスできます。"

配信に変数を追加できます。これは、トラッキングやパーソナライゼーションに役立ちます。これらの変数には、配信コンテンツとワークフローの両方からアクセスできます。保存された変数は、配信内のすべてのメッセージにわたって値が一定となるよう設定するために使用します。また、配信テンプレートで設定することもできます。

変数を追加するには、次に示すように、「**[!UICONTROL 変数]**」タブを参照します。

![](assets/variables-tab.png){zoomable="yes"}

「**[!UICONTROL 変数を追加]**」ボタンをクリックして、変数の詳細を入力します。その値を直接追加することも、チェックボックスをオンにすることで値に式を使用することもできます。**[!UICONTROL 値は式の結果です]**。次に、「**[!UICONTROL 確認]**」をクリックして変更を保存します。

![](assets/variables-add.png){zoomable="yes"}

[パーソナライゼーションに変数を使用](../personalization/personalize.md#variables-personalization)と[動的コンテンツに変数を使用](../personalization/conditions.md#variables-conditional)について詳しく説明します。