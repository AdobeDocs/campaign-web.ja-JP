---
audience: end-user
title: トラップグループの使用
description: Campaign web ユーザーインターフェイスでの配信にトラップグループを使用する方法について説明します
source-git-commit: 39dcf11797339ee9800da6c5a32b1a1c3470529a
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 29%

---

# トラップグループの使用 {#trap-group}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="トラップグループ"
>abstract="トラップグループを使用して配信に特定のアドレスを含めることができ、定義したターゲット条件に一致しないプロファイルをターゲティングすることで配信プロセスを監視および検証できます。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=ja" text="リリースノートを参照してください"

**[!UICONTROL トラップグループ]** （**[!UICONTROL シードリスト]** とも呼ばれます）を使用して、定義したターゲット条件に一致しないプロファイルをターゲティングすることで配信プロセスを監視および検証するために、配信に特定のアドレスを含めます。 これにより、配信スコープ外の受信者が他のターゲット受信者と同様に配信を受信することができます。

**[!UICONTROL トラップグループ]** は、Campaign web ユーザーインターフェイス上の **[!UICONTROL テストプロファイル]** という名前の **[!UICONTROL シードアドレス]** のグループです。

## トラップグループを使用する理由 {#why-trap-group}

**[!UICONTROL trap group]** を使用できます。

1. **証拠として**:**[!UICONTROL トラップグループ]** の各メンバーは、オーディエンスの一部であるかのように配信を受け取ります。

1. **メーリングリストを保護するため**：オーディエンスが受け取るものを受け取ることで、**[!UICONTROL トラップグループ]** の各 **[!UICONTROL テストプロファイル]** は、メーリングリストがサードパーティによって使用されている場合に通知されます。

>[!NOTE]
>
>[ 配信の作成時に配達確認を送信する ](../email/create-email.md#preview-test) や [ コントロール母集団 ](control-group.md) に加えて、トラップグループを追加すると、オーディエンスをテストするのに適した方法です。

## トラップグループについて {#about-trap-group}

テストプロファイルは、**クリック数**、**開封数**、**購読解除**&#x200B;の配信統計に関するレポートからは自動的に除外されます。レポートは、実際のオーディエンスに関する内容のみです。

メール配信の場合、**[!UICONTROL トラップグループ]**&#x200B;のメールアドレスのみが必要で、他のフィールドのパーソナライゼーションは Campaign によってランダムに入力されます。

## 配信へのトラップグループの追加 {#trap-group-in-delivery}

**[!UICONTROL トラップグループ]**&#x200B;を設定するには、配信の&#x200B;**[!UICONTROL オーディエンス]**&#x200B;設定に移動します。次の 2 つのオプションがあります。

* [テストプロファイルを選択](#select-test-profile)
* [条件を作成](#create-condition)

![](assets/trap-group.png){zoomable="yes"}

### テストプロファイルを選択 {#select-test-profiles}

**テストプロファイルを選択** を選択すると、次に示すように **「テストプロファイルを追加」** ボタンを使用できます。

![](assets/trap-no-test-profile.png){zoomable="yes"}

ボタンをクリックすると、**[!UICONTROL トラップグループ]** を追加できるテストプロファイルにアクセスできます。 使用するものを選択します。

また、新しいテストプロファイルを作成することもできます。 [詳細情報](#create-seed)

![](assets/trap-select-test-profiles.png){zoomable="yes"}

テストプロファイルを確認したら、「**[!UICONTROL トラップグループ]**」に正しい番号が表示されていることを確認します。

![](assets/trap-check.png){zoomable="yes"}

### 条件を作成 {#create-condition}

**[!UICONTROL 条件の作成]** オプションを使用して、使用するテストプロファイルを定義するクエリを作成できます。

![](assets/trap-create-condition.png){zoomable="yes"}

クエリは **[!UICONTROL トラップグループ]** の下に表示されます。

![](assets/trap-custom.png){zoomable="yes"}

## 新しいテストプロファイルを作成 {#create-seed}

**[!UICONTROL エクスプローラー]**/**[!UICONTROL リソース]**/**[!UICONTROL 6}Campaign Management]**/**[!UICONTROL シードメンバー]** フォルダーから、新しいテストプロファイル ]**を作成できます。**[!UICONTROL 

![](assets/trap-create.png){zoomable="yes"}

任意のプロファイルと同様に、**[!UICONTROL テストプロファイル]** に関するすべての設定を指定します。

![](assets/trap-create-contact.png){zoomable="yes"}