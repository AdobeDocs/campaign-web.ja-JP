---
audience: end-user
title: 詳細設定
description: Campaign v8 Web ドキュメント
source-git-commit: c90d8a5eff6169945d381f3250cb3e4d06194d31
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 40%

---

# 詳細設定 {#advanced-settings}

>[!NOTE]
>
>このドキュメントは作成中で、頻繁に更新されています。 このコンテンツの最終バージョンは、2023 年 1 月に準備が整います。

これらの設定は、E メールテンプレートで定義される技術的な配信パラメーターです。 特定の配信に対していずれかの変更を行う場合は、注意して作業を進めてください。

## E メール配信設定 {#email-delivery-settings}

<!--
October 2022 

Note that this page is for now a placeholder to host Contextualhelp blocks

Do not delete these blocks 

Documentation on this part is targeted for december 2022
-->

テンプレートからのすべての技術的な配信パラメーター。
パラメーターのみを変更し、ここには作成しません。
権限に従い、Practers はこの変更を行わないでください。 テンプレートで定義されたタイポロジルール —> rest のみを確認して変更します。

## タイポロジ {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="タイポロジ"
>abstract="タイポロジを使用すると、配信を制御、フィルターおよび監視できます。"

### 頻度パラメーター {#pressure-parameter}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_weight"
>title="配信の重み付け"
>abstract="配信に重みを付けることで、頻度管理のフレームワーク内で最も優先順位の高い配信を指定できます。最も大きな重みを付けられたメッセージが、最優先されます。"

### 処理能力設定 {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_recipient_importance"
>title="受信者の重要度"
>abstract="TBC"


## オーディエンス {#audience}

## 配信 {#delivery}

### 再試行 {#retries}

>[!CONTEXTUALHELP]
>id="acw_email_settings_retries"
>title="再試行の最大数"
>abstract="一時的なエラーが原因でメッセージ送信が失敗した場合、配信期間中に再試行がおこなわれます。"

## 承認 {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="承認 mode"
>abstract="配信の各手順では、様々なプロセスの監視と制御を完全におこなえるように、承認を受ける必要があります。"

## 有効性 {#validity}

### 有効期間 {#validity-period}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_duration"
>title="配信期間"
>abstract="「配信期間」フィールドには、グローバルでおこなう配信再試行の期限を入力できます。Adobe Campaign は、開始日にメッセージの送信を開始した後、エラーのみを返すメッセージについて、設定された定期的な再試行を、有効期限日に達するまで実行します。"

>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="リソースの有効期間"
>abstract="「有効期限」フィールドは、アップロードされたリソース（主にミラーページと画像）に関して使用されます。このページのリソースは、一定期間有効です。"


### トラッキング {#tracking}

>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="有効期間"
>abstract="このオプションは、URL で追跡を有効にする期間を定義します。"














