---
title: プロファイルの作成
description: Campaign Web でプロファイルを作成する方法を説明します。
badge: label="限定提供（LA）"
exl-id: 0680b726-8f2f-45bf-8aa0-c1d4aa1c2990
source-git-commit: 22b183a739dd92d7c4245fb4694034a247511d75
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 56%

---

# プロファイルの作成 {#profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_details"
>title="基本の詳細"
>abstract="この節では、プロファイルの基本的な詳細に関するインサイトを提供します。情報を変更するには、各フィールド内で直接変更を行い、画面の右上隅にある「**保存**」ボタンをクリックします。"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_contactinformation"
>title="連絡先情報"
>abstract="このセクションでは、プロファイルの連絡先情報に関するインサイトを提供します。情報を変更するには、各フィールド内で直接変更を行い、画面の右上隅にある「**保存**」ボタンをクリックします。"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_address"
>title="住所"
>abstract="この節では、プロファイルの郵送先住所と住所の品質に関するインサイトについて説明します。情報を変更するには、各フィールド内で直接変更を行い、画面の右上隅にある「**保存**」ボタンをクリックします。"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_account"
>title="アカウントの詳細"
>abstract="このセクションでは、プロファイルのアカウント詳細に関するインサイトを提供します。情報を変更するには、各フィールド内で直接変更を行い、画面の右上隅にある「**保存**」ボタンをクリックします。"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_nolongercontact"
>title="今後の連絡が不要な受信者"
>abstract="このセクションでは、プロファイルの連絡先設定に関するインサイトを提供します。情報を変更するには、各フィールド内で直接変更を行い、画面の右上隅にある「**保存**」ボタンをクリックします。"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_customfields"
>title="カスタムフィールド"
>abstract="カスタムフィールドは、インスタンス用に設定された、ニーズに合わせて調整された特定の属性です。情報を変更するには、各フィールド内で直接変更を行い、画面の右上隅にある「**保存**」ボタンをクリックします。"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_othersfields"
>title="その他"
>abstract="この節では、追加の組み込み属性について説明します。情報を変更するには、各フィールド内で直接変更を行い、画面の右上隅にある「**保存**」ボタンをクリックします。"

プロファイルを作成するには、次の手順に従います。

1. に移動します。 **[!UICONTROL 顧客管理]** > **[!UICONTROL プロファイル]** をクリックし、 **[!UICONTROL プロファイルを作成]** 」ボタンを使用して、画面の右上隅に表示されます。

1. プロファイル表示に使用できる属性のリスト。次の表で詳しく説明する様々なセクションに分類されています。

   ![](assets/create-profile.png)

   | 「属性」セクション | 説明 |
   |  ---  |  ---  |
   | **基本的な詳細** | 名前や生年月日など、プロファイルに関する基本情報。<br/>デフォルトでは、プロファイルは **[!UICONTROL 受信者]** フォルダー。 目的の場所を参照して変更できます。[詳しくは、フォルダーの操作方法を参照してください](../get-started/permissions.md#folders) |
   | **連絡先情報** | プロファイルの連絡先情報（電子メールアドレスや電話番号など）。 |
   | **住所** | プロファイルの住所。 また、アドレスの質の評価も行います。 「姓」、「市区町村」および「郵便番号」フィールドが指定されている場合、プロファイルのアドレスは有効と見なされます。 |
   | **アカウントの詳細** | プロファイルのアカウントに関する情報（ステータスやアカウント番号など）。 |
   | **今後の連絡は不要** | プロファイルの連絡先の環境設定。 これらのオプションのいずれかを選択すると、プロファイルはオンになブロックリストに加えるります。<br/>例えば、受信者がニュースレターの購読解除リンクをクリックした場合、この情報が連絡先データに追加されます。 このような受信者は、選択したチャネルのターゲットに設定されなくなりました。での強制隔離管理の詳細を説明します。 [Adobe Campaign v8 ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html?lang=ja){target="_blank"} |
   | **カスタムフィールド** | カスタムフィールドが設定されている場合は、このセクションに表示されます。 カスタムフィールドは、Adobe Campaign コンソールを通じて&#x200B;**[!UICONTROL プロファイル]**&#x200B;スキーマに追加される追加属性です。詳しくは、 [Adobe Campaign v8 ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema.html?lang=ja){target="_blank"} |
   | **その他** | 追加の組み込み属性。 |

1. プロファイルを設定したら、「 **[!UICONTROL 作成]** をクリックして、データベースに保存します。

   完了したら、プロファイルのリストから開いて、いつでもプロファイルを編集できます。 [プロファイルの詳細を参照する方法を説明します](profile-view.md)
