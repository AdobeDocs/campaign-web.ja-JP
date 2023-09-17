---
audience: end-user
title: 「ディメンションを変更」ワークフローアクティビティの使用
description: 「ディメンションを変更」ワークフローアクティビティの使用方法を説明します
badge: label="Beta"
source-git-commit: 253889459de03cf4df72be5a5fbc223588e9b86c
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 25%

---


# ディメンションを変更 {#change-dimension}

<!--
>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Generate Complement"
>abstract="TBD"
-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_dimension"
>title="ディメンションを変更アクティビティ"
>abstract="このアクティビティを使用すると、オーディエンスの作成時にターゲティングディメンションを変更できます。 データテンプレートと入力ディメンションに応じて軸が移動します。 例えば、「契約」ディメンションから「クライアント」ディメンションに切り替えることができます。"


The **ディメンションを変更** アクティビティは **ターゲット設定** アクティビティ。 このアクティビティを使用すると、オーディエンスの作成時にターゲティングディメンションを変更できます。 このアクティビティでは、データテンプレートと入力ディメンションに応じて軸を移動します。例えば、「契約」ディメンションから「クライアント」ディメンションに切り替えることができます。

さらに、このアクティビティを使用して、新しいターゲットの列を追加して定義したり、データの重複排除条件を定義したりできます。

## 設定

次の手順に従って、 **ディメンションを変更** アクティビティ：

1. を追加します。 **ディメンションを変更** アクティビティをワークフローに追加します。

   ![](../assets/workflow-change-dimension.png)

1. 次を定義： **新しいターゲットディメンション**.

ディメンションの変更時に、すべてのレコードが保持されます。