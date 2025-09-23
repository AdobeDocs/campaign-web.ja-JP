---
title: 外部アカウントの管理
description: 外部アカウントの設定方法について説明します
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '648'
ht-degree: 97%

---

# Campaign 固有の外部アカウント {#external-account}

選択した外部アカウントのタイプに基づいてアカウント設定を指定するには、次の手順に従います。

## バウンスメール（POP3） {#bounce}

バウンスメール外部アカウントで、メールサービスの接続に使用する外部 POP3 アカウントを指定します。POP3 アクセス用に設定されたすべてのサーバーは、返信メールを受信できます。

![バウンスメール（POP3）外部アカウント設定フィールドを示すスクリーンショット。](assets/external_account_bounce.png)

**[!UICONTROL バウンスメール（POP3）]**&#x200B;外部アカウントを設定するには、次のフィールドに入力します。

* **[!UICONTROL サーバー]** - POP3 サーバーの URL。

* **[!UICONTROL ポート]** - POP3 接続ポート番号（デフォルトポートは 110）。

* **[!UICONTROL アカウント]** - ユーザーの名前。

* **[!UICONTROL パスワード]**：ユーザーアカウントのパスワード。

* **[!UICONTROL 暗号化]** - 次を含む選択した暗号化のタイプ：
   * デフォルト（ポート 110 の場合は POP3、ポート 995 の場合は POP3S）。
   * STARTTLS の送信後に SSL に切り替える POP3。
   * 非セキュアな POP3（デフォルトポート 110）。
   * SSL による POP3 セキュア（デフォルトポート 995）。

* **[!UICONTROL 関数]** - 受信メールを受信するアカウントを設定するには「**[!UICONTROL インバウンドメール]**」を選択し、SOAP リクエストを処理するには「**[!UICONTROL SOAP ルーター]**」を選択します。

>[!IMPORTANT]
>
>Microsoft OAuth 2.0 を使用して POP3 外部アカウントを設定する前に、まず Azure portal にアプリケーションを登録する必要があります。詳しくは、[このページ](https://learn.microsoft.com/ja-jp/entra/identity-platform/quickstart-register-app){target=_blank}を参照してください。

Microsoft OAuth 2.0 を使用して POP3 外部を設定するには、「Microsoft OAuth 2.0」オプションをチェックし、次のフィールドに入力します。

* **[!UICONTROL Azure テナント]**

  Azure ID（またはディレクトリ（テナント）ID）は、Azure portal のアプリケーションの概要の初期設定ドロップダウンで確認できます。

* **[!UICONTROL Azure クライアント ID]**

  クライアント ID（またはアプリケーション（クライアント）ID）は、Azure portal のアプリケーションの概要の初期設定ドロップダウンで確認できます。

* **[!UICONTROL Azure クライアントシークレット]**

  クライアントシークレット ID は、Azure portal のアプリケーションの証明書と秘密鍵メニューから、「クライアントシークレット」列で確認できます。

* **[!UICONTROL Azure リダイレクト URL]**

  リダイレクト URL は Azure portal のアプリケーションの認証メニューで確認できます。次の構文 nl/jsp/oauth.jsp で終わる必要があります。例：`https://redirect.adobe.net/nl/jsp/oauth.jsp`。

設定を行い、クライアントコンソールの「テスト接続」ボタンを使用するには、インターネットアクセスが必要です。設定後、inMail プロセスはインターネットを使用せずに Microsoft サーバーと通信できます。

別の資格情報を入力した後、「接続を設定」をクリックして、外部アカウントの設定を終了できます。

## ルーティング {#routing}

外部配信用の特定の外部アカウントを設定するには、次の手順に従います。

1. 外部アカウントを作成します。[詳細情報](create-external-account.md)

1. **[!UICONTROL ルーティング]**&#x200B;タイプを選択します。

   ![外部アカウントのルーティングタイプの選択を示すスクリーンショット。](assets/external-account-routing.png){zoomable="yes"}

1. 目的のチャネルを選択し、「**[!UICONTROL 作成]**」をクリックします。

1. 外部アカウントの「**[!UICONTROL 詳細]**」セクションでは、**[!UICONTROL 配信モード]**&#x200B;として「**[!UICONTROL 外部]**」がデフォルトで選択されています。

   ![外部アカウントのルーティング用の配信モード設定を示すスクリーンショット。](assets/external-account-delivery-mode.png){zoomable="yes"}

   >[!NOTE]
   >
   >現在、使用可能なモードは&#x200B;**[!UICONTROL 外部]**&#x200B;のみです。

1. 配信実行後のプロセスを処理するには、後処理ワークフローに外部化します。[外部シグナル](../workflows/activities/external-signal.md)アクティビティを含むワークフローを作成し、「**[!UICONTROL 後処理]**」フィールドから選択します。

   ![外部アカウントのルーティング用の「後処理」フィールド設定を示すスクリーンショット。](assets/external-account-post-processing.png){zoomable="yes"}

1. 「**[!UICONTROL アクティビティ]**」フィールドでは、ログに表示される後処理ワークフローアクティビティの名前を編集します。<!--you can edit the name of the activity that will be created if you add an external or bulk delivery to a workflow-->

## 実行インスタンス {#instance-exec}

セグメント化されたアーキテクチャを使用している場合は、コントロールインスタンスに関連付けられた実行インスタンスを識別し、それらの間の接続を確立します。トランザクションメッセージテンプレートは、実行インスタンスにデプロイされます。

![実行インスタンス外部アカウント設定フィールドを示すスクリーンショット。](assets/external_account_exec.png)

**[!UICONTROL 実行インスタンス]**&#x200B;の外部アカウントを設定するには：

* **[!UICONTROL URL]** - 実行インスタンスがインストールされているサーバーの URL。

* **[!UICONTROL アカウント]** - オペレータフォルダーで定義されている Message Center エージェントに一致するアカウント名。

* **[!UICONTROL パスワード]** - 「オペレーター」フォルダーで定義されたアカウントのパスワード。

* **[!UICONTROL メソッド]** - web サービスまたは Federated Data Access（FDA）から選択します。

  FDA の場合は、FDA アカウントを選択します。外部システムへの Campaign の接続は上級ユーザーに制限され、クライアントコンソールからのみ使用できます。[詳細情報](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/connect/fda#_blank)

* **[!UICONTROL アーカイブワークフローの作成]** -1 つ以上のインスタンスがあるかどうかに関係なく、Message Center に登録された実行インスタンスごとに、実行インスタンスに関連付けられた外部アカウントにつき個別のアーカイブワークフローを作成します。
