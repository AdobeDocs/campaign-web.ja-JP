---
audience: end-user
title: 強制隔離について
description: 強制隔離アドレスの管理について
source-git-commit: 9abf58c35fcf396e3003f9ecba728cd77df844a1
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 20%

---

# 強制隔離

Adobe Campaignは、強制隔離アドレス（メール、SMS、プッシュ通知）を管理します。

強制隔離は、 **メールアドレス**, a **電話番号**、または **デバイストークン**&#x200B;ただし、プロファイル自体には適用されません。 例えば、メールアドレスが強制隔離されているプロファイルは、プロファイルを更新して新しいアドレスを入力できるので、再び配信アクションのターゲットになる可能性があります。同様に、2 つのプロファイルの電話番号が同じ場合、その番号が強制隔離されると、両方のプロファイルが影響を受けます。


>[!CAUTION]
>
>Adobe Campaignでの強制隔離では大文字と小文字が区別されます。

## 強制隔離とは

強制隔離は～する方法である **配信の無効なアドレスの管理**.

配信の無効なアドレスの割合が高い場合は、スパムと見なされることがあります。 強制隔離を使用してこれらのアドレスを管理すると、インターネットプロバイダーからブロックリストに加えるされるのを避けることができます。 これは、レピュテーションにとって重要です。

Adobe Campaignでアドレスが強制隔離されると、配信の分析中に、プロファイルはターゲットから自動的に除外されます。

強制隔離は、誤りのある電話番号を配信から除外することで、SMS の送信コスト削減に役立ちます。

## アドレスが強制隔離に送信される理由

多くの理由により、アドレスが強制隔離に送信される場合があります。

- SMS の場合、誤った電話番号
- SMS の場合、プロファイルが「STOP」などのキーワードを使用して SMS メッセージに返信したとき
- メールの場合、メッセージがスパムとして報告されたとき。 メッセージは、Adobeが管理するテクニカルメールボックスに自動的にリダイレクトされます。 さらに、そのメールアドレスは自動的に強制隔離され、ステータスが「ブロックリストに加える」となります。
- 例えば、メールボックスの容量が超過した場合、アドレスが存在しない場合、またはメールサーバーが使用できない場合などに、メールアドレスを強制隔離できます。

[配信エラーの詳細](https://experienceleague.adobe.com/en/docs/campaign-classic/using/sending-messages/monitoring-deliveries/understanding-delivery-failures)

## 強制隔離アドレスの場所

インスタンスのすべての強制隔離アドレスは、次の場所で表示できます **[!UICONTROL エクスプローラー]** > **[!UICONTROL 管理]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL 配信不能件数の管理]** > **[!UICONTROL 配信不能およびアドレス]**. このセクションには、メール、SMS およびプッシュ通知チャネルの強制隔離された要素のリストが表示されます。

![](assets/quarantine_location.png){zoomable="yes"}

また、インスタンスで強制隔離に関するレポートを取得することもできます。

![](assets/quarantine_reports.png){zoomable="yes"}

配信ごとに、配信の概要レポートを確認することもできます。このレポートには、配信ターゲット内の強制隔離中のアドレス数が表示されます。

![](assets/quarantine_delivery.png){zoomable="yes"}

Adobe Campaign コンソールで強制隔離アドレスを管理する可能性が高くなります。 [詳細情報](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/quarantines#access-quarantined-addresses)
