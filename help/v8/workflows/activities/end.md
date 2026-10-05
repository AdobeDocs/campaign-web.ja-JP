---
audience: end-user
title: 終了ワークフローアクティビティの使用
description: 終了ワークフローアクティビティの使用方法について説明します
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
source-git-commit: 4fa6c49fb2456ef2edeb3f609b77c0cc5d33b95e
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 100%
---
# 終了 {#end}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="終了アクティビティ"
>abstract="**終了**&#x200B;アクティビティを使用すると、ワークフローの終了を視覚的に示すことができます。 複数のインバウンドトランジションが使用可能な場合は、「**結合の設定**」セクションを使用して、アクティビティに接続するトランジションを選択します。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_end_sets"
>title="結合の設定"
>abstract="**終了**&#x200B;アクティビティのインバウンドトランジションとして接続する、以前のアクティビティをオンにします。 オンにしたアクティビティが&#x200B;**終了**&#x200B;に接続されます。 このセクションは、アクティビティに接続できるインバウンドトランジションが複数存在する場合にのみ表示されます。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_signal"
>title="外部シグナル"
>abstract="終了アクティビティパラメーターにおける、外部信号セクションのプレースホルダー。 オーケストレーションキャンペーンでのみ使用できます。 削除しない"

**終了**&#x200B;アクティビティは&#x200B;**フロー制御**&#x200B;アクティビティです。 ワークフローの終了をグラフィカルにマークできます。 このアクティビティはオプションです。

アクティビティは、複数のインバウンドトランジションが使用可能な場合にサポートします。

「**結合の設定**」セクションで、**終了**&#x200B;アクティビティのインバウンドトランジションとして接続する、以前のアクティビティをオンにします。 オンにしたアクティビティがワークフローキャンバスの&#x200B;**終了**&#x200B;にリンクされます。

![ワークフローの重複排除の設定プロセス](../assets/workflow-end.png)
