---
audience: end-user
title: トラップグループの使用
description: Campaign web ユーザーインターフェイスでの配信にトラップグループを使用する方法について説明します
exl-id: 48c34581-8825-4798-b24e-c462303f7645
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 35%

---

# トラップグループの使用 {#trap-group}

**[!UICONTROL トラップグループ]**（**[!UICONTROL シードリスト]**&#x200B;とも呼ばれる）を使用すると、配信に特定のアドレスを含め、定義済みのターゲット条件に一致しないプロファイルをターゲットにすることで、配信プロセスを監視および検証できます。これにより、配信スコープ外の受信者も、他のターゲット受信者と同様に配信を受信できます。

**[!UICONTROL トラップグループ]** は、Campaign web ユーザーインターフェイス上の **[!UICONTROL テストプロファイル]** という名前の **[!UICONTROL シードアドレス]** のグループです。

## トラップグループを使用する理由 {#why-trap-group}

**[!UICONTROL トラップグループ]** を使用できます。

1. **証拠として**:**[!UICONTROL トラップグループ]** の各メンバーは、オーディエンスの一部であるかのように配信を受け取ります。

1. **メーリングリストを保護するため**：オーディエンスが受け取るものを受け取ることで、**[!UICONTROL トラップグループ]** の各 **[!UICONTROL テストプロファイル]** は、メーリングリストがサードパーティによって使用されている場合に通知されます。

>[!NOTE]
>
>[配信の作成](../email/create-email.md#preview-test)や[コントロール母集団からの配達確認の送信](control-group.md)に加えて、トラップグループを追加することで、オーディエンスを適切にテストできます。

## トラップグループについて {#about-trap-group}

テストプロファイルは、**クリック数**、**開封数**、**購読解除**&#x200B;の配信統計に関するレポートからは自動的に除外されます。レポートは、実際のオーディエンスに焦点を当てています。

メール配信の場合、**[!UICONTROL トラップグループ]** に必要なのはメールアドレスのみです。 他のフィールドのパーソナライゼーションは、Campaign によってランダムに入力されます。

## 配信でのトラップグループの追加 {#trap-group-in-delivery}

**[!UICONTROL トラップグループ]** を設定するには、配信の **[!UICONTROL オーディエンス]** 設定に移動します。 次の 2 つのオプションがあります。

* [テストプロファイルを選択](#select-test-profiles)
* [条件を作成](#create-condition)

[ トラップグループ設定インターフェイスのスクリーンショット ](assets/trap-group.png){zoomable="yes"}

### テストプロファイルを選択 {#select-test-profiles}

**テストプロファイルを選択** を選択する場合は、次に示すように **「テストプロファイルを追加**」ボタンを使用します。

[ テストプロファイルを追加ボタンのスクリーンショット ](assets/trap-no-test-profile.png){zoomable="yes"}

このボタンをクリックすると、テストプロファイルにアクセスして **[!UICONTROL トラップグループ]** に追加できます。 使用するテストプロファイルを選択します。

また、新しいテストプロファイルを作成することもできます。[詳細情報](#create-seed)

[ テストプロファイルインターフェイスのスクリーンショットを選択 ](assets/trap-select-test-profiles.png){zoomable="yes"}

テストプロファイルを確認したら、「**[!UICONTROL トラップグループ]**」の下に正しい番号が表示されていることを確認します。

[ トラップグループ確認のスクリーンショット ](assets/trap-check.png){zoomable="yes"}

### 条件を作成 {#create-condition}

**[!UICONTROL 条件の作成]** オプションを使用して、使用するテストプロファイルを定義するクエリを作成します。

[ 条件インターフェイスのスクリーンショットを作成 ](assets/trap-create-condition.png){zoomable="yes"}

クエリは、**[!UICONTROL トラップグループ]**&#x200B;の下に表示されます。

[ トラップグループクエリの表示スクリーンショット ](assets/trap-custom.png){zoomable="yes"}

## 新しいテストプロファイルの作成 {#create-seed}

新しい **[!UICONTROL テストプロファイル]** は、**[!UICONTROL エクスプローラー]**/**[!UICONTROL リソース]**/**[!UICONTROL キャンペーン管理]**/**[!UICONTROL シードメンバー]** フォルダーから作成できます。

[ テストプロファイルナビゲーションのスクリーンショットの作成 ](assets/trap-create.png){zoomable="yes"}

**[!UICONTROL テストプロファイル]** のすべての設定を、他のプロファイルの場合と同様に設定します。

[ テストプロファイル設定のスクリーンショット ](assets/trap-create-contact.png){zoomable="yes"}