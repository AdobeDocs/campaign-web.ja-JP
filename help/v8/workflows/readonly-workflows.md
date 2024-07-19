---
audience: end-user
title: 読み取り専用ワークフローについて
description: ワークフローが読み取り専用モードである理由について説明します
exl-id: 5eaffe2c-7a9c-4508-8dd1-495cfcf99c59
source-git-commit: 89633454bb3de1ac05d37d767df45d9d143c80b5
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 100%

---

# 読み取り専用ワークフローについて {#readonly-workflows}

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="このワークフローは読み取り専用です"
>abstract="権限またはワークフローのタイプにより、このワークフローを編集できません。"

一部のワークフローは、読み取り専用モードになっている場合があります。次を使用して確認できます。

- 「**[!UICONTROL 設定]**」ボタンの近くにある「**[!UICONTROL **&#x200B;読み取り専用&#x200B;**]**」という記載
- アクセスできないアクションボタン

![](assets/readonly-workflow.png){zoomable="yes"}

読み取り専用ワークフローでは何も編集できません。アクティビティの設定は変更できません。


![](assets/scheduler-readonly.png){zoomable="yes"}


また、ワークフローを削除する権限もありません。

![](assets/readonly-rights.png){zoomable="yes"}

## 読み取り専用ワークフローを使用する理由

読み取り専用モードは、ワークフローを編集する権限やアクセス権を持たないユーザー用です。[詳しくは、こちらを参照してください](../get-started/permissions.md)

キャンペーンユーザーには、Adobe Campaign でアクセスできるデータに制限がある場合があります。管理者は、ユーザーに一部の機能を表示する権限を付与できますが、これらの機能を操作する権限は付与できません。

## 読み取り専用ワークフローのタイプ

ワークフローのタイプに応じて、読み取り専用モードが異なる場合があります。

### キャンペーンワークフロー

読み取り専用キャンペーンワークフローの場合、ユーザーは監視ボタンにアクセスできません。

![](assets/readonly-campaign-workflow.png){zoomable="yes"}

### テクニカルワークフロー

テクニカルワークフローは、キャンペーンユーザーに対して読み取り専用モードになります。
ビルトインのテクニカルワークフローは、管理者ユーザーも含め、すべてのユーザーに対して読み取り専用モードになります。ただし、ユーザーは必要に応じて**一時停止**&#x200B;または&#x200B;**停止**&#x200B;することができます。許可されるアクションは以下に限られています。[詳しくは、こちらを参照してください](https://experienceleague.adobe.com/ja/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows)

![](assets/readonly-technical-workflow.png){zoomable="yes"}
