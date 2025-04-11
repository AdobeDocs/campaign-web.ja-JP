---
audience: end-user
title: 強制隔離について
description: 強制隔離アドレスの管理について
exl-id: 4fddabbe-39ab-418b-a87c-f86fe96fa28b
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 33%

---

# 強制隔離の管理 {#quarantines}

Adobe Campaignは、メール、プッシュおよび SMS チャネルの強制隔離アドレスを管理します。

強制隔離は、**メールアドレス**、**電話番号**、または&#x200B;**デバイストークン**&#x200B;にのみ適用され、プロファイル自体には適用されません。例えば、メールアドレスが強制隔離されているプロファイルを新しいアドレスで更新できます。 その場合、プロファイルは配信アクションのターゲットに再度設定できます。 同様に、2 つのプロファイルの電話番号が同じ場合、その番号が強制隔離されると、両方のプロファイルが影響を受けます。

>[!CAUTION]
>
>Adobe Campaign の強制隔離では、大文字と小文字が区別されます。

## 強制隔離とは {#quarantines-what}

強制隔離は、**配信内の無効なアドレスを管理** するための方法です。

配信の無効なアドレスの割合が高い場合は、スパムと見なされる可能性があります。 強制隔離を使用してこれらのアドレスを管理すると、インターネットプロバイダーによるブロックリストに加えるを防ぐことができます。 これは、レピュテーションを維持するために重要です。

Adobe Campaignでアドレスが強制隔離されると、配信の分析中に、プロファイルがターゲットから自動的に除外されます。

強制隔離では、誤りのある電話番号を配信から除外することで、SMS の送信コストを削減します。

強制隔離について詳しくは、[Campaign v8（コンソール）ドキュメント](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/send/failures/quarantines){target="_blank"}を参照してください。

## アドレスが強制隔離に送信される理由 {#quarantines-why}

アドレスを強制隔離に送信する理由は様々です。

* SMS の場合、誤った電話番号
* SMS の場合、プロファイルが「STOP」などのキーワードを使用して SMS メッセージに返信する場合
* メールの場合、メッセージがスパムとして報告されたときメッセージは、Adobeが管理するテクニカルメールボックスに自動的にリダイレクトされます。 さらに、そのメールアドレスは自動的に強制隔離され、ステータスが「ブロックリスト登録済み」となります。
* 例えば、メールボックスの容量が超過した場合、アドレスが存在しない場合、またはメールサーバーが使用できない場合などに、メールアドレスを強制隔離できます。

配信の失敗について詳しくは、[Campaign v8（コンソール）ドキュメント](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/send/failures/delivery-failures){target="_blank"}を参照してください。

## 強制隔離アドレスの場所 {#quarantines-where}

インスタンス内のすべての強制隔離アドレスは、**[!UICONTROL エクスプローラー]**/**[!UICONTROL 管理]**/**[!UICONTROL キャンペーン管理]**/**[!UICONTROL 配信不能件数の管理]**/**[!UICONTROL 配信不能件数およびアドレス]** で表示できます。 このセクションには、メール、SMS およびプッシュ通知チャネルの強制隔離された要素のリストが表示されます。

![Adobe Campaign インターフェイスの強制隔離の場所 ](assets/quarantine_location.png){zoomable="yes"}

また、インスタンスの強制隔離に関するレポートにアクセスすることもできます。

![Adobe Campaign インターフェイスでの強制隔離レポート ](assets/quarantine_reports.png){zoomable="yes"}

配信ごとに、配信概要レポートを確認できます。 配信ターゲット内の強制隔離中のアドレス数が表示されます。

![ 強制隔離されたアドレスを示す配信概要レポート ](assets/quarantine_delivery.png){zoomable="yes"}

Adobe Campaign コンソールで、強制隔離アドレスを管理するためのその他のオプションを確認できます。 [詳細情報](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/send/failures/quarantines#access-quarantined-addresses)。