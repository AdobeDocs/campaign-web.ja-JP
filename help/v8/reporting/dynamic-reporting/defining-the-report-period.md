---
title: レポート期間の定義
description: レポートの期間を使用すると、選択した日付に応じてデータをフィルターできます。
audience: end-user
level: Intermediate
exl-id: 36506f7d-aeeb-41cf-b971-6e42e1c7cdc8
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
source-git-commit: 4fa6c49fb2456ef2edeb3f609b77c0cc5d33b95e
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 100%
---
# レポート期間の定義{#defining-the-report-period}

>[!NOTE]
>
>データレポートは過去 13 か月間に対して使用できます。 データ保持期間について詳しくは、アドビコンサルタントまたは技術管理者にお問い合わせください。

レポートを開始またはレポートにアクセスする前に、期間を適用する必要があります。 指定された期間はレポートの右上に表示されます。

デフォルトでは、キャンペーンまたはプログラムの場合、フィルター期間はプログラムまたはキャンペーンの開始日と終了日に設定されます。 配信の場合、開始日は送信日に、終了日は送信日に 7日を加えた日付になります。

フィルターを変更するには、開始日と期間を選択するか、または事前に設定された期間（先週、2 か月前など）を使用します。

フィルターを適用または変更すると、レポートが自動的に更新されます。 選択したレポート期間によって管理されるのは、その期間内に作成された配信のデータセット全体ではなく、その期間内に発生したイベントです。例えば、配信が 1月1日から 5日まで行われ、レポート期間が 1月1日から 2日までの場合、部分的なデータが表示されることがあります。 開封やクリックは、配信から 1 か月後でも発生する可能性があるため、選択した期間が開封／クリックの数に影響を与える可能性があります。

![](assets/campaign_reports_5.png)
