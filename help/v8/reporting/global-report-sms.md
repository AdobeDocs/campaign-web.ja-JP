---
audience: end-user
title: SMS チャネルのグローバルレポート
description: SMS チャネルのグローバルレポートについて
badge: label="限定提供（LA）"
source-git-commit: 6fbc6d477aac54e8cb7a1eeba40f7c32903c261f
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 26%

---

# SMS チャネルのグローバルレポート {#campaign-reports-sms}

グローバルレポートでは、トラフィック指標とエンゲージメント指標の包括的な概要をチャネルレベルでユーザーに提供します。

次に移動： **[!UICONTROL レポート]** メニュー内 **[!UICONTROL レポート]** 」セクションに入力します。 レポートの日付、フォルダーまたはルールに応じて、データをフィルタリングできます。 [詳細情報](global-reports.md)

## 配信の概要 {#delivery-summary-sms}

### 配信の概要 {#delivery-overview-sms}

The **[!UICONTROL 配信の概要]** レポートは、包括的な主要業績評価指標 (KPI) を提供し、各 SMS 配信に対する訪問者のインタラクションパターンに関する深いインサイトを提供します。 以下に、以下の指標の概要を示します。

![](assets/global_report_sms_delivery_overview.png)

+++配信の概要指標について詳しく説明します。

* **[!UICONTROL 配信メッセージ数]**：配信の準備中に処理されたメッセージの合計数。

* **[!UICONTROL 配信済み]**：送信されたメッセージの合計数に対する、正常に送信されたメッセージの割合。

* **[!UICONTROL クリックスルー率]**：配信で少なくとも 1 回クリックしたユニーク受信者の割合。

* **[!UICONTROL エラー]**：送信されたメッセージの合計数に対する、配信および自動返信処理の間に累積したエラーの割合。

+++

### 対象オーディエンス {#delivery-summary-sms-initial-target}

The **[!UICONTROL ターゲットオーディエンス]** 各送信 SMS 配信の受信者に関する表およびグラフのデータを参照してください。 指標については、以下で詳しく説明します。

![](assets/global_report_sms_targeted_audience.png)

+++ターゲットオーディエンス指標の詳細を説明します。

* **[!UICONTROL ターゲットオーディエンス]**：ターゲット受信者の合計数。

* **[!UICONTROL 配信メッセージ数]**：配信準備の後に配信されるメッセージの合計数。

* **[!UICONTROL 除外]**：ルール（アドレスが見つからない、強制隔離された、上など）を適用する際、分析中に無視されたアドブロックリストに加えるレスの合計数。

+++

### 配信統計 {#delivery-summary-sms-exec-stats}

The **[!UICONTROL 配信統計]** テーブルには、各 SMS 配信の成功の詳細が表示されます。 指標については、以下で詳しく説明します。

![](assets/global_report_sms_delivery_statistics.png)

+++配信統計指標の詳細を説明します。

* **[!UICONTROL 合計メッセージ数]**：配信の準備後に配信されるメッセージの合計数。

* **[!UICONTROL 成功]**：配信されるメッセージ数に関して正常に処理されたメッセージ数。

* **[!UICONTROL エラー/バウンス]**：配信するメッセージ数に関して、配信と自動リバウンド処理の間に累積したエラーの合計数。

* **[!UICONTROL 新しい強制隔離]**：配信の失敗後（不明なユーザー、無効なドメイン）に、配信されるメッセージ数に関して強制隔離されたアドレスの合計数。

  SMS エラータイプについては、[Adobe Campaign v8 （クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=ja#sms-quarantines){target="_blank"}を参照してください。

+++

### 除外の理由 {#causes-exclusion}

The **[!UICONTROL 除外の理由]** グラフおよびテーブルには、ターゲットプロファイルから除外されたユーザープロファイルが SMS 配信を受信できなかった理由が表示されます。

エラータイプは、 [Adobe Campaign v8 （クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=ja#email-error-types){target="_blank"}.

![](assets/global_report_sms_causes_exclusion.png)

## 配信スループット {#delivery-throughput-sms}

![](assets/global_report_sms_delivery_throughput.png)

このレポートは、指定した期間内の配信スループットに関する包括的な詳細を提供します。
