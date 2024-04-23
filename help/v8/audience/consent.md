---
audience: end-user
title: 同意
description: Adobe Campaign Web での同意について説明します
badge: label="限定提供（LA）"
source-git-commit: 9a184d7558ca39be3afed4a7217a5e5687799c0d
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 13%

---

# 同意の管理 {#manage-consent}

## 一般的なレコメンデーション {#general-recommendations}

Adobe Campaign を使用すると、個人情報や機密情報などのデータを収集できます。したがって、GDPR （一般データ保護規則）やその他の適用されるプライバシー法などのデータ保護規則に従って、受信者の同意を取得および監視することが不可欠です。

* まず第一に、未承諾のメール、プッシュ通知、SMS メッセージ（「スパム」）を送信しないようにします。 Adobeでは、顧客の生涯価値およびロイヤルティを促進するうえで許可型マーケティングの原則を重視しています。したがって、未承諾メッセージの送信にAdobe Campaignを使用することを固く禁止しています。 [詳細情報](#denylisted-profiles)

* 受信者は、配信をオプトアウトする機能を提供することで、コミュニケーションの受信に常に同意するようにします<!-- and keep honoring opt-out requests as quickly as possible-->. [詳細情報](#opt-out)

* 購読管理プロセスを使用すると、受信者の環境設定を管理し、どの受信者がどのタイプの購読にオプトインしたかを追跡できます。 [詳細情報](../../delivery/using/about-services-and-subscriptions.md)

## オプトアウトの管理 {#opt-out}

ブランドからの連絡を登録解除する機能を受信者に提供することは、法的要件であり、この選択を確実に行うためにも必要です。 <!--Learn more about the applicable legislation in the [Adobe Campaign Classic v7 documentation](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/privacy/privacy-and-recommendations.html#privacy-regulations){target="_blank"}.-->

**なぜそれが重要なのでしょうか？**

* これらの規制に準拠できないと、ブランドに法規制上のリスクが生じます。
* この機能を使用すると、未承諾の通信を受信者に送信して、メッセージがスパムと見なされたり、評判が損なわれたりする危険性を避けることができます。

Adobe Campaign Web を使用して配信を送信する場合は、顧客が今後の通信を登録解除できるようにする必要があります。 登録解除すると、プロファイルは、今後のマーケティングメッセージのオーディエンスから自動的に削除されます。

### メールオプトアウト {#email-opt-out}

メール配信を登録解除できる機能を受信者に提供するには、必ず以下を含める必要があります。 **購読解除リンク** 受信者に送信されるすべてのメールで。

それには、次の手順に従います。

1. 外部ランディングページを作成し、選択したサードパーティシステムでホストします。

1. メール配信を作成します。 [詳細情報](../email/create-email.md)

1. メールコンテンツへのリンクを挿入します。 [詳細情報](../email/message-tracking.md#insert-links)

   ![](../email/assets/message-tracking-insert-link.png)

1. が含まれる **[!UICONTROL Url]** フィールドに、サードパーティ製のランディングページへのリンクを貼り付けます。

1. 左側のパネルで 「**[!UICONTROL リンク]**」アイコンをクリックすると、追跡するコンテンツのすべての URL のリストが表示されます。

1. 新規リンクの横にある鉛筆アイコンをクリックして編集します。

1. を変更する **[!UICONTROL トラッキングタイプ]** およびを設定します **[!UICONTROL オプトアウト]**.

   ![](../email/assets/message-tracking-edit-a-link.png)

1. クリック **[!UICONTROL 保存]** メッセージを送信します。 [詳細情報](../monitor/prepare-send.md)

1. メッセージを受け取った受信者が購読解除リンクをクリックすると、ランディングページが表示されます。

1. 受信者がランディングページフォームを送信すると、プロファイルデータが更新されます。 [詳細情報](#denylisted-profiles)

<!--Any other option availabe such as one-click opt-out link or List-Unsubscribe (to include an unsubscribe link in the email header) to enable opt-out in a delivery?-->

## ブロックリストに加えるプロファイル {#denylisted-profiles}

購読解除（オプトアウト）後、プロファイルは **ブロックリスト** 特定のチャネルの場合：これは、配信のターゲットとならなくなったことを意味します。

>[!NOTE]
>
>メールチャネルのブロックリスト上のプロファイルに 2 つのメールアドレスがある場合、両方のアドレスが配信から除外されます。

プロファイルがチャネル内の 1 つ以上のブロックリストに登録されているかどうかを **[!UICONTROL 今後の連絡先]** プロファイルののセクション **[!UICONTROL 詳細]** タブ。 [詳細情報](../audience/about-recipients.md#access)

![](assets/profile-no-longer-contact.png)

<!--Denylisted status on quarantine list

Additionally, when recipients report your message as spam, or reply to an SMS message with a keyword such as "STOP", their address or phone number is quarantined with the **[!UICONTROL Denylisted]** status. Their profile is updated accordingly.

QUESTION: When a user marks an email as spam, is the profile's No longer contact section also updated? Apparently no (not the same = quarantine vs denylist)

>[!NOTE]
>
>The **[!UICONTROL Denylisted]** status refers to the address only, the profile is not on the denylist, so that the user continues receiving SMS messages and push notifications.

Learn more about Feedback loops in the [Delivery Best Practices Guide](https://experienceleague.adobe.com/docs/deliverability-learn/deliverability-best-practice-guide/transition-process/infrastructure.html#feedback-loops){target="_blank"}.

Learn more on quarantine in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html#non-deliverable-bounces){target="_blank"}.-->



