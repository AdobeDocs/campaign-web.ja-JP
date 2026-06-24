---
title: 外部アカウントの管理
description: 外部アカウントの設定方法について説明します
exl-id: 99648377-112b-428a-8faf-5268d730f19a
TQID: https://experienceleague.adobe.com/ZkfG6g4YYAkefJI1Pi7xsdulm1zS1BFJdXBTS37x2T8
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 5a231f1dc49379d1be5d36e1732660111f851649
workflow-type: ht
source-wordcount: 213
ht-degree: 100%

---

# Adobe ソリューション統合外部アカウント {#integration-external-account}

選択したアドビソリューション統合外部アカウントのタイプに応じて、次の手順に従って、アドビサービスとのシームレスな統合を行う接続とアカウント設定を指定します。

## Adobe Experience Cloud

Adobe ID を使用して Adobe Campaign コンソールに接続するには、Adobe Experience Cloud（MAC）外部アカウントを設定する必要があります。

![Adobe Experience Cloud MAC 外部アカウント設定フィールドを示すスクリーンショット。](assets/external-MAC.png)

**[!UICONTROL Adobe Experience Cloud]** 外部アカウントを設定するには、次のフィールドに入力します。

* **[!UICONTROL IMS サーバー]**

  IMS サーバーの URL。 また、ステージングと本番用のインスタンスがいずれも、同じ IMS 本番エンドポイントを指していることを確認します。

* **[!UICONTROL IMS スコープ]**

  スコープは、IMS によりプロビジョニングされているスコープのサブセットでなければなりません。

* **[!UICONTROL IMS クライアント識別子]**

  IMS クライアントの ID。

* **[!UICONTROL IMS クライアント秘密鍵]**

  IMS クライアント秘密鍵の資格情報。

* **[!UICONTROL コールバックサーバー]**

  Adobe Campaign インスタンスのアクセス URL。

* **[!UICONTROL IMS 組織 ID]**

  組織の ID。 組織 ID を見つけるには、[このページ](https://experienceleague.adobe.com/docs/core-services/interface/administration/organizations.html?lang=ja){target=_blank}を参照してください。

* **[!UICONTROL 関連付けマスク]**

  このフィールドでは、Enterprise Dashboard の設定名を Adobe Campaign のグループと同期させる構文を定義することができます。

* **[!UICONTROL サーバー]**

  Adobe Experience Cloud インスタンスの URL。

* **[!UICONTROL テナント]**

  Adobe Experience Cloud テナントの名前。
