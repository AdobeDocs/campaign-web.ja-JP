---
audience: end-user
title: 読み取り専用ワークフローについて
description: ワークフローが読み取り専用モードである理由について説明します
exl-id: 5eaffe2c-7a9c-4508-8dd1-495cfcf99c59
source-git-commit: 58f25a6b41c89e97c0f721f4437b5245d16b3757
workflow-type: ht
source-wordcount: '225'
ht-degree: 100%

---

# 読み取り専用ワークフローについて {#readonly-workflows}

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="このワークフローは読み取り専用です"
>abstract="権限またはワークフローのタイプにより、このワークフローを編集できません。"

一部のワークフローは読み取り専用です。ビルトインテクニカルワークフローは常に読み取り専用ですが、この再構築は他のタイプのワークフローでもアクティブ化できます。

Campaign ユーザーは、Adobe Campaign データへのアクセスが制限されている場合があります。Campaign 管理者は、一部の機能を表示する権限を付与できますが、編集または変更する権限は付与できません。データとプロセスのセキュリティを確保するには、データに対するユーザー権限が重要です。Campaign の権限管理について詳しくは、[この節](../get-started/permissions.md)を参照してください。

ワークフローが読み取り専用モードの場合：

* 「**[!UICONTROL 設定]**」ボタンの近くにある「**[!UICONTROL 読み取り専用]**」という記載
* アクセスできないアクションボタン

![](assets/readonly-workflow.png){zoomable="yes"}

ユーザーは、読み取り専用ワークフローでは何も編集できません。アクティビティの設定は変更できません。

![](assets/scheduler-readonly.png){zoomable="yes"}

ユーザーは、ワークフローを削除することもできません。

![](assets/readonly-rights.png){zoomable="yes"}


## 読み取り専用ワークフローのタイプ {#readonly-workflow-types}

ワークフローのタイプに応じて、読み取り専用モードが異なる場合があります。

### キャンペーンワークフロー {#readonly-campaign-wf}

読み取り専用キャンペーンワークフローの場合、ユーザーは監視ボタンにアクセスできません。

![](assets/readonly-campaign-workflow.png){zoomable="yes"}

### テクニカルワークフロー {#readonly-tech-wf}

ビルトインテクニカルワークフローは、すべての Campaign ユーザー（管理者も含む）に対して読み取り専用です。ただし、ユーザーは、必要に応じて&#x200B;**一時停止**&#x200B;または&#x200B;**停止**&#x200B;することができます。許可されるアクションは以下に限られています。

![](assets/readonly-technical-workflow.png){zoomable="yes"}

テクニカルワークフローについて詳しくは、[この節](https://experienceleague.adobe.com/ja/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows)を参照してください。
