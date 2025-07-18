---
title: コンポーネントのリスト
description: 動的レポートで使用可能なすべてのコンポーネントとその定義のリストを以下に示します。
level: Beginner
audience: end-user
exl-id: 5c58db92-7878-4c70-b076-a393f1cda8b7
source-git-commit: fb5bcde9c087f73bfe5724463fe280c1e494ef1f
workflow-type: ht
source-wordcount: '761'
ht-degree: 100%

---

# コンポーネントのリスト {#list-of-components}

2 つのコンポーネントに互換性がない場合、セルには「**なし**」という値が表示されます。

## ディメンション {#dimensions}

以下の表は、レポートで使用されるディメンションとその定義を示したものです。

<table> 
 <thead> 
  <tr> 
   <th> ディメンション<br/> </th> 
   <th> 定義<br/> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> ブラウザー<br/> </td> 
   <td> メッセージを開封またはクリックしたブラウザー。<br/> </td> 
  </tr> 
  <tr> 
   <td> キャンペーン<br/> </td> 
   <td> キャンペーンのラベルと ID。<br/> </td> 
  </tr> 
  <tr> 
   <td> 配信<br/> </td> 
   <td> 配信のラベルと ID。<br/> </td> 
  </tr> 
  <tr> 
   <td> デバイス<br/> </td> 
   <td> メール／SMS／プッシュ通知を、開封／表示／クリックしたデバイス。<br/> </td> 
  </tr> 
  <tr> 
   <td> エラーの理由<br/> </td> 
   <td> 各配信でバウンスを発生させたエラーのタイプ（不明なユーザー、無効なドメイン、メールボックス容量超過など）。<br/> </td> 
  </tr> 
  <tr> 
   <td> モバイルアプリ名<br/> </td> 
   <td> モバイルアプリケーションの名前。<br/> </td> 
  </tr>
  <tr> 
   <td> プラットフォーム<br/> </td> 
   <td> メッセージを開封／表示／クリックしたデバイスのプラットフォーム。<br/> </td> 
  </tr> 
  <tr> 
   <td> プロファイル<br/> </td> 
   <td> プロファイルリソースの拡張時に作成された標準およびカスタムのプロファイルフィールドを再グループ化します。<br/> </td> 
  </tr> 
  <tr> 
   <td> 受信者ドメイン<br/> </td> 
   <td> メールを開くために使用されるドメイン。<br/> </td> 
  </tr> 
  <tr> 
   <td> 繰り返し配信<br/> </td> 
   <td> 繰り返し配信のラベルと ID。<br/> </td> 
  </tr> 
  <tr> 
   <td> 送信者ドメイン<br/> </td> 
   <td> メールを送信するために使用されるドメイン。<br/> </td> 
  </tr> 
  <tr> 
   <td> 送信者 IP<br/> </td> 
   <td> メールを送信するために使用される IP。<br/> </td> 
  </tr> 
  <tr> 
   <td> トラッキング URL<br/> </td> 
   <td> ユーザーがメッセージからクリックした URL。<br/> </td> 
  </tr> 
  <tr> 
   <td> トラッキング URL カテゴリ<br/> </td> 
   <td> トラッキング URL に割り当てられているカテゴリ。<br/> </td> 
  </tr> 
  <tr> 
   <td> トラッキング URL ラベル<br/> </td> 
   <td> 「ミラーページ」、「お問い合わせ」、「開く」など、URL に付けられるラベル。<br/> </td> 
  </tr> 
  <tr> 
   <td> トランザクション配信<br/> </td> 
   <td> トランザクション配信のラベルと ID。<br/> </td> 
  </tr> 
  <tr> 
   <td> バリアント<br/> </td> 
   <td> A/B テストを行う際のメールのバリアント。<br/> </td> 
  </tr> 
 </tbody> 
</table>

## 指標 {#metrics}

以下の表は、レポートで使用する指標のリストと、配信タイプに応じた定義を示したものです。

### メールの指標 {#email-and-sms-metrics}

<table> 
 <thead> 
  <tr> 
   <th> 指標<br/> </th> 
   <th> 定義<br/> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> ブロックリスト登録済み<br/> </td> 
   <td> メールをスパムまたは迷惑メールとして報告した受信者の数。<br/> </td> 
  </tr> 
  <tr> 
   <td> ブロックリスト登録率<br/> </td> 
   <td> ブロックリストでマークされている配信の割合。<br/> </td> 
  </tr> 
  <tr> 
   <td> バウンス数 + エラー数<br/> </td> 
   <td> 送信されたメッセージの合計数に対して、配信および自動返信処理時のエラー累計の合計。<br/> </td> 
  </tr> 
  <tr> 
   <td> バウンス率 + エラー率<br/> </td> 
   <td> 送信されたメールに対するバウンスしたメールの割合。<br/> </td> 
  </tr> 
  <tr> 
   <td> クリック<br/> </td> 
   <td> 1 つの配信で、あるコンテンツがクリックされた回数。<br/> </td> 
  </tr> 
  <tr> 
   <td> クリックスルー率<br/> </td> 
   <td> 1 つの配信がクリックされた割合。<br/> </td> 
  </tr> 
  <tr> 
   <td> 配信済み<br/> </td> 
   <td> 送信されたメッセージの合計数に対して、正常に送信されたメッセージの数。<br/> </td> 
  </tr> 
  <tr> 
   <td> 配信率<br/> </td> 
   <td> 正常に送信されたメッセージの割合。<br/> </td> 
  </tr> 
  <tr> 
   <td> ハードバウンス<br/> </td> 
   <td> 永続的なエラー（メールアドレスの間違いなど）の合計数。<br/> </td> 
  </tr> 
  <tr> 
   <td> ハードバウンス率<br/> </td> 
   <td> 永続的なエラーが原因で失敗した配信の割合。<br/> </td> 
  </tr> 
  <tr> 
   <td> ミラーページ<br/> </td> 
   <td> ミラーページのリンクをクリックした受信者の数。<br/> </td> 
  </tr> 
  <tr> 
   <td> ミラーページ率<br/> </td> 
   <td> 合計配信メッセージに対するミラーページリンクのクリック数の割合。<br/> </td> 
  </tr> 
  <tr> 
   <td> オファークリック数<br/> </td> 
   <td> 1 つの配信で、あるオファーがクリックされた回数。<br/> </td> 
  </tr> 
  <tr> 
   <td> オファーのクリック率<br/> </td> 
   <td> オファーがクリックされた割合。<br/> </td> 
  </tr> 
  <tr> 
   <td> 開封数<br/> </td> 
   <td> 1 つの配信で、あるメッセージが開かれた回数。<br/> </td> 
  </tr> 
  <tr> 
   <td> 開封率<br/> </td> 
   <td> 開封されたメッセージの割合。<br/> </td> 
  </tr> 
  <tr> 
   <td> 処理済み / 送信済み<br/> </td> 
   <td> 配信の合計送信数。<br/> </td> 
  </tr> 
  <tr> 
   <td> 強制隔離<br/> </td> 
   <td> バウンスし、アドレスが強制隔離されたメッセージの数。<br/> </td> 
  </tr> 
  <tr> 
   <td> 強制隔離率<br/> </td> 
   <td> 送信されたメッセージに対する強制隔離の割合。<br/> </td> 
  </tr> 
  <tr> 
   <td> 却下<br/> </td> 
   <td> SMTP サーバーによってスパムとして分類されたメッセージの数。<br/> </td> 
  </tr> 
  <tr> 
   <td> 却下率<br/> </td> 
   <td> 却下としてマークされたメッセージの割合。<br/> </td> 
  </tr> 
  <tr> 
   <td> ソフトバウンス<br/> </td> 
   <td> 一時的なエラー（受信トレイが満杯など）の合計数。<br/> </td> 
  </tr> 
  <tr> 
   <td> ソフトバウンス率<br/> </td> 
   <td> 一時的な理由で失敗した配信の割合。<br/> </td> 
  </tr> 
  <tr> 
   <td> ユニーククリック数<br/> </td> 
   <td> 1 つの配信で、あるコンテンツをクリックした受信者の数。<br/> </td> 
  </tr> 
  <tr> 
   <td> ユニーク開封数<br/> </td> 
   <td> 配信を開いた受信者の数。<br/> </td> 
  </tr> 
  <tr> 
   <td> ユニーク購読解除数<br/> </td> 
   <td> 購読解除リンクをクリックした受信者の数。<br/> </td> 
  </tr> 
  <tr> 
   <td> 購読解除率<br/> </td> 
   <td> 配信されたメッセージに対するユニーク購読解除数。<br/> </td> 
  </tr> 
  <tr> 
   <td> 購読解除済み<br/> </td> 
   <td> 購読解除リンクがクリックされた回数。<br/> </td> 
  </tr> 
 </tbody> 
</table>

<!--
### Push notification metrics {#push-notification-metrics}

<table> 
 <thead> 
  <tr> 
   <th> Metric<br/> </th> 
   <th> Definition<br/> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> Bounces + Errors<br/> </td> 
   <td> Total of errors cumulated during delivery in relation to the total number of sent messages, e.g. errors from MCPNS or provider.<br/> </td> 
  </tr> 
  <tr> 
   <td> Bounce + Error rate<br/> </td> 
   <td> Percentage of push notifications that bounced compared to push notifications sent.<br/> </td> 
  </tr> 
  <tr> 
   <td> Click<br/> </td> 
   <td> Number of times a push notification has been delivered to the device and clicked on by the user. The user either wanted to view the notification, which will then be moved to Push Open tracking, or dismiss it.<br/> </td> 
  </tr> 
  <tr> 
   <td> Click through rate<br/> </td> 
   <td> Percentage of users who interacted with the push notification.<br/> </td> 
  </tr> 
  <tr> 
   <td> Delivered<br/> </td> 
   <td> Number of push notifications successfully sent, in relation to the total number of sent push notifications.<br/> </td> 
  </tr> 
  <tr> 
   <td> Delivered rate<br/> </td> 
   <td> Percentage of push notifications successfully sent.<br/> </td> 
  </tr> 
  <tr> 
   <td> Impressions<br/> </td> 
   <td> Number of times a push notification has been delivered to the device and left untouched in the notification center. In most cases, impressions number should be similar to the delivered number. This ensures that the device got the message and relayed that information back to the server.<br/> </td> 
  </tr> 
  <tr> 
   <td> Processed/sent<br/> </td> 
   <td> Total number of push notifications sent.<br/> </td> 
  </tr> 
  <tr> 
   <td> Open<br/> </td> 
   <td> Total number of push notifications delivered to the device and clicked on by users thus opening the app. This is similar to the Push Click except a Push Open will not be triggered if the notification was dismissed.<br/> </td> 
  </tr> 
  <tr> 
   <td> Open rate<br/> </td> 
   <td> Percentage of opened push notifications.<br/> </td> 
  </tr> 
  <tr> 
   <td> Unique clicks<br/> </td> 
   <td> Number of times a unique user interacts with the push notification, e.g. clicks on the notification or button.<br/> </td> 
  </tr> 
  <tr> 
   <td> Unique impressions<br/> </td> 
   <td> Number of impressions by recipient.<br/> </td> 
  </tr> 
  <tr> 
   <td> Unique Opens<br/> </td> 
   <td> Number of recipients who opened the delivery.<br/> </td> 
  </tr> 
 </tbody> 
</table>

### In-App metrics {#in-app-metrics}

<table> 
 <thead> 
  <tr> 
   <th> Metric<br/> </th> 
   <th> Definition<br/> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> Delivered<br/> </td> 
   <td> Total number of In-App messages delivered to the device by the service provider.<br/> </td> 
  </tr> 
  <tr> 
   <td> Impressions<br/> </td> 
   <td> Total of In-App messages seen by recipients depending on whether trigger criterion was met.<br/> </td> 
  </tr> 
  <tr> 
   <td> In-App clicks <br/> </td> 
   <td> Total number of recipients who clicked on Button 1 or Button 2.<br/> </td> 
  </tr> 
  <tr> 
   <td> In-App click through rate<br/> </td> 
   <td> Percentage of users who clicked on Button 1 or Button 2 compared to users who saw the message.<br/> </td> 
  </tr> 
  <tr> 
   <td> In-App dismissal<br/> </td> 
   <td> Total number of messages that recipients dismissed either by clicking the close button or auto-dismiss.<br/> </td> 
  </tr> 
  <tr> 
   <td> In-App dismissal rate<br/> </td> 
   <td> Percentage of In-App messages that recipients dismissed.<br/> </td> 
  </tr> 
  <tr> 
   <td> Processed/sent<br/> </td> 
   <td> Total number of In-App messages sent from Adobe Campaign as part of the delivery sent process.<br/> </td> 
  </tr> 
  <tr> 
   <td> Unique impressions<br/> </td> 
   <td> Number of impressions by a unique recipient.<br/> </td> 
  </tr> 
  <tr> 
   <td> Unique In-App clicks<br/> </td> 
   <td> Number of times recipients clicked on Button 1 or Button 2.<br/> </td> 
  </tr> 
  <tr> 
   <td> Unique In-App dismissals<br/> </td> 
   <td> Number of time recipients dismissed an In-App message.<br/> </td> 
  </tr> 
 </tbody> 
</table>
-->

## セグメント {#segments}

以下の表は、レポートで使用されるセグメントとその定義を示したものです。

<table> 
 <thead> 
  <tr> 
   <th> セグメント<br/> </th> 
   <th> 定義<br/> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 年齢：ブーマー 1<br/> </td> 
   <td> 1946～1954年生まれの受信者。<br/> </td> 
  </tr> 
  <tr> 
   <td> 年齢：ブーマー 2<br/> </td> 
   <td> 1955～1965年生まれの受信者。<br/> </td> 
  </tr> 
  <tr> 
   <td> 年齢：18～25 歳<br/> </td> 
   <td> 18～25 歳の受信者。<br/> </td> 
  </tr> 
  <tr> 
   <td> 年齢：26～30 歳<br/> </td> 
   <td> 26～30 歳の受信者。<br/> </td> 
  </tr> 
  <tr> 
   <td> 年齢：31～40 歳<br/> </td> 
   <td> 31～40 歳の受信者。<br/> </td> 
  </tr> 
  <tr> 
   <td> 年齢：41～50 歳<br/> </td> 
   <td> 41 歳～50 歳の受信者。<br/> </td> 
  </tr> 
  <tr> 
   <td> 年齢：X 世代<br/> </td> 
   <td> 1966～1976年生まれの受信者。<br/> </td> 
  </tr> 
  <tr> 
   <td> 年齢：Y 世代（ミレニアル世代）<br/> </td> 
   <td> 1977～1994年生まれの受信者。<br/> </td> 
  </tr> 
  <tr> 
   <td> 年齢：Z 世代<br/> </td> 
   <td> 1995年から現在までに生まれた受信者。<br/> </td> 
  </tr> 
  <tr> 
   <td> 年齢：50 歳超<br/> </td> 
   <td> 年齢が 50 歳を超える受信者。<br/> </td> 
  </tr> 
  <tr> 
   <td> 年齢：25 歳未満<br/> </td> 
   <td> 年齢が 25 歳未満の受信者。<br/> </td> 
  </tr> 
  <tr> 
   <td> 年齢：30 歳未満<br/> </td> 
   <td> 年齢が 30 歳未満の受信者。<br/> </td> 
  </tr> 
  <tr> 
   <td> 年齢：40 歳未満<br/> </td> 
   <td> 年齢が 40 歳未満の受信者。<br/> </td> 
  </tr> 
  <tr> 
   <td> 年齢：50 歳未満<br/> </td> 
   <td> 年齢が 50 歳未満の受信者。<br/> </td> 
  </tr> 
  <tr> 
   <td> 年齢：サイレントジェネレーション<br/> </td> 
   <td> 1945 年以前に生まれた受信者。<br/> </td> 
  </tr> 
  <tr> 
   <td> すべての訪問<br/> </td> 
   <td> すべての受信者<br/> </td> 
  </tr>
 </tbody> 
</table>
