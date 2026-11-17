---
title: Adobe Campaign Web インターフェイスに接続
description: Adobe Campaign Web ユーザーインターフェイスに接続する方法について説明します
exl-id: 5a8023a9-5b9e-429f-ba56-b01423993e55
TQID: 'https://experienceleague.adobe.com/TSbgkDH1v-9HH-szfGQx0z6-6fP8tny4s7Vx2SE8gUo'
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
topic_v2:
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
    internal-label: Data management
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 7bbc2d4c383886788afc1ef83cdd27e7ec4b24ae
workflow-type: tm+mt
source-wordcount: '926'
ht-degree: 81%
---
# Adobe Campaign への接続 {#connect-to-campaign}

[!DNL Adobe CX Enterprise]は、Adobeの統合デジタルマーケティングアプリケーション、製品、サービスのファミリーです。 直感的なインターフェイスから、クラウドアプリケーション、製品機能、サービスにすばやくアクセスできます。 [!DNL CX Enterprise]に接続し、このページのAdobe Campaign Web インターフェイスにアクセスする方法について説明します。

## [!DNL Adobe CX Enterprise]にログイン {#sign-in-to-exc}

シングルサインオン（SSO）のみを使用して Campaign に接続できます。 通常、[!DNL CX Enterprise]人の管理者がアプリケーションとサービスへのアクセス権を付与します。 [!DNL CX Enterprise]へのメール招待状の手順に従います。

[!DNL Adobe CX Enterprise]にログインするには、次の基本的な手順に従います。

1. [[!DNL Adobe CX Enterprise]](https://experience.adobe.com/){target="_blank"}を参照します。

1. Adobe ID または Enterprise ID を使用してログインします。 アドビの ID タイプについて詳しくは、[この記事](https://helpx.adobe.com/jp/enterprise/using/identity.html){target="_blank"}を参照してください。

   [!DNL CX Enterprise]にログインすると、すべてのソリューションとアプリにすばやくアクセスできます。

   ![Adobe CX Enterpriseのホームページを示すスクリーンショット ](assets/exc-home.png){zoomable="yes"}

1. 自分が正しい組織に属していることを確認してください。

   ![Adobe CX Enterpriseでの組織選択を示すスクリーンショット ](assets/exc-orgs.png){zoomable="yes"}{width="50%"}

   [!DNL Adobe CX Enterprise]の組織について詳しくは、[この記事](https://experienceleague.adobe.com/docs/core-services/interface/administration/organizations.html?lang=ja){target="_blank"}を参照してください。

## Adobe Campaign にアクセス {#access-to-campaign}

Campaign環境にアクセスするには、[!DNL Adobe CX Enterprise] ホームページの&#x200B;**クイックアクセス** セクションから&#x200B;**Campaign**&#x200B;を選択します。

既に別の[!DNL Adobe CX Enterprise] ソリューションに接続している場合は、画面右上のソリューション スイッチャーからCampaign環境を参照します。

Adobe CX Enterpriseのソリューションスイッチャーを示す![ スクリーンショット ](assets/solution-switcher.png){zoomable="yes"}

複数の環境（Campaign コントロールパネルを含む）にアクセスできる場合は、「**起動する**」ボタンをクリックして正しいインスタンスを確認します。

![Adobe Campaign の「起動する」ボタンを示すスクリーンショット](assets/launch-campaign.png){zoomable="yes"}

Campaign に接続しました。 ユーザーインターフェイスの使用を開始する方法については、[このページ](user-interface.md)を参照してください。

### アクセス制御 {#access-control}

>[!CONTEXTUALHELP]
>id="acw_explorer_permissions_create"
>title="権限が必要です"
>abstract="このオブジェクトを作成するには、管理者から権限が付与されている必要があります。"

>[!CONTEXTUALHELP]
>id="acw_audiences_read_only"
>title="このオーディエンスは読み取り専用です"
>abstract="このオーディエンスを編集する権限がありません。 必要に応じて、管理者に連絡し、アクセス権の付与を依頼してください。"

>[!CONTEXTUALHELP]
>id="acw_subscription_services_read_only"
>title="このサービスは読み取り専用です"
>abstract="このサービスを編集する権限がありません。 必要に応じて、管理者に連絡し、アクセス権の付与を依頼してください。"

>[!CONTEXTUALHELP]
>id="acw_recipients_readonlyprofile"
>title="受信者の読み取り専用プロファイル"
>abstract="このプロファイルを編集する権限がありません。 必要に応じて、管理者に連絡し、アクセス権の付与を依頼してください。"

>[!CONTEXTUALHELP]
>id="acw_campaign_read_only"
>title="このキャンペーンは読み取り専用です"
>abstract="このキャンペーンを編集する権限がありません。 必要に応じて、管理者に連絡し、アクセス権の付与を依頼してください。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_read_only"
>title="この配信は読み取り専用です"
>abstract="この配信を編集する権限がありません。 必要に応じて、管理者に連絡し、アクセス権の付与を依頼してください。"

>[!CONTEXTUALHELP]
>id="acw_wf_read_only"
>title="このワークフローは読み取り専用です"
>abstract="このワークフローを編集する権限がありません。 必要に応じて、管理者に連絡し、アクセス権の付与を依頼してください。"

アクセス制御では、配信、受信者、ワークフローなどのメインリストからのオブジェクトやデータへのアクセスを制限します。 また、これらの制限は、エクスプローラーのナビゲーションツリーにも適用されます。 さらに、ユーザーインターフェイスからオブジェクトを作成、削除、複製、編集する権限が必要です。

Campaign web のすべての権限は、Campaign クライアントコンソールの権限と同期されます。 ユーザー権限を定義および変更できるのは、Campaign 管理者のみです。

Campaign web ユーザーインターフェイスを参照すると、権限に応じてデータ、オブジェクト、機能にアクセスできます。 例えば、フォルダーへのアクセス権限がない場合、そのフォルダーは表示されません。 また、権限は、オブジェクトとデータの管理にも影響します。 特定のフォルダーに対する書き込み権限がないと、ユーザーインターフェイスに配信が表示されていても、そのフォルダーに配信を作成することはできません。

詳しくは、[権限の表示と管理](permissions.md)の方法を参照してください。

## [!DNL Adobe CX Enterprise]上部ナビゲーション {#top-bar}

インターフェイスの上部バーでは、コア [!DNL CX Enterprise]機能にすばやくアクセスできます。

![Adobe CX Enterpriseの上部のナビゲーションバーを示すスクリーンショット ](assets/do-not-localize/unified-shell.png){zoomable="yes"}

上部のバーを使用すると、以下を実行できます。

* Campaign web ユーザーインターフェイスに関するフィードバックを共有する。
* 組織を切り替える。
* [!DNL Adobe CX Enterprise]個のソリューションとアプリを切り替えます。
* [Adobe Experience League](https://experienceleague.adobe.com/docs/?lang=ja){target="_blank"} でヘルプを検索する。
* 製品通知を表示する。
* アドビのプロファイルを編集し、[優先言語の更新](#language-pref)や[ライト／ダークテーマに切り替え](#dark-theme)などの設定を管理する。

## サポートしているブラウザー {#browsers}

Adobe Campaign Web は、最新バージョンの Google Chrome、Safari および Microsoft Edge で最適に動作するように設計されています。 古いバージョンや他のブラウザーでは、特定の機能を使用する際に問題が発生する可能性があります。

## 言語環境設定 {#language-pref}

Adobe Campaign Web は現在、次の言語で利用できます。

* 英語（米国）- EN-US
* フランス語 - FR
* ドイツ語 - DE
* イタリア語 - IT
* スペイン語 - ES
* ポルトガル語（ブラジル）- PTBR
* 日本語 - JP
* 韓国語 - KR
* 簡体字中国語 - CHS
* 繁体字中国語 - CHT

さらに、ロケール固有の書式設定（日付、時刻、カレンダー、数値など）も、ユーザーインターフェイスでサポートされている言語のバリアントで使用できる場合があります。

* 英語（イスラエル）
* 英語（英国）
* スペイン語（メキシコ）
* スペイン語（ラテンアメリカ）
* フランス語（カナダ）

Campaign web のデフォルト言語は、ユーザープロファイルで指定された優先言語によって決まります。 Campaign サーバーとクライアントコンソールの言語とは関係ありません。

言語を変更するには：

1. 右上のプロファイルアイコンをクリックし、 「**環境設定**」を選択します。
1. メールアドレスの下に表示されている言語リンクをクリックします。
1. 優先言語を選択し、「**保存**」をクリックします。 使用しているコンポーネントが第一希望の言語にローカライズされていない場合に備えて、第二の言語を選択できます。


## ダークテーマとライトテーマ {#dark-theme}

Adobe Campaign は、ライトテーマとダークテーマで使用できます。 デフォルトでは、ユーザーインターフェイスはライトテーマで有効になっています。 ダークテーマに切り替えるには、プロファイルアイコンをクリックし、「**ダークテーマ**」切替スイッチを使用して有効または無効にします。

ユーザープロファイルの設定とアカウントの環境設定について詳しくは、[この節](https://experienceleague.adobe.com/docs/core-services/interface/experience-cloud.html?lang=ja#preferences){target="_blank"}を参照してください。

Experience Cloud セントラルインターフェイスコンポーネントについて詳しくは、[このドキュメント](https://experienceleague.adobe.com/docs/core-services/interface/experience-cloud.html?lang=ja){target="_blank"}を参照してください。