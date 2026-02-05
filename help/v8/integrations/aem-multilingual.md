---
audience: end-user
title: Adobe Experience Managerでの多言語メールの作成
description: Campaign web でAdobe Experience Managerの言語コピーを使用して、多言語メール配信を作成する方法について説明します。
feature: Email
topic: Content Management
role: User
level: Intermediate
source-git-commit: f772e19fd033b007680777f75b48775b6d7851b9
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 3%

---


# Adobe Experience Managerでの多言語メールの作成 {#aem-multilingual}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn3"
>title="Experience Managerのライブコピーと言語コピー"
>abstract="Adobe Experience Manager言語とライブコピーに Campaign で直接アクセスできるようになりました。 リアルタイムのコンテンツ更新により、手動での同期が不要になり、複数の言語を使用したワークフローが合理化されます。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=ja" text="リリースノートを参照してください"

Adobe Experience Manager統合を使用すると、Adobe Experience Managerの言語コピーを使用して多言語のメール配信を作成できます。 これにより、様々な言語のコンテンツのバリアントを管理し、受信者の言語の環境設定に基づいてパーソナライズされたメールを配信できます。

## 前提条件 {#prerequisites}

多言語メール配信を作成する前に、次のことを確認します。

* Adobe Campaign Web インターフェイス統合用に設定されたAdobe Experience Manager インスタンスにアクセスします。
* 言語コピーが作成済みおよび承認済みのAdobe Experience Manager コンテンツ。 言語コピーウィザードについて詳しくは、[Adobe Experience Manager ドキュメントを参照してください ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/sites/administering/reusing-content/translation/wizard)
* Adobe Experience Manager コンテンツを受信するように設定されたメール配信テンプレート。 [ 多言語モードの有効化 ](#enable-multilingual) の節で説明されている手順を参照してください。

## 多言語配信の作成

多言語メール配信を作成するには、まず配信設定で多言語オプションを有効にする必要があります。 使用可能な言語コピーが自動的に検出され、追加する言語コピーを選択できます。

### 多言語モードの有効化 {#enable-multilingual}

新しい配信を作成し、詳細設定で多言語オプションを有効にします。

1. **[!UICONTROL 配信]** メニューから、「**[!UICONTROL 配信を作成]**」をクリックします。

   ![](assets/lg-copy-1.png)

1. **[!UICONTROL AEM コンテンツでメール配信]** テンプレートを選択し、「**[!UICONTROL 配信を作成]**」をクリックします。

   ![](assets/lg-copy-2.png)

1. 配信のラベルを入力し、オーディエンスを設定します。 [詳細情報](../email/create-email.md)

1. 配信 **[!UICONTROL 設定]** にアクセスし、「**[!UICONTROL 詳細]** セクションに移動します。

1. 「**[!UICONTROL AEMの多言語を有効にする]** オプションを有効にします。

   ![](assets/lg-copy-3.png)

1. 次のことを確認します。

   * **[!UICONTROL コンテンツ編集モード]** が **[!UICONTROL AEM]** に設定されています。
   * 正しいAdobe Experience Manager **[!UICONTROL 外部アカウント]** が選択されています。

1. **[!UICONTROL 保存して閉じる]** をクリックします。

### コンテンツバリアントを作成 {#create-variants}

Adobe Experience Manager コンテンツを選択し、配信に含める言語のバリアントを選択します。

1. 「**[!UICONTROL コンテンツを編集]**」をクリックします。

1. 「**[!UICONTROL コンテンツバリアントを作成]**」を選択します。

   ![](assets/lg-copy-4.png)

1. リストからAdobe Experience Manager コンテンツを選択します。

   ![](assets/lg-copy-5.png)

1. 選択したコンテンツに関連付けられているすべての言語コピーが検出されます（親子関係）。例えば、Adobe Experience Managerのコンテンツにフランス語、ドイツ語、イタリア語のバリアントがある場合、すべてのバリアントを選択できます。

   配信に含める言語のバリアントを選択します。

   ![](assets/lg-copy-6.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

1. コンテンツエディターで言語のバリアントをレビューします。 これで [ 各バリアントを個別に管理 ](#manage-variants) するか、[ 配信の送信 ](../monitor/prepare-send.md) に進むことができます。

   ![](assets/lg-copy-7.png)

## 言語バリアントの管理 {#manage-variants}

コンテンツのバリアントを作成したら、配信内で直接管理できます。

1. デフォルトの言語を設定するには、選択したバリアントの詳細メニューにアクセスし、「**[!UICONTROL デフォルトとして設定]** を選択します。 デフォルトの言語は、プロファイルの言語の環境設定が設定されていない場合や、使用可能なバリアントと一致しない場合に使用されます。

   **[!UICONTROL 削除]** をクリックして、配信からバリアントを削除します。

   ![](assets/lg-copy-8.png)

1. コンテンツバリアントの詳細メニューで、「**[!UICONTROL ロケールを管理]**」をクリックして、配信に他のロケールを追加します。

   ![](assets/lg-copy-9.png)

1. 追加の言語コピーを選択してさらにバリアントを含め、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/lg-copy-11.png)

1. Adobe Experience Managerでコンテンツを更新する場合は、「**[!UICONTROL AEM コンテンツを更新]**」をクリックして、すべてのバリアントを最新バージョンに同期します。

   ![](assets/lg-copy-10.png)

1. コンテンツを Campaign で直接編集する場合や、AEMとのリンクを解除する場合は、「**[!UICONTROL Adobe Experience Manager コンテンツのリンクを解除]**」をクリックします。

   >[!CAUTION]
   >
   >リンクを解除した後は、Adobe Experience Managerのコンテンツを更新したり、新しいバリアントを作成したりすることはできません。 コンテンツがAdobe Experience Managerから独立します。


