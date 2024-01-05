---
audience: end-user
title: サービスのサブスクライバーを管理
description: Adobe Campaign Web で、サービスのサブスクライバーに対して管理および配信する方法を学ぶ
badge: label="ベータ版"
exl-id: cf72d27e-365c-4edc-b661-a67c148f0eeb
source-git-commit: cd7e2bb325b4e571018a8e04ffa0eaef74fe6768
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 100%

---

# サービスのサブスクライバーを管理 {#manage-subscribers}

「[サービスを作成](manage-services.md#create-service)」したら、サブスクライバーを追加したり、受信者を登録解除したり、そのサービスのサブスクライバーにメッセージを送信したりできます。

サブスクライバー管理について詳しくは、このページを参照してください。サブスクライバーにメッセージを送信する方法については、[この節](../msg/send-to-subscribers.md)を参照してください

## サブスクライバーをサービスに追加 {#add-subscribers}

サブスクライバーを手動で追加するには、次の手順に従います。

1. **[!UICONTROL サブスクライバーサービス]**&#x200B;リストから既存のサービスを選択します。

1. 「**[!UICONTROL サブスクライバー]**」タブを選択し、「**[!UICONTROL プロファイルを追加]**」をクリックします。

   ![](assets/service-subscribers-tab.png)

1. リストから追加するプロファイルを選択し、「**[!UICONTROL 確認]**」をクリックします。

   ![](assets/service-subscribers-select-profiles.png)

1. 「**[!UICONTROL 送信]**」をクリックします。<!--if you click cancel, does it mean that no message is sent but recipients are still subscribed, or they are not subscribed? it's 2 different actions in the console)-->[サービスを作成](manage-services.md#create-service)の際に選んだサブスクリプション[確認メッセージ](manage-services.md#create-confirmation-message)を、選択した受信者が受信します。

   ![](assets/service-subscribers-confirmation-msg.png)

追加されたプロファイルは、**[!UICONTROL サブスクライバー]**&#x200B;リストに表示されます。このプロファイルをサービスに登録しました。

## サービスからサブスクライバーを削除 {#remove-subscribers}

### 手動で受信者を登録解除 {#manual-unsubscription}

サービスに[サブスクライバーを追加](#add-subscribers)したら、それ各サブスクライバーを手動で登録解除できます。以下の手順に従います。

1. **[!UICONTROL サブスクリプションサービス]**&#x200B;リストから既存のサービスを選択します。

1. 目的の受信者名の横にある 3 つのドットのアイコンをクリックし、「**[!UICONTROL 削除]**」を選択します。

   ![](assets/service-subscribers-delete.png)

1. 「削除」を確認して、「**[!UICONTROL 送信]**」をクリックします。[サービスを作成](manage-services.md#create-service)の際に選んだ登録解除[確認メッセージ](manage-services.md#create-confirmation-message)を、選択した受信者が受信します。

   ![](assets/service-subscribers-delete-confirmation.png)

受信者が&#x200B;**[!UICONTROL サブスクリプション]**&#x200B;リストから削除され、サービスの登録が解除されました。

### 受信者を自動的に登録解除 {#automatic-unsubscription}

サブスクリプションサービスの期間を限定することができます。有効期間が終了すると、受信者は自動的に登録解除されます。

この期間は、[サービスの作成](manage-services.md#create-service)時に指定されます。「**[!UICONTROL その他のオプション]**」から、「**[!UICONTROL 無制限の有効期間]**」オプションを選択し、サービスの有効期間を定義します。

![](assets/service-create-validity-period.png)

指定された期間が終了すると、すべてのサブスクライバーがそのサービスから自動的に登録解除されます。
