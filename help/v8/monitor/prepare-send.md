---
audience: end-user
title: E メールの準備と送信
description: Campaign v8 Web ドキュメント
source-git-commit: fe06419e429f48dbcc71802c372130be22e68d52
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 13%

---

# メールの準備と送信 {#prepare-send}

>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="メールの準備と送信"
>abstract="メールの準備方法と KPI の送信に関する詳細を確認します。"

>[!NOTE]
>
>このドキュメントは作成中で、頻繁に更新されています。 このコンテンツの最終バージョンは、2023 年 1 月に準備が整います。

<!--

	show how to prepare and send the email + the live kpis in the dashboard

like acc when preparation, target calculated then send
real time KPIs, not in AJO. similar to ACS.
exclusion logs, causes
-->

<!--
send also KPIs
-->

## 送信の準備

準備中に、ターゲット母集団が計算され、ターゲットに含まれる各プロファイルに対して生成されるメッセージコンテンツが表示されます。 準備が完了したら、メッセージは、即座に、またはスケジュールされた日時に送信できる状態になります。 分析時に使用される検証ルールについて詳しくは、ここで説明します [セクション](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/key-steps-when-creating-a-delivery/steps-validating-the-delivery.html?lang=en#validation-process-with-typologies).

1. 次をクリック： **準備** ボタンをクリックします。

1. 準備の進行状況が表示されます。 ターゲット母集団のサイズによっては、この操作に時間がかかる場合があります。

   >[!NOTE]
   >
   >準備は、 **準備を停止** 」ボタンをクリックします。 準備段階では、メッセージは送信されません。 したがって、何かに影響を与えるリスクを伴わずに、これを開始または停止できます。

1. 準備が完了したら、 **ターゲット**, **配信する** および **除外する** KPI 送信するメッセージの数が期待どおりでない場合は、オーディエンスを変更し、準備を再開します。

1. 次をクリック： **ログ** 」ボタンをクリックし、エラーがないことを確認します。 すべての検証手順、警告およびエラーが表示されます。色付きのアイコンは、メッセージタイプを示します。

   * 灰色のアイコンは、情報メッセージを示します。
   * 黄色のアイコンは、重要でない処理エラーを示します。
   * 赤色のアイコンは、配信の送信を妨げる重大なエラーを示します。

1. 変更を加えた後、準備を再開します。

準備が完了したら、メッセージを送信する準備が整います。 詳しくは、送信の確認を参照してください。


## メッセージの送信

準備が完了したら、次の手順に従ってメッセージを送信します。

1. 次をクリック： **送信ボタン** をクリックし、確定します。

1. 送信の進行状況は、次の 3 つの KPI と共に表示されます。配信済み、開封数、クリック数。

1. 「 OK 」ボタンをクリックして送信を完了します。

ログ

>[!NOTE]
>
>メッセージがスケジュールされている場合、送信時間に達すると送信されます。 メッセージのスケジュールについて詳しくは、この節を参照してください。

