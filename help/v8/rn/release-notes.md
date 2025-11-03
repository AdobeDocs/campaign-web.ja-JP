---
title: Campaign v8 web ユーザーインターフェイスリリースノート
description: 最新の Campaign web ユーザーインターフェイスリリースで提供される新機能について説明します
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 934a37cfebfacd2df0b7610285252d883611f252
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 64%

---

# リリースノート {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="リリースノート"
>abstract="Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。これにより、Campaign リリースノートは月に数回更新され、最新の機能、改善点、修正が含まれます。定期的に確認することをお勧めします。"

Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。したがって、これらのリリースノートは月に数回更新されます。定期的に確認してください。

以前のリリースで利用可能な変更と改善点について詳しくは、[2024](release-notes-24.md) ページと [2025](release-notes-25.md) ページを参照してください。

## 2025 年 10 月リリース {#25-10-updates}

_2025 年 10 月 28 日_

<table>
<thead>
<tr>
<th><strong>トランザクションメッセージ、プッシュ通知、SMS （LA）の多言語機能</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Campaign web ユーザーインターフェイスで、複数のトランザクションメッセージ、プッシュ通知、SMS メッセージを異なる言語で送信できるようになりました。 多言語配信機能を使用すると、配信のデフォルト言語と、配信を送信できる様々な言語を選択できます。また、選択した言語でこれらの配信をプレビューすることもできます。</p>
<p>メモ：この機能は一連の組織でのみ使用でき（使用制限あり）、今後のリリースでグローバルにロールアウトされます。</p>
<p>詳しくは、<a href="../msg/multilingual.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<!--
* Enable OOTB File Upload for Multi-lingual Push Notification Deliveries. 
-->

<table>
<thead>
<tr>
<th><strong>トランザクションメッセージ（LA）でのプロファイルエンリッチメント</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>この機能では、Adobe Campaign データベースフィールドをメッセージのコンテンツにリンクすることによって、トランザクションメッセージをパーソナライズできます。 ターゲットマッピング、エンリッチメント列および紐付けキーを選択して、パフォーマンスのしきい値を維持しながら、正確でリアルタイムのパーソナライゼーションを行うことができます。</p>
<p>メモ：この機能は一連の組織でのみ使用でき（使用制限あり）、今後のリリースでグローバルにロールアウトされます。 この機能は現在、メールでのみ使用できます。</p>
<p>詳しくは、<a href="../transactional-messaging/profile-enrichment.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Adobe GenStudioとの統合</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>これで、マーケティング効率を高め、ブランドの一貫性を保つために、GenStudio for Performance Marketingのエクスペリエンスを Campaign とシームレスに統合できるようになりました。 これにより、Campaign の高度なオーケストレーション機能と共に、GenStudioの AI を活用したコンテンツ作成を活用できます。<p>
<p>詳しくは、<a href="../integrations/genstudio.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>メールデザイナーでのダークモードのサポート</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>メールDesignerで、ダークモード表示に切り替える機能が追加されました。このビューで、特定のカスタム設定を追加で定義できます。 最終的なレンダリングは受信者のメールクライアントに依存し、すべてのメールクライアントがダークモードをサポートしているわけではありません。</p>
<p>詳しくは、<a href="../email/accessible-content.md#dark-mode">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<!-- table>
<thead>
<tr>
<th><strong>Continuous delivery activity</strong><br/></th> not ready
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Continuous delivery activity</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

### 機能強化 {#25-10-improvements}

* クライアントコンソールで作成した配信の「**オーディエンス**」セクションに、配達確認ターゲットに対する動的条件が定義されているかどうかを示すようになりました。<!-- [Learn more](../msg/gs-deliveries.md#access)-->

* メールDesignerの条件付きコンテンツ機能を使用して条件を設定する際に、新しいルールビルダーと従来のルールビルダーを切り替えられるようになりました。<!-- [Learn more](../personalization/conditions.md#condition-condition-builder)-->

* 受信者スキーマの画面定義で、購入などのコレクションリンクを選択できるようになりました。 専用のタブを使用して、プロファイル画面に関連データが表示されます。<!-- [Learn more](../administration/schemas.md#collection-lists)-->

* Campaign 管理者は、Salesforce CRM とMicrosoft Dynamicsへの接続を設定できるようになりました。
  [詳細情報](../administration/external-crm.md)

<!--
* Stop button for deliveries not linked to release and no info
-->

