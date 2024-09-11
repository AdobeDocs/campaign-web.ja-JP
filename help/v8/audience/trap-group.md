---
audience: end-user
title: トラップグループの使用
description: Campaign web ユーザーインターフェイスでの配信にトラップグループを使用する方法について説明します
exl-id: 48c34581-8825-4798-b24e-c462303f7645
source-git-commit: dfd5f2e000b02d4382eaac0c9bb00fe940a99f79
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 100%

---

# トラップグループの使用 {#trap-group}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn3"
>title="トラップグループ"
>abstract="トラップグループを使用すると、配信に特定のアドレスを含め、定義済みのターゲット条件に一致しないプロファイルをターゲットにすることで、配信プロセスを監視および検証できます。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=ja" text="リリースノートを参照してください"

**[!UICONTROL トラップグループ]**（**[!UICONTROL シードリスト]**&#x200B;とも呼ばれる）を使用すると、配信に特定のアドレスを含め、定義済みのターゲット条件に一致しないプロファイルをターゲットにすることで、配信プロセスを監視および検証できます。これにより、配信スコープ外の受信者が他のターゲット受信者と同様に配信を受信することができます。

**[!UICONTROL トラップグループ]**&#x200B;は、**[!UICONTROL シードアドレス]**&#x200B;のグループです。Campaign web ユーザーインターフェイスでは&#x200B;**[!UICONTROL テストプロファイル]**&#x200B;という名前になります。

## トラップグループを使用する理由 {#why-trap-group}

次の目的のために、**[!UICONTROL トラップグループ]**&#x200B;を使用できます。

1. **配達確認として**：**[!UICONTROL トラップグループ]**&#x200B;の各メンバーは、オーディエンスの一部であるかのように、配信を受信します。

1. **メーリングリストを保護するために**：オーディエンスと同じ内容を受信することで、サードパーティがメーリングリストを使用した場合、**[!UICONTROL トラップグループ]**&#x200B;の各&#x200B;**[!UICONTROL テストプロファイル]**&#x200B;に通知が送られます。

>[!NOTE]
>
>[配信の作成](../email/create-email.md#preview-test)や[コントロール母集団からの配達確認の送信](control-group.md)に加えて、トラップグループを追加することで、オーディエンスを適切にテストできます。

## トラップグループについて {#about-trap-group}

テストプロファイルは、**クリック数**、**開封数**、**購読解除**&#x200B;の配信統計に関するレポートからは自動的に除外されます。レポートは、実際のオーディエンスに関する内容のみです。

メール配信の場合、**[!UICONTROL トラップグループ]**&#x200B;のメールアドレスのみが必要で、他のフィールドのパーソナライゼーションは Campaign によってランダムに入力されます。

## 配信でのトラップグループの追加 {#trap-group-in-delivery}

**[!UICONTROL トラップグループ]**&#x200B;を設定するには、配信の&#x200B;**[!UICONTROL オーディエンス]**&#x200B;設定に移動します。次の 2 つのオプションがあります。

* [テストプロファイルを選択](#select-test-profile)
* [条件を作成](#create-condition)

![](assets/trap-group.png){zoomable="yes"}

### テストプロファイルを選択 {#select-test-profiles}

「**テストプロファイルを選択**」を選択する際、次に示すように「**テストプロファイルを追加**」ボタンを使用できます。

![](assets/trap-no-test-profile.png){zoomable="yes"}

ボタンをクリックすると、**[!UICONTROL トラップグループ]**&#x200B;を追加できるテストプロファイルにアクセスできます。使用するテストプロファイルを選択します。

また、新しいテストプロファイルを作成することもできます。[詳細情報](#create-seed)

![](assets/trap-select-test-profiles.png){zoomable="yes"}

テストプロファイルを確認する際は、**[!UICONTROL トラップグループ]**&#x200B;の番号が正しいことを確認します。

![](assets/trap-check.png){zoomable="yes"}

### 条件を作成 {#create-condition}

「**[!UICONTROL 条件を作成]**」オプションでは、クエリを作成して、使用するテストプロファイルを定義できます。

![](assets/trap-create-condition.png){zoomable="yes"}

クエリは、**[!UICONTROL トラップグループ]**&#x200B;の下に表示されます。

![](assets/trap-custom.png){zoomable="yes"}

## 新しいテストプロファイルの作成 {#create-seed}

**[!UICONTROL エクスプローラー]**／**[!UICONTROL リソース]**／**[!UICONTROL キャンペーン管理]**／**[!UICONTROL シードメンバー]**&#x200B;フォルダーから新しい&#x200B;**[!UICONTROL テストプロファイル]**&#x200B;を作成できます。

![](assets/trap-create.png){zoomable="yes"}

任意のプロファイルについて、**[!UICONTROL テストプロファイル]**&#x200B;に関するすべての設定を行います。

![](assets/trap-create-contact.png){zoomable="yes"}
