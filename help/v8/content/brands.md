---
audience: end-user
title: ブランドの管理
description: ブランドガイドラインの作成および管理方法について説明します
hide: true
hidefromtoc: true
badge: label="Beta" type="Informative"
source-git-commit: e6e23a758cce657b582174e522d61193dc7326cf
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 2%

---

# ブランドの作成と管理 {#brands}

>[!AVAILABILITY]
>
>この機能は、プライベートベータ版としてリリースされます。 今後のリリースで、すべてのお客様が段階的に利用できるようになります。

ブランドガイドラインは、ブランドの視覚的および言語的なアイデンティティを定義する包括的な一連のルールおよび標準です。 すべてのマーケティングおよびコミュニケーションチャネルにわたって一貫したブランド表現を確保するための参照として機能します。

[!DNL Adobe Campaign Web] では、ブランド情報を手動で入力および整理したり、自動データ抽出用のブランドガイドラインドキュメントをアップロードしたりできるようになりました。

## ブランドへのアクセス {#generative-access}

[!DNL Adobe Campaign Web] で **[!UICONTROL ブランド]** メニューにアクセスするには、ユーザーに **[!UICONTROL 管理者（管理者）]** および **[!UICONTROL ブランドキット]** 製品プロファイルを割り当てて、ブランドを作成および管理する必要があります。 読み取り専用アクセスの場合、ユーザーは [!UICONTROL AI アシスタント ] 製品プロファイルが必要です。

[詳細情報](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

+++  ブランド関連の権限の割り当て方法を学ぶ

1. [Admin Console](https://adminconsole.adobe.com/enterprise) のホームページで、Campaign 製品にアクセスします。

   ![](assets/brands_admin_1.png)

1. ユーザーに付与する権限のレベルに応じて **[!DNL Product profile]** を選択します。

   ![](assets/brands_admin_2.png)

1. 「**[!DNL Add users]**」をクリックして、選択した製品プロファイルを割り当てます。

   ![](assets/brands_admin_3.png)

1. ユーザーの名前、ユーザーグループまたはメールアドレスを入力します。

1. 「**保存**」をクリックして、変更を適用します。

この役割に既に割り当てられているユーザーの権限は自動的に更新されます。

+++

## ブランドを作成 {#create-brand-kit}

ブランドガイドラインを作成および管理するには、次の手順に従います。

ブランドガイドラインを作成および管理するには、詳細を自分で入力するか、ブランドガイドラインドキュメントをアップロードして、情報を自動的に抽出します。


1. **[!UICONTROL コンテンツ管理]** メニューから「**[!UICONTROL ブランド]**」を選択します。

1. **[!UICONTROL ブランド]** メニューで、「**[!UICONTROL ブランドを作成]**」をクリックします。

   ![](assets/brands_1.png)

1. ブランドの **[!UICONTROL 名前]** を入力します。

1. ファイルをドラッグ&amp;ドロップまたは選択してブランドガイドラインをアップロードし、自動的に関連するブランド情報を抽出します。 **[!UICONTROL ブランドを作成]** をクリックします。

   情報の抽出プロセスが開始されます。 完了するまでに数分かかる場合があります。

   ![](assets/brands_7.png)

1. コンテンツとビジュアル作成標準が自動的に入力されるようになりました。 様々なタブを参照して、必要に応じて情報を調整します。

1. 「**[!UICONTROL ライティングスタイル]**」タブで「![](assets/do-not-localize/Smock_Add_18_N.svg)」をクリックし、例を含むガイドラインや除外を追加します。

   ![](assets/brands_2.png)

1. **[!UICONTROL ビジュアルコンテンツ]** タブで、![](assets/do-not-localize/Smock_Add_18_N.svg) をクリックして、別のガイドラインまたは除外を追加します。

1. 正しい使用方法を示す画像を追加するには、「例 **[!UICONTROL を選択し]** 「**[!UICONTROL 画像を選択]**」をクリックします。 また、除外の例として、誤った使用法を示す画像を追加することもできます。

   ![](assets/brands_3.png)

1. 設定が完了したら、**[!UICONTROL 保存]** をクリックしてから **[!UICONTROL 公開]** をクリックして、ブランドガイドラインを AI アシスタントで使用できるようにします。

1. 公開済みのブランドに変更を加えるには、「**[!UICONTROL ブランドを編集]**」をクリックします。

   >[!NOTE]
   >
   >これにより、編集モードで一時コピーが作成され、公開後にライブバージョンが置き換えられます。

   ![](assets/brands_4.png)

1. **[!UICONTROL ブランド]** ダッシュボードで、![](assets/do-not-localize/Smock_More_18_N.svg) のアイコンをクリックして詳細メニューを開きます。

   * ブランドを表示
   * 編集
   * 複製
   * 公開
   * 非公開
   * 削除

   ![](assets/brands_5.png)

ブランドガイドラインに AI アシスタントメニューの **[!UICONTROL ブランド]** ドロップダウンからアクセスできるようになり、仕様に合ったコンテンツとアセットを生成できるようになりました。 [ 詳しくは、AI アシスタントを参照してください ](gs-generative.md)

![](assets/brands_6.png)
