---
title: Adobe Developer Console へのテクニカルユーザーの移行
description: Campaign Standardから Campaign V8 にユーザーアクセス管理を移行する方法を説明します
feature: Technote
role: Admin
source-git-commit: e5baa9012e7904f841d4e6706d9dc8970253e899
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 4%

---

# Campaign Standardから Campaign V8 へのユーザーアクセス管理 {#user-management-acs}

Adobe Campaign StandardとAdobe Campaign V8 の両方を使用すると、ユーザーは異なるユーザー/オペレーターの権限を定義および管理できます。 これらの権限は、製品の様々な機能へのアクセス権をユーザーに付与する特定の権限で構成されます。 ただし、これら 2 つの製品では、ユーザーアクセスを管理するための個別のアプローチと実装が使用されています。

Adobe Campaign Standardと Campaign V8 では、ユーザーアクセスを管理するために、以下の概念が使用されています。

| Campaign Standard | Campaign V8 |
|---------|----------|
| ユーザー | 演算子 |
| 役割 | ネームド権限 |
| セキュリティグループ | オペレーターグループ |
| 組織単位 | フォルダー権限 |

## セキュリティグループからオペレーターグループへの移行アプローチ

>[!CAUTION]
>
>これらの役割/ネームド権限の機能は、実装が異なる場合があり、権限の昇格や機能の中断などの承認の問題を引き起こす可能性があります。 適切なアクセス制御を確保するために、移行後にこれらのマッピングを確認することをお勧めします。 [ 権限の詳細 ](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

次の表に、Adobe Campaign Standardから Campaign V8 に移行する際のユーザーロールグループの移行アプローチの概要を示します。 Campaign Standard、Campaign V8 では **オペレーターグループ** と呼ばれる **セキュリティグループ** を使用して、一連のロールをユーザーに割り当てます。 一部のセキュリティグループやオペレーターグループはすぐに使用できますが、ユーザーは、必要に応じて新しいグループを作成したり、既存のグループを変更したりできます。

| | **Campaign Standard** | **Campaign V8** |
|---------|----------|---------|
| **用語**  | セキュリティグループ | オペレーターグループ |

Adobe Campaign Standardと Campaign V8 の両方で、**セキュリティグループ** および **オペレーターグループ** が Admin Console の製品プロファイルにマッピングされます。 **セキュリティグループ** または **オペレーターグループ** をユーザーに割り当てる場合は、対応する **製品プロファイル** を Admin Console でリンクできます。 この関連付けは、ユーザーがログインしたときに同期されます。 [ 詳しくは、製品プロファイルを参照してください ](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

| **Campaign Standard セキュリティ グループ** | **Campaign V8 オペレーターグループ** |
|----------|---------|
| 管理者 | 管理者 |
| 配信スーパーバイザー | 管理者 |
| ワークフロースーパーバイザー | ワークフロースーパーバイザー  |

## ユーザーの役割からネームド権限への移行アプローチ

Adobe Campaign Standardでは、**ユーザーロール** という用語は、Campaign V8 では **ネームド権限** と呼ばれます。 次の表に、Campaign Standardの **ユーザーの役割** に対応する Campaign V8 の **ネームド権限** に使用される用語の概要を示します。

| **Campaign Standard ユーザーの役割** | **Campaign V8 のネームド権限** | **説明**  |
|----------|---------|---------|
| 管理 | 管理 | 管理権限を持つユーザーは、インスタンスに対して完全なアクセス権を持ちます。 |
| データモデル  | 管理 | パブリケーションを実行し、カスタム リソースを作成する権限。 Campaign V8 で管理者が使用できるスキーマ作成関連の機能。  |
| 配信品質  | 管理  | 以前に分析された配信を承認する権限。  |
| 書き出し | 書き出し | データを書き出す権限。  |
| ファイルアクセス  | ファイルへのアクセス  | 以前に分析された配信を承認する権限。  |
| 一般的なインポート  | インポート  | 汎用データインポートの権限 |
| 配信の準備 | 配信の準備 | 配信を作成、変更、準備および削除する権限。  |
| SQL スクリプトの実行 | SQL スクリプトの実行 | データベース上で直接 SQL コマンドを実行する権限。 |
| 配信の開始  | 配信の開始  | 以前に分析された配信を承認する権限。  |
| システムコマンドの実行 | プログラムの実行 | サーバ上でシステム・コマンドを実行する権限。 |
| ワークフロー | ワークフロー | ワークフローの実行を管理する権限の開始、停止、一時停止など |

## 組織単位からの移行アプローチ

Adobe Campaign Standardでは、同様のアクセス制御を維持するために、**Organization uni** t が Campaign V8 の既存の **フォルダー** 階層モデルにマッピングされます。 [ 詳しくは、フォルダー管理を参照してください ](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/admin/permissions/folder-permissions)

| | **Campaign Standard** | **Campaign V8** |
|---------|----------|---------|
| **用語**  | 組織単位 | フォルダー |

## プログラムからの移行アプローチ

Campaign V8 では、**プログラム** は **フォルダー** として表されます。 Campaign V8 では、フォルダーを作成でき、フォルダーへのアクセスを制限できます。

**グループ** および **ネームド権限** を使用すると、**オペレーター** にナビゲーション階層内の特定の **フォルダー** へのアクセス権を付与し、読み取り、書き込みおよび削除の権限を割り当てることができます。 [ 詳しくは、フォルダー管理を参照してください ](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/admin/permissions/folder-permissions)

**プログラム** は Campaign V8 では **フォルダー** として扱われるので、そのアクセスは他のフォルダーと同じように管理できます。 移行後、Campaign Standard管理者は次の手順に従うことができます。

1. エクスプローラーで任意のフォルダーを右クリックし、「**[!UICONTROL プロパティ…]**」を選択します。
1. 「**[!UICONTROL セキュリティ]**」タブに移動します。
1. 目的のアクセスモデルに従って、オペレーターグループの権限を変更します。 

## REST API にアクセスするための製品プロファイルのマッピング 

Campaign V8 の実行インスタンスからトランザクション API にアクセスするには、**管理者** および **Message Center** 製品プロファイルに加えて、新しい **製品プロファイル** が必要です。 この新しい **製品プロファイル** は、Campaign Standardの既存または事前に作成されたテクニカルアカウントに追加されます。

移行後、Campaign Standardユーザーは **製品プロファイルのマッピング** を確認し、適切な **製品プロファイル** を割り当てます。その際、**テクニカルアカウント** を **管理者** 製品プロファイルにリンクしたくない場合。 今後の統合では、以前のCampaign Standard **テナント ID** ではなく、**REST URL** で Campaign V8 **テナント ID** を使用することをお勧めします。

## Campaign Standardオペレーター向けの組み込み Campaign リソースへのアクセスの移行

Campaign Standardから移行したオペレーターは、Campaign V8 の特定のビルトインリソースに読み取りアクセスできます。

## 移行されていないセキュリティ・グループと役割 {#non-migrated-groups-roles}

以下は、移行されていないCampaign Standardロールのリストです。

* 既定のリレーアカウント 

* Message Center のプッシュ 

移行されていないCampaign Standard セキュリティ グループ マッピングの一覧を以下に示します。

* Message Center エージェント

* Message Center プッシュエージェント

* Adobe Experience Manager アプリケーションマネージャー

* リレーアカウント
 


 

 

