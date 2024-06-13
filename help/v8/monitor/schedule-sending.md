---
audience: end-user
title: 配信の送信のスケジュール設定
description: 配信をスケジュール設定する方法について説明します
exl-id: 0738a148-d550-41c2-a8c2-6054684ba789
source-git-commit: 89633454bb3de1ac05d37d767df45d9d143c80b5
workflow-type: ht
source-wordcount: '514'
ht-degree: 100%

---

# 配信の送信のスケジュール設定 {#schedule-sending}

配信の送信をスケジュール設定できます。この手順は、スタンドアロン（1 回限りの）配信であるか、キャンペーンワークフローのコンテキストで作業しているかによって異なります。

## スタンドアロン配信

スタンドアロン配信の場合は、配信の日時を直接スケジュール設定できます。
各配信タイプ（メール、SMS、プッシュ通知）の例については、以下を参照してください。

### メール {#schedule-email-standalone}

メール配信の送信をスケジュール設定するには、次の手順に従います。

1. 配信プロパティの「**[!UICONTROL スケジュール]**」セクションで、「**[!UICONTROL スケジュールを有効にする]**」切替スイッチをオンにします。

1. 送信する日時を設定し、「**[!UICONTROL 確認して送信]**」ボタンをクリックします。

   ![](assets/schedule-email-standalone.png){zoomable="yes"}

>[!NOTE]
>
>デフォルトでは、「**[!UICONTROL 送信前に確認を有効にする]**」オプションが有効になっています。このオプションでは、スケジュール設定した日時に配信を送信する前に送信を確定する必要があります。スケジュール設定した日時に&#x200B;**配信を自動的に送信**&#x200B;する必要がある場合は、このオプションを無効にする必要があります。
>

1. スケジュールが正しいことを確認して、「**[!UICONTROL 準備]**」ボタンをクリックします。

![](assets/schedule-email-standalone-prepare.png){zoomable="yes"}

1. 準備が完了すると、メッセージを送信する準備が整います。配信の主要指標（ターゲット母集団の合計、配信するメッセージの数、除外された受信者の数）が表示されます。「**[!UICONTROL スケジュールどおりに送信]**」ボタンをクリックして、スケジュール設定した日時にメインターゲットに配信を送信できることを確認します。

![](assets/schedule-email-standalone-send.png){zoomable="yes"}


### SMS

SMS 配信を特定の日時にスケジュール設定する手順は、メール配信と同じです（[上記を参照](#schedule-email-standalone)）。

![](assets/schedule-sms-standalone.png){zoomable="yes"}

また、スケジュールが考慮されていることを確認することもできます。

![](assets/schedule-sms-standalone-prepare.png){zoomable="yes"}

### プッシュ通知

スタンドアロンのプッシュ配信を特定の日時にスケジュール設定する手順は、メール配信と同じです（[上記を参照](#schedule-email-standalone)）。

![](assets/schedule-push-standalone.png){zoomable="yes"}

また、スケジュールが考慮されていることを確認することもできます。

![](assets/schedule-push-standalone-prepare.png){zoomable="yes"}

### キャンペーンでのスタンドアロン配信

ワークフローを使用せずに、キャンペーン内にスタンドアロン配信を作成できます。上記の説明に従って、この配信の日時スケジュールを設定できます。
キャンペーンには、開始日と終了日を含むスケジュールが設定されている場合があります。このスケジュールが配信スケジュールに干渉することはありません。

![](assets/schedule-delivery-standalone.png){zoomable="yes"}

## キャンペーンワークフローでの配信のスケジュール設定

キャンペーンワークフローのコンテキストでは、**ベストプラクティス**&#x200B;として、**[!UICONTROL スケジューラー]**&#x200B;アクティビティを使用して、配信の送信を含むワークフローを開始する日時を適用することをお勧めします。[スケジューラーの詳細](../workflows/activities/scheduler.md)

![](assets/schedule-workflow.png){zoomable="yes"}


**[!UICONTROL スケジューラー]**&#x200B;アクティビティで日時を設定する必要があります。

![](assets/schedule-workflow-scheduler.png){zoomable="yes"}


>[!NOTE]
>
>**[!UICONTROL スケジューラー]**&#x200B;アクティビティを使用してワークフローで配信の送信をスケジュール設定する場合は、**[!UICONTROL 配信]**&#x200B;アクティビティ設定で「**[!UICONTROL スケジュールを有効にする]**」切替スイッチを&#x200B;**オンにしないでください**。配信は自動的に送信されます。
>

**[!UICONTROL 配信]**&#x200B;アクティビティ設定で「**[!UICONTROL スケジュールを有効にする]**」切替スイッチをオンにし、そこで日時を設定すると、配信はこの日時に送信されるまで待機します。つまり、ワークフローの開始日と送信日の間に遅延がある場合、オーディエンスが最新でない可能性があります。
