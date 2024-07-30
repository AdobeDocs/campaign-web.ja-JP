---
audience: end-user
title: トラップグループの使用
hide: true
hidefromtoc: true
description: Campaign web ユーザーインターフェイスでの配信にトラップグループを使用する方法について説明します
source-git-commit: 2feea0c5a1b021786e58bf6a69a2018ec37ea4b1
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 48%

---

# **[!UICONTROL トラップグループ]**&#x200B;の使用 {#trap-group}

**[!UICONTROL トラップグループ]** （**[!UICONTROL シードリスト]** とも呼ばれます）を使用して、定義したターゲット条件に一致しないプロファイルをターゲティングすることで配信プロセスを監視および検証するために、配信に特定のアドレスを含めます。 これにより、配信スコープ外の受信者が他のターゲット受信者と同様に配信を受信することができます。
**[!UICONTROL トラップグループ]** は、AC Web UI 上の **[!UICONTROL テストプロファイル]** という名前の **[!UICONTROL シードアドレス]** のグループです。

## **[!UICONTROL トラップ グループ]** を使用する理由

次の目的のために、**[!UICONTROL トラップグループ]**&#x200B;を使用できます。

1. **配達確認として**：**[!UICONTROL トラップグループ]**&#x200B;の各メンバーは、オーディエンスの一部と同様に配信を受信します。


1. **メーリングリストを保護するため**：オーディエンスが受け取るものを受け取ると、**[!UICONTROL トラップグループ]** の各 **[!UICONTROL テストプロファイル]** が、メーリングリストがサードパーティによって使用されているかどうかを通知されます。

>[!NOTE]
>
>トラップグループは、[ 配信の作成時に配達確認を送信する ](../email/create-email.md#preview-test) および [ コントロールグループ ](control-group.md) とは異なります。


## **[!UICONTROL トラップグループ]**&#x200B;について

テストプロファイルは、**クリック数**、**開封数**、**購読解除**&#x200B;の配信統計に関するレポートからは自動的に除外されます。レポートは、実際のオーディエンスに関する内容のみです。

メール配信の場合、**[!UICONTROL トラップグループ]**&#x200B;のメールアドレスのみが必要で、他のフィールドのパーソナライゼーションは Campaign によってランダムに入力されます。

## 配信で&#x200B;**[!UICONTROL トラップグループ]**&#x200B;を設定する方法

**[!UICONTROL トラップグループ]**&#x200B;を設定するには、配信の&#x200B;**[!UICONTROL オーディエンス]**&#x200B;設定に移動します。次の 2 つのオプションがあります。
- [テストプロファイルを選択](#select-test-profile)
- [条件を作成](#create-condition)

![](assets/trap-group.png){zoomable="yes"}

### テストプロファイルを選択 {#select-test-profiles}

「テストプロファイルを選択」を選択すると、以下のようなウィンドウが表示され、**[!UICONTROL テストプロファイルを追加]**&#x200B;するように促されます。

![](assets/trap-no-test-profile.png){zoomable="yes"}

ボタンをクリックすると、**[!UICONTROL トラップグループ]** を追加できるテストプロファイルにアクセスできます。 使用するシードアドレスをオンにします。
新しいテストプロファイルを作成できます。 [詳細情報](#create-seed)

![](assets/trap-select-test-profiles.png){zoomable="yes"}

テストプロファイルを確認したら、「**[!UICONTROL トラップグループ]**」に正しい番号が表示されていることを確認します。

![](assets/trap-check.png){zoomable="yes"}

### 条件を作成 {#create-condition}

**[!UICONTROL 条件を作成]** を選択すると、新しいウィンドウが表示され、使用するテストプロファイルを定義するクエリをカスタムできます。

![](assets/trap-create-condition.png){zoomable="yes"}

クエリは、**[!UICONTROL トラップグループ]**&#x200B;の下に表示されます。

![](assets/trap-custom.png){zoomable="yes"}

## 新しい **[!UICONTROL テストプロファイル]** の作成方法 {#create-seed}

**[!UICONTROL エクスプローラー]**/**[!UICONTROL リソース]**/**[!UICONTROL 6}Campaign Management]**/**[!UICONTROL シードメンバー]** で、新しいテストプロファイル ]**を作成できます**[!UICONTROL 

![](assets/trap-create.png){zoomable="yes"}

**[!UICONTROL テストプロファイル]** に関するすべての詳細を、オーディエンスプロファイルのように入力できます。

![](assets/trap-create-contact.png){zoomable="yes"}