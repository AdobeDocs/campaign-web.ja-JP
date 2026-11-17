---
title: Campaign StandardとCampaign v8の違い
description: Campaign StandardからCampaign v8に移行する際の変更点と、詳細を確認する場所について説明します
hide: true
robots: noindex
googlebot: noindex
role: User, Admin, Developer
level: Beginner
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
source-git-commit: 5a6b111d1aaa2a34ce165eaf6d1b1a997fd8bc85
workflow-type: tm+mt
source-wordcount: '1916'
ht-degree: 5%
---
# Campaign StandardとCampaign v8の違い {#acs-v8-differences}

ほとんどのコンセプトは、Campaign StandardとCampaign v8で同じです。 このページでは、移行後に影響を与える違いを収集し、それぞれの違いを説明するページにリンクします。 [ マーケター](marketers.md)および[管理者と開発者](admin-developers.md)のガイドを補完します。

* 用語の変更については、[用語](#terminology)を参照してください。
* 移行を実行するためのチェックと、移行後に報告された問題については、[移行後のチェックとトラブルシューティング ](post-transition-checks.md)を参照してください。
* クライアントコンソールでのみ使用できる機能については、[Campaign WebおよびCampaign クライアントコンソール ](../../v8/get-started/capability-matrix.md)を参照してください。

## 用語 {#terminology}

ほとんどの概念は、Adobe Campaign v8 と Adobe Campaign Standard で類似しています。 ただし、用語から始めて、いくつかの違いがあります。

| Campaign Standardの | Campaign v8で |
|---|---|
| カスタムリソース | **スキーマ** |
| メッセージ | **配信** |
| 製品ユーザー | **演算子** |
| 役割 | **名前付き権限**&#x200B;で構成 |
| セキュリティグループ | **オペレーターグループ** |
| 組織単位 | **フォルダー権限**&#x200B;で管理 |

また、既存の Campaign ユーザーとして、一部の概念は最新の用語標準に合わせて名前が変更されています。 これらの変更は、Campaign Web ユーザーインターフェイスにのみ適用され、クライアントコンソールには反映されません。

| Campaign Standardの | Campaign Web | 詳細情報 |
|---|---|---|
| 受信者 | **プロファイル** | [ プロファイル ](../../v8/audience/gs-audiences-recipients.md) |
| シードアドレス | **プロファイルのテスト** | [配信のテスト ](../../v8/preview-test/test-deliveries.md) |
| 配信分析 | **配信準備**。 メッセージの準備を開始するには、「**準備**」ボタンをクリックします。 | [準備と送信](../../v8/monitor/prepare-send.md) |
| メールのプレビュー | 「**コンテンツをシミュレート**」ボタンから使用できます。 | [プレビューとテスト](../../v8/preview-test/preview-test.md) |
| リスト | **オーディエンス** | [ オーディエンス ](../../v8/audience/gs-audiences-recipients.md) |

## チャネルとコンテンツ {#channels}

メッセージの作成と送信の手順は、両方の製品で似ています。詳しくは、[ マーケター向けガイド ](marketers.md)を参照してください。 以下の違いは、チャネルの可用性、テスト配信、ランディングページ、ダイレクトメールワークフローに関するものです。

| 変更点 | 詳細情報 |
|---|---|
| アプリ内チャネルは、Campaign v8では使用できません。 | [ アプリ内チャネル ](marketers.md#acs-gs-marketers-in-app) |
| 既存のプッシュワークフローと配信を移行するには、Adobe Campaign Transition Managerにお問い合わせください。 | [プッシュ通知](marketers.md#acs-gs-marketers-push) |
| Campaign Standardでは、テストプロファイルを&#x200B;**トラップ**&#x200B;としてマークして、最終送信を受け取ることができます。 Campaign v8で、配信のオーディエンス設定に&#x200B;**トラップグループ**&#x200B;を追加します。 | [ トラップグループ ](../../v8/audience/trap-group.md) |
| Campaign Web ユーザーインターフェイスで作成されたランディングページは、非表示の入力フィールドやカスタム JavaScriptをサポートしていません。 | [ランディングページ](../../v8/landing-pages/get-started-lp.md) |
| Campaign Standardでは、ダイレクトメールアクティビティのアウトバウンドトランジションにも、生成されたファイルが含まれています。 Campaign v8では、ターゲット母集団のみが取り込まれます。 ファイルをサーバーに送信するには、**データ抽出** アクティビティを追加してから、**ファイル転送** アクティビティを追加します。 | [ ダイレクトメール ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |

## オーディエンス、ワークフロー、配信 {#data-and-workflows}

これらの違いは、Campaign Standardから移行されたオーディエンスとワークフロー、定期的な配信と&#x200B;**ファイル転送** アクティビティのオプション、動的レポートの範囲に影響します。

| 変更点 | 詳細情報 |
|---|---|
| Campaign Standardの「クエリ」アクティビティで作成されたオーディエンスは、Campaign v8で[定義済みフィルター](../../v8/query/build-query.md)になります。 Campaign v8では、クエリアクティビティもサポートしています。 | [ オーディエンスの管理](marketers.md#acs-gs-marketers-audiences) |
| オーディエンスを読み取りアクティビティは、定義済みのフィルターを持つクエリアクティビティになります。 | [ オーディエンスの管理](marketers.md#acs-gs-marketers-audiences) |
| 定義済みフィルターは、オーディエンスの移行後に最新の値のみを使用します。 | [ オーディエンスの管理](marketers.md#acs-gs-marketers-audiences) |
| ファイルタイプのオーディエンスは、ディメンションを持たないリストタイプのオーディエンスになります。 | [ オーディエンスの管理](marketers.md#acs-gs-marketers-audiences) |
| Campaign Standardで実行されたワークフローの履歴ログは移行されません。 | [ワークフローの作成](marketers.md#acs-gs-marketers-wf) |
| Campaign Standardでは、定期的なメールの集計期間を選択できます。 このオプションは、Campaign v8では使用できません。 | [ チャネルアクティビティ ](../../v8/workflows/activities/channels.md) |
| 動的レポートでは、メール配信、メール配信を伴うキャンペーン、トランザクションメッセージを取り上げます。 | [レポート](marketers.md#acs-gs-marketers-reporting) |

## アクセスとセキュリティ {#access}

Campaign Standardのセキュリティグループ、ロール、組織単位は、移行時にオペレーターグループ、名前付き権限、フォルダー権限にマッピングされます。 特に、一部のユーザーが以前よりも広範または狭い権限を持っている場合は、以下の点を確認してください。

| 変更点 | 詳細情報 |
|---|---|
| セキュリティグループ、役割、組織単位は、オペレーターグループ、名前付き権限、フォルダー権限にマッピングされます。 カスタムの役割は移行されません。 | [ ユーザーアクセス管理](user-management-acs.md) |
| **データモデル**&#x200B;の役割を持ち、**管理**&#x200B;の役割を持たないユーザーは、**管理**&#x200B;へのアクセス権を取得します。 | [ ユーザーアクセス管理](user-management-acs.md#migration-approach-from-user-roles-to-named-rights) |
| 並列の組織単位を持つセキュリティ グループに割り当てられたユーザーは、Campaign v8でより広範なアクセス権を持つことができます。 | [組織ユニットの並列割り当て](user-management-acs.md#parallel-assignments) |
| 実行インスタンスからトランザクション APIにアクセスするには、新しい製品プロファイルが必要です。 | [製品プロファイルマッピング ](user-management-acs.md#product-profile-mapping-to-access-rest-apis) |
| プライバシーリクエストは、Campaign Standard環境がアクティブな状態を維持している間に、Campaign StandardとCampaign v8の両方に送信されます。 | [プライバシーと同意](admin-developers.md#privacy-and-consent) |

## APIと統合 {#apis-and-integrations}

これらの違いは、そのREST APIを介してCampaignを呼び出す統合機能、および他のAdobe ソリューションやツールとの統合機能に影響します。

| 変更点 | 詳細情報 |
|---|---|
| PKEY値は、移行後に変更されます。 Campaign以外でPKEYを保存する場合は、代わりにAPIから返されるhrefsに従います。 | [ キーの使用状況](#key-usage) |
| タイムゾーンや`ccpaOptOut`などの一部の移行されたプロファイルフィールドは、`profileAndServicesExt/profile` APIによってのみ返されます。 | [ プロファイルタイムゾーンとccpaOptOut](#profile-timezone) |
| Adobeは、Adobe AnalyticsとAudience Managerの設定を移行します。 トリガーとAdobe Targetの統合を再度設定する必要があります。 | [Adobe Campaign統合の管理](admin-developers.md#acs-gs-integrations) |

## REST APIの推奨事項と制限事項 {#rest-api-limitations}

以下の推奨事項と制限事項は、Campaign StandardからCampaign v8に移行する際のREST APIに適用されます。

### 権限とセキュリティ {#permissions}

#### 製品プロファイルの構築 {#rest-product-profiles}

Campaign Standardでは、割り当てられた製品プロファイルに関係なく、APIへの管理者権限が昇格されました。 Campaign v8では、別の製品プロファイルのセットが導入されるため、Campaign StandardからCampaign v8の製品プロファイルへのマッピングが必要になります。

移行を行うと、既存または事前に作成されたテクニカルアカウントに2つの製品プロファイルが追加されます。管理者とメッセージセンター（トランザクション APIにアクセスする場合）。 管理者の製品プロファイルをテクニカルアカウントにマッピングしない場合は、製品プロファイルマッピングを確認し、必要な製品プロファイルを割り当てます。

#### テナント ID

移行後、今後の統合を行う場合は、以前のCampaign Standard テナント IDを置き換えて、REST URLで&#x200B;**Campaign v8 テナント ID**&#x200B;を使用することをお勧めします。

#### キーの使用状況

PKey値の管理は、Campaign Standard v8とCampaign v8で異なります。 Campaign Standardを使用してPKeyを保存する場合は、以前のAPI呼び出しから取得したPKeyまたはhrefsを使用して、その後のAPI呼び出しを動的にフォーム化します。

### 利用可能なAPI {#available-apis}

現時点では、以下に示すREST APIを使用できます。

* **プロファイル**
* **サービスとサブスクリプション**
* **カスタムリソース**
* **ワークフロー**
* **トランザクションメッセージ**

>[!AVAILABILITY]
>
>以下に示すREST APIは非推奨（廃止予定）であり、使用できません。
>* マーケティング履歴
>* 組織単位
>* プライバシー管理

### フィルタリング {#rest-filtering}

* REST API ペイロードでフィルターを使用するには、Campaign v8でフィルターを編集し、ペイロードで使用する名前を指定する必要があります。 これを行うには、「**[!UICONTROL パラメーター]**」タブからフィルターの追加パラメーターにアクセスし、「**[!UICONTROL REST APIのフィルター名]**」フィールドに目的の名前を入力します。

  ![](assets/api-filtering.png)


* カスタムフィルターを使用するために必要な「by」プレフィックスは不要になりました。 フィルター名は、リクエストでそのまま使用する必要があります。

  例：

  `GET https://mc.adobe.io/<ORGANIZATION>/campaign/profileAndServicesExt/<resourceName>/<customFilterName>?<customFilterparam>=<customFilterValue>`

### ドロップされたデータベースフィールド {#dropped-fields}

データベースの一部のフィールドは、移行中に削除されています。 ドロップされたフィールドを使用する場合、REST APIは空白の値を返します。 今後、ドロップされたすべてのフィールドは非推奨となり、削除されます。

### リンクされたリソースを投稿 {#post-linked}

次のリクエスト本文フォーマットを使用する場合、「vehicleOwner」は「nms:recipient」へのリンクを表します。

```
{
    "vehicleNumber": "20009",
    "vehicleName": "Model E",
    "vehicleOwner":{
        "firstName":"tester 11",
        "lastName":"Smith 11"
    }
}
```

リンク情報は無視されます。 したがって、「vehicleNumber」と「vehicleName」の値のみを含む「cusVehicle」の下に新しいレコードが生成されます。 ただし、リンクはnullのままであるため、「vehicleOwner」はnullに設定されます。

Campaign v8では、同じリクエスト本文構造が使用され、「vehicle」がプロファイルにリンクされている場合、エラーが発生します。 このエラーは、「firstName」プロパティが「cusVehicle」に対して有効であると認識されないために発生します。 ただし、リンクのない属性のみを含むリクエスト本文は問題なく機能します。

### PATCH オペレーション {#patch}

* Campaign v8は、空のリクエスト本文を持つPATCHをサポートしていません。204 No Content ステータスを返します。
* Campaign Standardは、スキーマ内のエレメントや属性に対してPATCHをサポートしていますが、Campaign v8では場所に対するPATCH操作はサポートされていないことに注意してください。 場所でPATCHを試すと、「zipCode」プロパティが「profile」リソースに対して無効であることを示すエラーメッセージが表示され、500内部サーバーエラーが発生します。

### REST応答 {#rest-responses}

以下の節では、Campaign Standardとv8 REST応答の間の小さな違いを示します。

* 単一のGET レコードの場合、応答にはhrefが含まれます。
* 属性を使用してクエリを実行すると、Campaign v8は応答にカウントとページネーションを提供します。
* POST操作の後、リンクされたリソースの値が応答で返されます。

### エラーコードとメッセージ {#rest-errors}

以下の節では、Campaign StandardとCampaign v8 エラーコードおよびメッセージの違いを示します。

| シナリオ | Campaign Standard | Campaign v8 |
|  ---  |  ---  |  ---  |
| リクエスト本文で無効なPKeyを使用する | 500 - &#39;O5iRp40EGA&#39;属性が不明です（「プロファイル （nms:recipient）」スキーマの定義を参照）。 XTK-170036式「@id = @O5iRp40EGA」を解析できません。 | 404 - PKeyを復号できません。 （PKey=@jksad） |
| URIで無効なPKeyを使用する | 500 - &#39;O5iRp40EGA&#39;属性が不明です（「プロファイル （nms:recipient）」スキーマの定義を参照）。 XTK-170036式「@id = @O5iRp40EGA」を解析できません。 | 404 - PKeyを復号できません。 （PKey=@jksad）サポートされていないエンドポイント。 （endpoint=rest/profileAndServices/profile/@jksad） |
| URIとリクエスト本文で2つの異なる生のPkeyを使用する | 500 - RST-360011 エラーが発生しました – 管理者にお問い合わせください。 RST-360012 リソース「サービス」に対する一貫性のない操作 – キー「SVC3」を「SVC4」に更新できません。 | 500 - エラーが発生しました – 管理者にお問い合わせください。 |
| URIにPKey、リクエスト本文に別の生のPKeyを使用する | 500 – 同じキー「SVC4」を持つ「Service」が既に存在します。 PGS-220000 PostgreSQL エラー：エラー：重複するキーの値が一意の制約「nmsservice_name」の詳細：キー（sname）=（SVC4）が既に存在します。 | 500 - エラーが発生しました – 管理者にお問い合わせください。 |
| URIでの既存でないRaw-IDの使用 | 404 - RST-360011 エラーが発生しました – 管理者にお問い合わせください。 キー「adobe_nl:0」（スキーマ「service」および名前「adobe_nl」を持つドキュメント）からパス「Service」を持つドキュメントが見つかりません | 404 - キー「adobe_nl」（スキーマ「service」および名前「adobe_nl」を持つドキュメント）からパス「Service」を持つドキュメントが見つかりません |
| リクエスト本文で既存でないRaw-IDを使用している | 404 - RST-360011 エラーが発生しました – 管理者にお問い合わせください。 キー「adobe_nl」（スキーマ「service」および名前「adobe_nl」を持つドキュメント）からパス「Service」を持つドキュメントが見つかりません | 404 - キー「adobe_nl」（スキーマ「service」および名前「adobe_nl」を持つドキュメント）からパス「Service」を持つドキュメントが見つかりません |
| - | 500 - RST-360011 エラーが発生しました – 管理者にお問い合わせください。 | 500 - エラーが発生しました – 管理者にお問い合わせください。 |
| 無効な性別（または任意の）列挙値を持つプロファイル/サービスを挿入する | 500 - RST-360011 エラーが発生しました – 管理者にお問い合わせください。 値「invalid」は、「@gender」フィールドの「nms:recipient:gender」列挙に対して無効です | 500 - エラーが発生しました – 管理者にお問い合わせください。 |

### プロファイルタイムゾーンとccpaOptOut {#profile-timezone}

Campaign Standardでは、タイムゾーンは&#x200B;**profileAndServices/profile** REST API呼び出しのJSON応答の一部として表示されます。

Campaign v8では、タイムゾーンは&#x200B;**profileAndServicesExt/profile** REST API呼び出しの一部としてのみユーザーに表示されます。 拡張スキーマに追加されているため、**profileAndServices/profile** REST API呼び出しの一部ではありません。

同じことが`ccpaOptOut` フィールドにも当てはまります。データ移行の一環として拡張スキーマに追加されるので、**profileAndServices/profile**&#x200B;呼び出しではなく、**profileAndServicesExt/profile** REST API呼び出しの一部としてのみ表示されます。

### ワークフローの外部シグナル {#workflow-signals}

Campaign Standard Workflow GET APIは、ワークフローインスタンス変数およびそのデータタイプ（ブール値、文字列など）などのパラメーター名を返します。 これは、POST API呼び出しを介してシグナルをトリガーする際に、適切な形式のJSON リクエスト本文を作成するために使用されます。

Campaign v8は、広告ワークフローインスタンス変数をサポートしていませんが、開発者がそれらの変数を理解していることを期待しています。 したがって、移行後、POST リクエスト本文のパラメーター情報は、GET API応答のパラメーター情報を利用せずに構築する必要があります。
