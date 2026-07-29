---
title: ブランディング
description: ブランドの設定方法について説明します。
audience: administration
context-tags: branding,overview;branding,main
role: Admin
level: Experienced
exl-id: 7afc802d-e90c-48c8-aa04-3ea543dfdfbc
source-git-commit: 5c9d3db95905f77dddffaf824156c87b9d79013c
workflow-type: tm+mt
source-wordcount: '809'
ht-degree: 37%

---

# ブランドの設定 {#branding-configure}

技術管理者は、Web UIから複数のブランドを直接作成および管理できます。 これにより、ロゴやメールトラッキング設定など、ブランドアイデンティティを設定するすべての要素を定義できます。

>[!NOTE]
>
>この機能を使用するには、インスタンス上のブランディングパッケージが必要です。 **Branding** メニューが表示されない場合は、Adobe担当者にお問い合わせください。

## ブランドの作成または編集 {#create-edit-brand}

>[!CONTEXTUALHELP]
>id="acw_branding_create"
>title="ブランドの構築"
>abstract="「**ブランドを作成**」をクリックして、新しいブランドアイデンティティを定義します。 設定タブでブランドの詳細を入力し、**ブランドを作成**&#x200B;をクリックして保存します。 ブランドは、配信テンプレートとスタンドアロン配信にリンクできるようになります。"

新しいブランドを作成するには、次の手順に従います。

1. 左側のメニューから&#x200B;**[!UICONTROL 管理/ ブランディング]**&#x200B;に移動するか、**[!UICONTROL エクスプローラー]**&#x200B;から&#x200B;**[!UICONTROL 管理/ プラットフォーム / ブランディング]**&#x200B;に移動します。

1. リストの上にある「**[!UICONTROL ブランドを作成]**」ボタンをクリックします。

   ブランド作成を示す![ スクリーンショット ](assets/branding-create.png)

1. さまざまなセクションにブランドの詳細を入力します。 各フィールドについては、以下の「[ ブランド属性](#brand-attributes)」セクションで説明します。

   ブランド作成フィールドを示す![ スクリーンショット ](assets/branding-create2.png)

1. 「**[!UICONTROL ブランドを作成]**」をクリックして保存します。 ブランドは、配信テンプレートとスタンドアロン配信にリンクできるようになりました。 [ ブランドの割り当て方法を学ぶ](branding-assign.md)。

既存のブランドを編集するには、リストからブランドを選択し、フィールドを更新して、変更を保存します。

## ブランド属性 {#brand-attributes}

**[!UICONTROL ブランド]**&#x200B;は、4つのセクションに分けて設定されています：**[!UICONTROL ID]**、**[!UICONTROL ブランド設定]**、**[!UICONTROL メールヘッダーパラメーター]**、および&#x200B;**[!UICONTROL URL トラッキングパラメーター]**。

### ID {#identity}

「**[!UICONTROL ID]**」セクションでは、ブランドを定義およびパーソナライズできます。

ブランド作成時に「ID」タブを表示する![ スクリーンショット ](assets/branding-create3.png)

このセクションには、次のフィールドが含まれています。

* **[!UICONTROL ブランド名]**：ブランドの名前。 このフィールドは必須です。
* **[!UICONTROL Label]**: インターフェイスに表示されるラベル。
* **[!UICONTROL ID]**：内部識別子が自動的に生成されます。 それを変更することができます。 英数字とアンダースコアのみ使用できます。 特殊文字はアンダースコアに置き換えられます。
* **[!UICONTROL ロゴ URL]**: ブランドロゴ画像のURL。
* **[!UICONTROL Web サイト URL]**&#x200B;および&#x200B;**[!UICONTROL Web サイト ラベル]**：ブランドに関連付けられているweb サイト URLとラベル。


### ブランド設定 {#brand-configs}

「**[!UICONTROL ブランド設定]**」セクションでは、トラッキングとランディングページへのアクセスに使用するサブドメインとURL プロトコルを定義します。

「ブランド設定」タブを表示する![ スクリーンショット ](assets/branding-create4.png)

このセクションには、次のフィールドが含まれています。

* **[!UICONTROL ブランドサブドメイン]**：このブランドに固有のサブドメイン URLで、Adobeからの委任を要求されています。
* **[!UICONTROL トラッキング URL プロトコル]**、**[!UICONTROL ミラーページ URL プロトコル]**、および&#x200B;**[!UICONTROL アプリケーション URL プロトコル]**：各URL タイプに使用されるプロトコル（**セキュア （https）**&#x200B;など）。

>[!NOTE]
>
>トラッキング、ミラー、およびアプリケーションサーバーの設定は、ルーティングに関連付けられた個別の外部アカウントに保存されます。 これらの設定は、プロビジョニング中に適用されるので、変更しないでください。 URL を表示するには、外部アカウントから「**[!UICONTROL ブランディングプレフィックス]**」タブにアクセスします。

### メールヘッダーのパラメーター {#header-param}

**[!UICONTROL メールヘッダーパラメーター]**&#x200B;を使用すると、キャンペーンのヘッダーセクションに表示される受信者の内容をパーソナライズできます。

![電子メールヘッダーフィールドを含む「ヘッダーパラメーター」タブを示すスクリーンショット ](assets/branding-create5.png)

このセクションには、次のフィールドが含まれています。

* **[!UICONTROL 送信者（メールアドレス）]**：ブランドのメールアドレス。
* **[!UICONTROL 送信者（名前）]**：ブランド名。
* **[!UICONTROL 返信先（電子メールアドレス）]**：お客様が返信できる電子メールアドレス。
* **[!UICONTROL 返信先（名前）]**：返信の表示名。
* **[!UICONTROL エラー（電子メールアドレス）]**：エラーが発生した場合に使用する電子メールアドレス。

<!--
>[!IMPORTANT]
>
>After having updated the header parameters of the emails, if the name and email address of the sender have not changed in the email created from the template, check the template's advanced settings.
-->

### URL トラッキングパラメーター {#tracking-param}

**[!UICONTROL URL トラッキングパラメーター]** セクションでは、Adobe AnalyticsやGoogle AnalyticsなどのWeb分析ツールと統合するためのパラメーターを追加してURL トラッキングを強化できます。

「ヘッダーパラメーター」タブにURL トラッキングパラメーターを表示する![ スクリーンショット ](assets/branding-create6.png)

このセクションには、次のフィールドが含まれています。

* **[!UICONTROL 追加のURL パラメーター]**: パラメーターをキーと値のペアとして、適用条件とともに追加します。 各パラメーター名は一意で空でない必要があり、各パラメーター値は空でない必要があります。 適用条件は空にすることができますが、これらの値には JST タグを含めることはできません。

* **[!UICONTROL ドメイン名allow-list]**：トラッキングパラメーターが追加されるURLに一致するように、ドメイン名または正規表現を追加します。

**例：**`https://www.luma.com` のようなトラッキング対象 URL は、そのドメインに追加パラメーター `age=21` および `deliveryName=DM101` が設定されている場合は `https://www.luma.com/?age=21&deliveryName=DM101` になります。

## トランザクションメッセージのブランディングの設定 {#branding-transactional-config}

>[!IMPORTANT]
>
>この節は、トランザクションメッセージ（Message Center）にのみ適用されます。
>
>トランザクション機能は Campaign web UI で使用できますが、以下の手順は Campaign v8 クライアントコンソール（コントロールインスタンス）で実行する必要があります。

ブランディングにトランザクションメッセージ（Message Center）を使用している場合は、追加の設定が必要です。

### リアルタイムインスタンスのトラッキング式

リアルタイム（RT）コントロールインスタンスでブランディングをアクティブ化すると、トラッキング式を管理する特定のトラッキングオプションが使用されます。 これらの式は、各 RT 実行インスタンスで個別に設定するのではなく、RT コントロールインスタンスで一元的に設定されます。

次のオプションは、RT 配信で使用されるトラッキング式を定義します。

* **`NmsTracking_RT_ClickFormula`**：RT インスタンスのクリックの追跡に使用される式を指定します

* **`NmsTracking_RT_OpenFormula`**：RT インスタンスの開封トラッキングに使用される式を指定します

実装でトランザクションメッセージのカスタムトラッキング式が必要な場合は、以下のオプションを使用します。

* **`Branding_RT_ListXtkOptions_toPublish`**：カスタム式の XTK オプション名をここにリストします（コンマで区切ります）。 これにより、RT 配信でカスタムトラッキング式を適用できます。
