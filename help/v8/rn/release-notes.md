---
title: 最新のリリースノート
description: Campaign Web ユーザーインターフェイスに含まれている新機能を確認する
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 9%

---

# リリースノート {#latest-release}


>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="新機能"
>abstract="Adobe Campaignの Web ユーザーインターフェイスリリースは、機能のデプロイメントに向けて、よりスケーラブルで段階的なアプローチを可能にする、継続的な配信モデルで動作します。 リリースノートは月に数回更新されます。 **3 月のリリースがリリースされました**（ダイレクトメールチャネル、新しいデータソースの変更ワークフローアクティビティ、その他の機能強化を含む）。"


<!--Last update: **March 19, 2024**-->

Adobe Campaignの Web ユーザーインターフェイスリリースは、機能のデプロイメントに向けて、よりスケーラブルで段階的なアプローチを可能にする、継続的な配信モデルで動作します。 したがって、これらのリリースノートは月に数回更新されます。 定期的に確認してください。

>[!AVAILABILITY]
>
>このバージョンは、開始するすべてのユーザーが利用できます [Campaign （コンソール） v8.6 リリース](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=ja). Adobe Campaign Client Console のリリースとアップグレードについて詳しくは、 [Campaign v8（コンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=ja){target="_blank"}.

## 3 月のリリースノート {#24-3-release}

**リリース日**:2024 年 3 月 19～20 日

### ダイレクトメールチャネル {#24-3-dm}

**ダイレクトメール** チャネルは、ワークフローで、またはスタンドアロン配信として使用できるようになりました。 ダイレクトメールは、抽出ファイルの作成、パーソナライズ、生成、ダイレクトメールプロバイダーとの間での共有、顧客へのメール送信を可能にするオフラインチャネルです。 [詳細情報](../direct-mail/gs-direct-mail.md)

![](../assets/do-not-localize/direct-mail.gif)

### 新しい「データソースを変更」ワークフローアクティビティ {#24-3-change-data-source}

The **データソースを変更** ターゲティングアクティビティを使用すると、ワークフローの作業用テーブルで使用されるデータソースを変更できます。 このアクティビティでは、様々なデータベース間でデータを管理し、パフォーマンスを向上させることで、より柔軟にデータを管理できます。 [詳細情報](../workflows/activities/change-data-source.md)

![](../assets/do-not-localize/change-data-source.gif)

### ワークフローアクティビティの改善を分割 {#24-3-split}

これで、 **同じテーブルにすべてのサブセットを生成** オプションを **分割** すべてのサブセットを 1 つの出力トランジションにグループ化するワークフローアクティビティ。 [詳細情報](../workflows/activities/split.md)

### クエリモデラー {#24-3-query-modeler}

* クエリモデラーを E メールデザイナーで使用できるようになりました。 条件付きコンテンツを作成する際に、条件を作成できます。 [詳細情報](../personalization/conditions.md)
* カスタム条件を作成する際に、日付タイプの属性で事前定義された値を使用できるようになりました。 [詳細情報](../query/build-query.md)
* ダイアグラム内の新しいトランジションにオペレーターを追加できなくなりました。 これらは、コンポーネントをフィルタリングしてグループ化する前に、既存のトランジションに対してのみ追加できます。 [詳細情報](../query/build-query.md)
