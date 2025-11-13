---
title: 外部アカウントの管理
description: CRM 外部アカウントの設定方法について説明します
source-git-commit: 934a37cfebfacd2df0b7610285252d883611f252
workflow-type: ht
source-wordcount: '857'
ht-degree: 100%

---

# CRM 外部アカウント {#external-crm}

外部 CRM タイプのアカウントを使用して、Adobe Campaign をサードパーティのデータベースに接続します。

この外部アカウントの設定は、接続先の特定のデータベースエンジンによって異なります。サポートされている各データベースの設定手順について詳しくは、以下の節を参照してください。

## Microsoft Dynamics CRM

Microsoft Dynamics CRM 外部アカウントを使用すると、Campaign インスタンスを Microsoft Dynamics CRM 外部データベースに接続できます。

Adobe Campaign web ユーザーインターフェイスで、Microsoft Dynamics CRM 外部アカウントを設定します。

1. [外部アカウントを作成](external-account.md)し、外部アカウントの&#x200B;**[!UICONTROL タイプ]**&#x200B;として「**[!UICONTROL 外部データベース]**」を選択し、**[!UICONTROL プロバイダータイプ]**&#x200B;として「Microsoft Dynamics CRM」を選択します。

1. 「**[!UICONTROL 作成]**」をクリックします。

1. **[!UICONTROL Microsoft Dynamics CRM]** 外部アカウントを設定するには、次のフィールドに入力します。

   ![Microsoft Dynamics CRM 外部アカウント設定フィールドを示すスクリーンショット。](assets/crm-microsoft-1.png)

   +++ CRM OAuth タイプの場合：パスワード資格情報

   * **[!UICONTROL サーバー]**：Microsoft CRM Server の URL を入力します。

     Microsoft CRM Server URL を見つけるには、Microsoft Dynamics CRM アカウントにログインし、「Dynamics 365」を選択して、アプリを開きます。サーバーの URL は、ブラウザーのアドレスバーに表示されます（例：`https://myserver.crm.dynamics.com/`）。

   * **[!UICONTROL アカウント]**：Microsoft CRM へのログインに使用するアカウントを指定します。

   * **[!UICONTROL パスワード]**：指定したアカウントに関連付けられたパスワードを入力します。

   * **[!UICONTROL クライアント識別子]**：Microsoft Azure の管理ポータルにあるクライアント ID を入力します。

   * **[!UICONTROL CRM バージョン]**：Dynamics CRM 365 CRM バージョンを選択します。

   +++

   </br>

   +++ CRM O-Auth タイプの場合：証明書

   * **[!UICONTROL サーバー]**：Microsoft CRM Server の URL を入力します。

     Microsoft CRM Server URL を見つけるには、Microsoft Dynamics CRM アカウントにログインし、「Dynamics 365」を選択して、アプリを開きます。サーバーの URL は、ブラウザーのアドレスバーに表示されます（例：`https://myserver.crm.dynamics.com/`）。

   * **[!UICONTROL 秘密鍵（Base64 エンコード）]**：Base64 形式でエンコードされた秘密鍵を指定します。

     それには、Base64 エンコーダーを利用するか、Linux の場合はコマンドライン `base64 -w0 private.key` を使用します。

   * **[!UICONTROL カスタムキー識別子]**：証明書に使用するカスタムキー識別子を入力します。

   * **[!UICONTROL キー ID]**：証明書に関連付けられたキー ID を入力します。

   * **[!UICONTROL クライアント識別子]**：Microsoft Azure の管理にあるクライアント ID を入力します

   * **[!UICONTROL CRM バージョン]**：Dynamics CRM 365 CRM バージョンを選択します。

   +++

1. 接続を設定したら、**[!UICONTROL Microsoft CRM 設定ウィザード]**&#x200B;にアクセスして、Microsoft CRM テーブルリストを生成します。

   「**[!UICONTROL 次へ]**」をクリックして、必要なテーブルを選択します。

   ![Microsoft Dynamics CRM 外部アカウント設定フィールドを示すスクリーンショット。](assets/crm-microsoft-2.png)

1. 取得する Microsoft CRM テーブルを選択するか、**[!UICONTROL テーブルラベル]**&#x200B;と&#x200B;**[!UICONTROL テーブル内部名]**&#x200B;を指定してリモートテーブルを追加し、**[!UICONTROL 選択済み]**&#x200B;切替スイッチを有効にします。

   「**[!UICONTROL 次へ]**」をクリックします。

1. 「**[!UICONTROL 開始]**」をクリックして、選択したテーブルに基づいた Microsoft CRM スキーマの作成を開始します。

1. 画面上の指示に従って、Adobe Campaign のマーケティング履歴および購読管理から Microsoft Dynamics CRM に直接ページを挿入します。

1. 「**[!UICONTROL マーケティング履歴 URL を表示]**」をクリックすると、マーケティング履歴ページを統合する URL が表示されます。また、「**[!UICONTROL リード購読の URL を表示]**」をクリックすると、購読管理ページを統合する URL が表示されます。

   ![Microsoft Dynamics CRM 外部アカウント設定フィールドを示すスクリーンショット。](assets/crm-microsoft-3.png)

1. Microsoft CRM 外部アカウントを設定したら、「**[!UICONTROL 保存]**」をクリックします。

1. 外部アカウントを作成したら、「**[!UICONTROL 定義済みリストを同期中...]**」をクリックして、Microsoft CRM から Adobe Campaign web ユーザーインターフェイスに定義済みリストを自動的に同期できます。

   ![Microsoft CRM 外部アカウント設定フィールドを示すスクリーンショット。](assets/crm-microsoft-4.png)

1. Microsoft CRM 定義済みリストに一致する Adobe Campaign 定義済みリストを選択します。

   Adobe Campaign の値を Microsoft CRM の値に置き換えるには、「**[!UICONTROL 置換]**」オプションを有効にします。

## Salesforce {#salesforce}

Salesforce 外部アカウントを Adobe Campaign で使用できるように設定するには、次の情報を提供する必要があります。

1. [外部アカウントを作成](external-account.md)し、外部アカウントの&#x200B;**[!UICONTROL タイプ]**&#x200B;として「**[!UICONTROL 外部データベース]**」を選択し、**[!UICONTROL プロバイダータイプ]**&#x200B;として「Salesforce.com」を選択します。

   ![Salesforce 外部アカウント設定フィールドを示すスクリーンショット。](assets/crm-salesforce-1.png)

1. 「**[!UICONTROL 作成]**」をクリックします。

1. **[!UICONTROL Salesforce]** 外部アカウントを設定するには、次のフィールドに入力します。

   * **[!UICONTROL CRM O-Auth タイプ]**：**[!UICONTROL パスワード資格情報]**&#x200B;または **[!UICONTROL 資格情報]**

   * **[!UICONTROL アカウント]**：Salesforce CRM へのログインに使用するアカウント。

   * **[!UICONTROL パスワード]**：指定したアカウントに関連付けられたパスワードを入力します。

   * **[!UICONTROL セキュリティトークン]**：アカウントに関連付けられた Salesforce セキュリティトークンを入力します。

   * **[!UICONTROL API バージョン]**：「バージョン 49」を選択します。

   ![Salesforce 外部アカウント設定フィールドを示すスクリーンショット。](assets/crm-salesforce-2.png)

1. **[!UICONTROL Salesforce CRM 設定ウィザード]**&#x200B;を開いて Salesforce CRM テーブルリストを生成し、「**[!UICONTROL 次へ]**」をクリックします。

   ![Salesforce CRM 外部アカウント設定フィールドを示すスクリーンショット。](assets/crm-salesforce-3.png)

1. 取得する Salesforce テーブルを選択するか、**[!UICONTROL テーブルラベル]**&#x200B;と&#x200B;**[!UICONTROL テーブル内部名]**&#x200B;を入力してリモートテーブルを追加し、**[!UICONTROL 選択済み]**&#x200B;切替スイッチを有効にします。

   「**[!UICONTROL 次へ]**」をクリックします。

1. 「**[!UICONTROL 開始]**」をクリックして、選択したテーブルに基づいた Salesforce CRM スキーマの作成を開始します。

1. 「**[!UICONTROL Salesforce リンク作成ウィザード…]**」をクリックして、Salesforce で web リンクを生成します。

   その後、「**[!UICONTROL 次へ]**」をクリックして、Salesforce から&#x200B;**リード**&#x200B;と&#x200B;**連絡先**&#x200B;の web リンクを取得します。

1. Salesforce web リンクリストにエクスポートするリンクを選択します。

1. 画面上の指示に従って、Adobe Campaign web ユーザーインターフェイスから&#x200B;**マーケティング履歴**&#x200B;ページと&#x200B;**購読管理**&#x200B;ページを Salesforce CRM に挿入します。

1. Salesforce CRM 外部アカウントを設定したら、「**[!UICONTROL 保存]**」をクリックします。

1. 外部アカウントを作成したら、「**[!UICONTROL 定義済みリストを同期中...]**」をクリックして、Salesforce から Adobe Campaign web ユーザーインターフェイスに定義済みリストを自動的に同期できます。

   ![Salesforce CRM 外部アカウント設定フィールドを示すスクリーンショット。](assets/crm-salesforce-4.png)

1. Salesforce 定義済みリストに一致する Adobe Campaign 定義済みリストを選択します。

   Adobe Campaign の値を Salesforce の値に置き換えるには、「**[!UICONTROL 置換]**」オプションを有効にします。

   ![Salesforce CRM 外部アカウント設定フィールドを示すスクリーンショット。](assets/crm-salesforce-5.png)

