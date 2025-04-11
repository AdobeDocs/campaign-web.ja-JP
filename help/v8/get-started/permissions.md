---
audience: end-user
title: Campaign web ユーザーインターフェイスでの権限管理
description: Campaign web ユーザーインターフェイスの権限について説明します
exl-id: c95b854b-ebbe-4985-8f75-fb6bc795a399
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 14%

---

# 権限 {#permissions}

Adobe Campaignの各ユーザーには、アプリケーションで固有の権限と制限があります。 ユーザーはオペレーターグループに属し、グループの権限を継承することができます。

オペレーターは、権限に基づいて、次の操作を実行できます。

* 特定の機能へのアクセス
* 特定のデータへのアクセス
* 特定のアクションへのアクセス（作成、変更、削除）

Adobe Campaignで権限を設定する手順について詳しくは、[Adobe Campaign v8 （コンソール）ドキュメント ](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"} を参照してください。

## フォルダーに対する権限 {#folder-permissions}

権限に基づいて、**[!UICONTROL フォルダー設定]** でフォルダーに対する権限を表示および管理できます。

配信フォルダーの例を次に示します。

![Adobe Campaignのフォルダー設定の例 ](assets/folder_settings.png){zoomable="yes"}

**[!UICONTROL フォルダー設定]** の **[!UICONTROL セキュリティ]** セクションでは、フォルダーにアクセスできるオペレーターまたはグループを表示および管理（追加または削除）できます。

![Adobe Campaignにおけるフォルダーセキュリティ設定の例 ](assets/folder_security.png){zoomable="yes"}

権限を直接クリックして、それらを **[!UICONTROL 許可]** または **[!UICONTROL 拒否]** に変更できます。

![ フォルダーセキュリティ設定での拒否された権限の例 ](assets/folder_security_denied.png){zoomable="yes"}

「**[!UICONTROL サブフォルダーにも反映]** オプションが有効になっている場合は、フォルダーに対して定義されているすべての権限が、そのフォルダーのすべてのサブフォルダーに適用されます。 これらの権限は、サブフォルダーごとに上書きできます。

**[!UICONTROL システムフォルダー]** オプションが選択されている場合、権限に関係なく、すべてのオペレーターがアクセスできます。

また、[Adobe Campaign コンソールでフォルダーの権限を管理](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/admin/permissions/folder-permissions){target="_blank"}することもできます。

Campaign web ユーザーインターフェイスのすべての権限は、Campaign クライアントコンソールの権限と同期されます。