---
audience: end-user
title: Adobe Experience Manager での多言語メールの作成
description: Campaign Web で Adobe Experience Manager の言語コピーを使用して、多言語メール配信を作成する方法を説明します。
feature: Email
topic: Content Management
role: User
level: Intermediate
exl-id: 6fc6ff43-ac7f-46c7-aa1a-9489ffc45423
TQID: https://experienceleague.adobe.com/t7jTgugTG9NOGwqQ9OMcRCrLcr83sTI5cu-O-iYQsRk
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2:
  - id: d5ef99fa-df0c-4153-bf94-105ad0724167
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 5a231f1dc49379d1be5d36e1732660111f851649
workflow-type: ht
source-wordcount: 527
ht-degree: 100%

---

# Adobe Experience Manager での多言語メールの作成 {#aem-multilingual}

Adobe Experience Manager との統合により、Adobe Experience Manager の言語コピーを使用して、多言語メール配信を作成できます。これにより、様々な言語でコンテンツのバリアントを管理し、受信者の言語設定に基づいて、パーソナライズされたメールを配信することができます。

## 前提条件 {#prerequisites}

多言語メール配信を作成する前に、次のことを確認してください。

* Adobe Campaign Web インターフェイス統合用に設定された、Adobe Experience Manager インスタンスへのアクセス。
* Adobe Experience Manager のコンテンツと、すでに作成および承認されている言語コピー。言語コピーウィザードについて詳しくは、[Adobe Experience Manager ドキュメント](https://experienceleague.adobe.com/ja/docs/experience-manager-cloud-service/content/sites/administering/reusing-content/translation/wizard)を参照してください
* Adobe Experience Manager コンテンツを受信するように設定されたメール配信テンプレート。[多言語モードを有効にする](#enable-multilingual)セクションで、詳細な手順を参照してください。

## 多言語配信を作成

多言語メール配信を作成するには、まず配信設定で多言語オプションを有効にする必要があります。システムによって使用可能な言語コピーが自動的に検出され、追加する言語コピーを選択できます。

### 多言語モードを有効にする {#enable-multilingual}

新しい配信を作成し、詳細設定で多言語オプションを有効にします。

1. **[!UICONTROL 配信]**&#x200B;メニューで、「**[!UICONTROL 配信を作成]**」をクリックします。

   ![](assets/lg-copy-1.png)

1. 「**[!UICONTROL AEM コンテンツでメール配信]**」テンプレートを選択し、「**[!UICONTROL 配信を作成]**」をクリックします。

   ![](assets/lg-copy-2.png)

1. 配信のラベルを入力し、オーディエンスを設定します。[詳細情報](../email/create-email.md)

1. 配信&#x200B;**[!UICONTROL 設定]**&#x200B;にアクセスし、「**[!UICONTROL 詳細]**」セクションに移動します。

1. 「**[!UICONTROL AEM Multilingual を有効化]**」オプションを有効にします。

   ![](assets/lg-copy-3.png)

1. 次のことを確認します。

   * 「**[!UICONTROL コンテンツ編集モード]**」が「**[!UICONTROL AEM]**」に設定されている。
   * 適切な Adobe Experience Manager の&#x200B;**[!UICONTROL 外部アカウント]**&#x200B;が選択されている。

1. 「**[!UICONTROL 保存して閉じる]**」をクリックします。

### コンテンツバリアントを作成 {#create-variants}

Adobe Experience Manager のコンテンツを選択し、配信に含める言語のバリアントを選択します。

1. 「**[!UICONTROL コンテンツを編集]**」をクリックします。

1. 「**[!UICONTROL コンテンツバリアントを作成]**」を選択します。

   ![](assets/lg-copy-4.png)

1. リストから Adobe Experience Manager コンテンツを選択します。

   ![](assets/lg-copy-5.png)

1. システムにより、選択したコンテンツ（親子関係）に関連付けられたすべての言語コピーが検出されます。例えば、Adobe Experience Manager コンテンツにフランス語、ドイツ語、イタリア語のバリアントがある場合、すべてのバリアントを選択できます。

   配信に含める言語のバリアントを選択します。

   ![](assets/lg-copy-6.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

1. コンテンツエディターで言語のバリアントを確認します。各バリアントを[個別に管理](#manage-variants)するか、[配信の送信](../monitor/prepare-send.md)に進むことができます。

   ![](assets/lg-copy-7.png)

## 言語バリアントの管理 {#manage-variants}

コンテンツのバリアントを作成したら、配信でそれらを直接管理できます。

1. デフォルトの言語を設定するには、選択したバリアントの詳細メニューにアクセスし、「**[!UICONTROL デフォルトとして設定]**」を選択します。デフォルトの言語は、プロファイルの言語設定が設定されていないか、使用可能なバリアントと一致しない場合に使用されます。

   「**[!UICONTROL 削除]**」をクリックして、配信からバリアントを削除します。

   ![](assets/lg-copy-8.png)

1. コンテンツバリアントの詳細メニューで、「**[!UICONTROL ロケールを管理]**」をクリックして、配信に他のロケールを追加します。

   ![](assets/lg-copy-9.png)

1. さらに多くのバリアントを含めるには、追加の言語コピーを選択し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/lg-copy-11.png)

1. Adobe Experience Manager でコンテンツが更新された場合は、「**[!UICONTROL AEM コンテンツを更新]**」をクリックして、すべてのバリアントを最新バージョンと同期します。

   ![](assets/lg-copy-10.png)

1. Campaign で直接コンテンツを編集する場合や、Adobe Experience Manager とのリンクを解除する場合は、「**[!UICONTROL AEM コンテンツをリンク解除]**」をクリックします。

   >[!CAUTION]
   >
   >リンクを解除すると、Adobe Experience Manager からコンテンツを更新したり、新しいバリアントを作成したりできなくなります。コンテンツは Adobe Experience Manager から独立します。
