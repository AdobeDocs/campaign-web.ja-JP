---
audience: end-user
title: 読み取り専用ワークフローについて
description: ワークフローが読み取り専用モードである理由について説明します
exl-id: 5eaffe2c-7a9c-4508-8dd1-495cfcf99c59
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 18%

---

# 読み取り専用ワークフローについて {#readonly-workflows}

>[!CONTEXTUALHELP]
>
一部のワークフローは読み取り専用です。 ビルトインテクニカルワークフローは常に読み取り専用ですが、この制限は他のタイプのワークフローにも適用されます。

Campaign ユーザーは、Adobe Campaign データへのアクセスを制限されている場合があります。 Campaign 管理者は、特定の機能を表示する権限を付与できますが、編集や変更の権限は付与できません。 データとプロセスのセキュリティを確保するには、データに対するユーザー権限が不可欠です。 Campaign での権限管理について詳しくは、[ この節 ](../get-started/permissions.md) を参照してください。

ワークフローが読み取り専用モードの場合：

* メンション **[!UICONTROL 読み取り専用]** が「**[!UICONTROL 設定]** ボタンの近くに表示されます。
* アクションボタンにアクセスできません。

![ 設定ボタンと無効なアクションボタンを示す読み取り専用ワークフローインターフェイス ](assets/readonly-workflow.png){zoomable="yes"}

ユーザーは、読み取り専用ワークフローでは何も編集できません。アクティビティの設定を変更することはできません。

![ 読み取り専用モードのスケジューラーインターフェイス。無効な設定オプションが表示されます。](assets/scheduler-readonly.png){zoomable="yes"}

ユーザーはワークフローを削除できません。

![ ワークフローを削除するための制限付きの権限を示すインターフェイス ](assets/readonly-rights.png){zoomable="yes"}

## 読み取り専用ワークフローのタイプ {#readonly-workflow-types}

ワークフローのタイプによって、読み取り専用モードは異なる場合があります。

### キャンペーンワークフロー {#readonly-campaign-wf}

読み取り専用のキャンペーンワークフローでは、ユーザーは「監視」ボタンにアクセスできません。

![ 読み取り専用モードの Campaign ワークフローインターフェイスに、無効な監視オプションが表示される。](assets/readonly-campaign-workflow.png){zoomable="yes"}

### テクニカルワークフロー {#readonly-tech-wf}

ビルトインテクニカルワークフローは、管理者を含むすべての Campaign ユーザーに対して読み取り専用です。 ただし、ユーザーは、必要に応じて&#x200B;**一時停止**&#x200B;または&#x200B;**停止**&#x200B;することができます。許可されているアクションはこれだけです。

![ 読み取り専用モードのテクニカルワークフローインターフェイス。ワークフローを一時停止または停止するオプションが表示されます ](assets/readonly-technical-workflow.png){zoomable="yes"}。

テクニカルワークフローについて詳しくは、[ この節 ](https://experienceleague.adobe.com/ja/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows) を参照してください。