---
audience: end-user
title: Campaign web ユーザーインターフェイスでの権限管理
description: Campaign web ユーザーインターフェイスの権限について説明します
exl-id: c95b854b-ebbe-4985-8f75-fb6bc795a399
source-git-commit: 2feea0c5a1b021786e58bf6a69a2018ec37ea4b1
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 28%

---


# 権限 {#permissions}

Adobe Campaignの各ユーザーには、アプリケーションで独自の権限と制限があります。

ユーザーは、オペレーターグループの一部になることができ、グループの権限を継承します。

オペレーターは、権限に応じて次のことが可能です。

* 特定の機能へのアクセス
* 特定のデータへのアクセス
* 特定のアクション（作成、変更、削除）へのアクセス

## フォルダーに対する権限 {#folder-permissions}

ユーザーの権限に応じて、「フォルダー設定 **[!UICONTROL のフォルダーに対する権限を表示および管理でき]** す。
配信フォルダーの例を以下に示します。

![](assets/folder_settings.png){zoomable="yes"}

**[!UICONTROL フォルダー設定]** の「**[!UICONTROL セキュリティ]**」セクションでは、フォルダーにアクセスできるオペレーターまたはグループを表示および管理（追加または削除）できます。

![](assets/folder_security.png){zoomable="yes"}

権限を直接クリックして、変更 **[!UICONTROL 許可]** または **[!UICONTROL 拒否]** できます。

![](assets/folder_security_denied.png){zoomable="yes"}

「**[!UICONTROL 生成]**」オプションが有効になっている場合、フォルダーに定義されているすべての権限がそのすべてのサブフォルダーに適用されます。これらの権限は、サブフォルダーごとにオーバーロードできます。

「**[!UICONTROL システムフォルダー]**」オプションがオンの場合、権限に関係なく、すべてのオペレーターがアクセスできます。

また、[Adobe Campaign コンソールでフォルダーに対する権限を管理 ](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/admin/permissions/folder-permissions) することもできます。
Campaign web UI のすべての権限は、Campaign クライアントコンソールの権限と同期されます。
