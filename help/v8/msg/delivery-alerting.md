---
audience: end-user
title: 配信アラート
description: 配信アラートの操作方法を説明します。
exl-id: 120afaa0-7017-4644-b6db-229b4a5c8a91
source-git-commit: bb61fdb34fecb4131d4069965cda8a3a5099b6bc
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 2%

---

# 配信アラートの基本を学ぶ {#gs-delivery-alerting}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="配信アラート"
>abstract="Campaign で配信アラートが使用できるようになりました。 この機能は、ユーザーのグループが、配信の実行に関する情報を含んだメール通知を自動的に受信できるようにするアラート管理システムです。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=ja" text="リリースノートを参照してください"

配信アラートは、ユーザーのグループが配信実行に関する情報を含んだメール通知を自動的に受信できるようにするアラート管理システムです。 受信者は、Adobe Campaignで処理される進行中の配信をモニタリングし、問題が発生した場合は適切なアクションを実行できます。

通知は、Adobe Campaign web ユーザーインターフェイスで定義された特定のアラート条件に基づいてカスタマイズできます。

配信エラーの管理方法について詳しくは、を参照してください。 [Adobe Campaign v8 （コンソール）ドキュメント](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/delivery-failures#send){target="_blank"}

## メール通知コンテンツ {#content}

メール通知には、次のセクションが含まれます。

* **概要**：定義した条件に一致する配信数が、条件ごとのラベルとカラーで表示されます。
* **詳細**：ダッシュボードに対して定義されているすべての配信条件と、条件ごとに対応する配信をリストします。

![](assets/alerting-email.png)

## 配信アラートの設定 {#set-up}

これらのアラートの設定に役立つように、Campaign web ユーザーインターフェイスでは、以下の項目を作成および管理できます。

* **配信アラートダッシュボード**：受信者を指定し、ダッシュボードに含めるアラート条件を設定し、送信されたアラートの履歴にアクセスします。 [ダッシュボードの操作方法を学ぶ](../msg/delivery-alerting-dashboards.md)
* **配信アラート条件**:Campaign web ユーザーインターフェイスには、ダッシュボードに追加できる事前定義済みのアラート条件（スループットの低い配信、準備に失敗した配信など）が用意されています。 また、ニーズに合わせて独自の条件を作成することもできます。 [条件の操作方法を学ぶ](../msg/delivery-alerting-criteria.md)

例えば、管理権限を持つユーザーには失敗した配信についてのみ通知し、マーケティングユーザーにはソフトバウンスエラー率が高い配信について通知するとします。 これを実現するには、受信者のグループごとに適切な条件を持つ 2 つの個別のダッシュボードを作成します。

>[!NOTE]
>
>ダッシュボードとアラート条件にアクセスして設定するには、次の情報が必要です **管理権限** または、 **配信スーパーバイザー** セキュリティグループ。 標準ユーザーは、Adobe Campaign インターフェイスのダッシュボードにアクセスできませんが、アラート通知を受信できます。 [アクセスと権限の詳細を学ぶ](../get-started/permissions.md)
