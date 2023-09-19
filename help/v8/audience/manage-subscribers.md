---
audience: end-user
title: サービスの購読者の管理
description: Adobe Campaign Web でサービスの購読者に管理して配信する方法を説明します
badge: label="Beta"
source-git-commit: 5125de258edd4e3eda9a8507228156ee40215532
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 0%

---


# サービスの購読者の管理 {#manage-subscribers}

一度 [サービスを作成しました](manage-services.md#create-service)を使用すると、購読者を追加したり、受信者を購読解除したり、そのサービスの購読者に配信したりできます。

## サービスへの購読者の追加 {#add-subscribers}

購読者を手動で追加するには、次の手順に従います。

1. 次の中から既存のサービスを選択します： **[!UICONTROL 購読サービス]** リスト。

1. を選択します。 **[!UICONTROL 購読者]** タブをクリックし、 **[!UICONTROL プロファイルを追加]**.

   ![](assets/service-subscribers-tab.png)

1. リストから追加するプロファイルを選択し、 **[!UICONTROL 確認]**.

   ![](assets/service-subscribers-select-profiles.png)

1. クリック **[!UICONTROL 送信]**.<!--if you click cancel, does it mean that no message is sent but recipients are still subscribed, or they are not subscribed? it's 2 different actions in the console)--> 選択した受信者が購読を受け取ります [確認メッセージ](manage-services.md#create-confirmation-message) 選択した日時 [サービスの作成](manage-services.md#create-service).

   ![](assets/service-subscribers-confirmation-msg.png)

追加されたプロファイルは、「 **[!UICONTROL 購読者]** リスト。 これで、サービスが購読されました。

## サービスから購読者を削除する {#remove-subscribers}

### 手動で受信者を購読解除 {#manual-unsubscription}

一度 [追加購読者](#add-subscribers) をサービスに追加すると、それぞれを手動で購読解除できます。 次の手順に従います。

1. 次の中から既存のサービスを選択します： **[!UICONTROL 購読サービス]** リスト。

1. 目的の受信者名の横にある 3 つのドットのアイコンをクリックし、「 」を選択します。 **[!UICONTROL 削除]**.

   ![](assets/service-subscribers-delete.png)

1. 削除を確定し、「 **[!UICONTROL 送信]**. 選択した受信者が購読解除を受け取ります [確認メッセージ](manage-services.md#create-confirmation-message) 選択した日時 [サービスの作成](manage-services.md#create-service).

   ![](assets/service-subscribers-delete-confirmation.png)

受信者が **[!UICONTROL 購読者]** リストに登録され、サービスの購読登録が解除されました。

### 受信者を自動的に配信停止 {#automatic-unsubscription}

サブスクリプションサービスの期間を限定できます。 有効期間が終了すると、受信者は自動的に購読解除されます。

この期間は、 [サービスの作成](manage-services.md#create-service). 次から： **[!UICONTROL その他のオプション]**、無効 **[!UICONTROL 無制限の有効期間]** 」オプションを選択し、サービスの有効期間を定義します。

![](assets/service-create-validity-period.png)

指定された期間が終了すると、すべての購読者がそのサービスから自動的に購読解除されます。

## サービスの購読者への配信

一度 [購読サービスを作成しました](manage-services.md#create-service)を使用すると、配信の購読者をターゲットに設定できます。 次の手順に従います。

1. [オーディエンスの作成](../audience/create-audience.md) 作成したサービスの購読者を含める：

   * Adobe Analytics の **[!UICONTROL オーディエンスの構築]** アクティビティ、詳細属性の表示および選択 **[!UICONTROL 受信者]** > **[!UICONTROL 購読]** > **[!UICONTROL サービス]**.

   * この例では、 **Luma ニュースレター** ラベル。

   ![](assets/service-audience-subscribers.png)

1. [配信の作成](../msg/gs-messages.md#create-delivery) をクリックし、上で作成したオーディエンスを選択します。

   ![](assets/service-delivery-targeting-subscribers.png)

1. 必要に応じてメッセージコンテンツを編集し、配信を送信します。

   ![](assets/service-delivery-ready.png)

配信は、そのサービスの購読者にのみ送信されます。
