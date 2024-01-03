---
title: プロファイルの監視と管理
description: Campaign Web でプロファイルを監視および管理する方法について説明します。
badge: label="限定提供（LA）"
source-git-commit: 41c38ff3b18c28fbcb6fd07dd398600a207f53cb
workflow-type: tm+mt
source-wordcount: '663'
ht-degree: 9%

---

# プロファイルの監視と管理 {#profiles}

>[!CONTEXTUALHELP]
>id="acw_homepage_rn4"
>title="プロファイルの 360 ビュー"
>abstract="新しいプロファイルを作成し、強力なレポートやツールを使用してそれらを監視します。 プロファイルの属性、インタラクションおよびログにアクセスします。 フィルターオプションを使用して、プロファイルのリストを参照し、プロファイルを編集および更新します。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html" text="リリースノートを参照"

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="プロファイル"
>abstract="プロファイルとは、Adobe Campaign から送信されるメッセージの受信対象となる個人です。このリストから、権限に基づいてプロファイルの詳細を表示できます。 フィルターオプションを使用して、このリストを参照します。プロファイルの属性の一部を編集および更新できます。"

## プロファイルの基本を学ぶ {#gs}

Adobe Campaign Web のプロファイルは、データベースに格納された個人で、配信のオーディエンスを作成し、コンテンツにパーソナライゼーションデータを追加するための主要なコンポーネントとして機能します。 様々なタイプのプロファイルがデータベースに保存されます（テストプロファイルなど）。テストプロファイルは、最終的なオーディエンスに配信を送信する前に配信をテストするように設計されています。 [テストプロファイルの操作方法を説明します。](test-profiles.md)

プロファイルは、Campaign クライアントコンソールからのみ追加できます。 ただし、Adobe Campaign Web では、 **プロファイル** エントリをクリックします。 また、 **エクスプローラ** フォルダ、サブフォルダを参照、作成、および関連付けられた権限を確認できるビュー。

プロファイルリストは、 **フィルターを表示** 」ボタンをクリックします。

![](assets/profiles-list.png)

>[!NOTE]
>
>権限によっては、データベースに保存されているプロファイルの完全なリストへのアクセス権がない場合があります。 権限について詳しくは、[この節](../get-started/permissions.md)を参照してください。

## プロファイルの属性へのアクセスと編集 {#access}

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_details"
>title="基本の詳細"
>abstract="この節では、プロファイルの基本的な詳細に関するインサイトを提供します。 情報を変更するには、各フィールド内で直接変更をおこない、 **保存** ボタンをクリックします。"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_contactinformation"
>title="連絡先情報"
>abstract="この節では、プロファイルの連絡先情報に関するインサイトを提供します。 情報を変更するには、各フィールド内で直接変更をおこない、 **保存** ボタンをクリックします。"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_address"
>title="住所"
>abstract="このセクションでは、プロファイルの住所と住所の質に関するインサイトを提供します。 情報を変更するには、各フィールド内で直接変更をおこない、 **保存** ボタンをクリックします。"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_account"
>title="アカウントの詳細"
>abstract="この節では、プロファイルのアカウント詳細に関するインサイトを提供します。 情報を変更するには、各フィールド内で直接変更をおこない、 **保存** ボタンをクリックします。"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_nolongercontact"
>title="受信者の今後の連絡は不要"
>abstract="この節では、プロファイルの連絡先設定に関するインサイトを提供します。 情報を変更するには、各フィールド内で直接変更をおこない、 **保存** ボタンをクリックします。"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_customfields"
>title="カスタムフィールド"
>abstract="カスタムフィールドは、お使いのインスタンスに合わせて設定された、ニーズに合わせた特定の属性です。 情報を変更するには、各フィールド内で直接変更をおこない、 **保存** ボタンをクリックします。"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_othersfields"
>title="その他"
>abstract="この節では、追加の組み込み属性を提供します。 情報を変更するには、各フィールド内で直接変更をおこない、 **保存** ボタンをクリックします。"

>[!CONTEXTUALHELP]
>id="acw_recipients_subscription_list"
>title="受信者の購読リスト"
>abstract="このタブには、プロファイルが購読しているすべてのサービスが表示されます。"

プロファイルの詳細にアクセスするには、プロファイルリストでプロファイルの名前をクリックします。

![](assets/profiles-details.png)

この画面から、プロファイルの詳細情報にアクセスできます。

* The **[!UICONTROL 詳細]** 「 」タブを使用すると、プロファイルの組み込み属性とカスタム属性を参照できます。 属性を編集するには、目的のフィールドに変更を加え、 **[!UICONTROL 保存]** 」ボタンをクリックします。
* The **[!UICONTROL 購読]** 「 」タブには、プロファイルが購読しているサービスに関する情報が表示されます。 [サブスクリプションサービスの使用方法を学ぶ](manage-services.md)
* The **[!UICONTROL ログ]** 画面の右上隅にあるボタンを使用すると、送信、除外、トラッキングのログや、プロファイルに提示された提案を通じて、プロファイルのインタラクションの履歴を表示できます。
