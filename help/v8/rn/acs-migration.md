---
audience: end-user
title: Campaign Standard から Adobe Campaign web への移行
description: Campaign web ユーザーインターフェイスの確認
exl-id: 4cf406af-4cf5-434d-b1c7-a7c102f8dc2f
source-git-commit: a1c16a9ba5e5ca844eaf82ed3b587f4f7a0b0873
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 100%

---

# Campaign v8 への Campaign Standard の移行 {#acs-to-ac}

Adobe Campaign Standard ユーザーは、Adobe Campaign Managed Cloud Services v8 に移行できるようになりました。この移行には、次のような多くのメリットがあります。

* 堅牢な IT インフラストラクチャ：Managed Cloud Services v8 を使用すると、クライアントはより堅牢な IT インフラストラクチャを活用して、キャンペーンのパフォーマンス、信頼性、スケーラビリティを強化できます。
* サポートの強化：Managed Cloud Services チームは、お客様のプラットフォームのスムーズな移行と継続的なモニタリングを確保し、優れたサポートを提供することに全力を注いでいます。トラブルシューティングからプロアクティブなメンテナンスまで、お客様をサポートします。
* Adobe Experience Platform との統合：Managed Cloud Services v8 では、Adobe Experience Platform とシームレスに接続し、クライアントがデータの可能性を最大限に活用し、パーソナライズされた効果的なキャンペーンをチャネル全体で提供できるようにします。
* 一貫性の高いユーザーインターフェイスとエクスペリエンス：Managed Cloud Services v8 に移行しても、ワークフローが中断されることはありません。使い慣れたユーザーインターフェイスとユーザーエクスペリエンスを引き続き利用して、チームの学習曲線を最小限に抑えることができます。

**Campaign Standard ユーザーが Campaign v8 に移行する場合の開始方法について詳しくは、[このドキュメント](../../adoption/home.md)を参照してください。**

<!--
As a Campaign Standard user, we now offer you a way to migrate to Adobe Campaign v8. You will benefit from both the new Campaign Web interface and the v8 console.


## Key capabilities {#key-features}

As a Campaign v8 user, you have access to both the new Campaign Web interface and the v8 console. Data and settings are synchronized from an environment to another. All your data and settings available in the client console is visible in the Campaign Web user interface, from the Explorer left navigation. [Learn more](../get-started/user-interface.md#user-interface-explorer)

Campaign web user interface is designed for marketers to easily build and orchestrate their campaigns. Let's dig deeper in what key capabilities Campaign v8 web user interface will offer you:

* Modern, friendly, and unified experience. [Learn more](../get-started/connect-to-campaign.md).
* New powerful capabilities and seamless processes. [Learn more](../get-started/user-interface.md)
* New simplified and intuitive query modeler. [Learn more](../query/query-modeler-overview.md)
* Built-in cross-channel campaign management capabilities. [Learn more](../msg/gs-messages.md)
* New and redesigned campaign workflow activities. [Learn more](../workflows/gs-workflows.md)
* Easy profile creation and management. [Learn more](../audience/about-recipients.md)
* Predefined Filters. [Learn more](../get-started/predefined-filters.md)
* HTML Converter for email design. [Learn more](../email/existing-content.md)
* SMS with offers. [Learn more](../msg/offers.md)

Campaign client console is designed for administrators and developers to confgure and customize their environment. Key capabilities available in Campaign client console are detailed in [this documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/whats-new){target="_blank"}.

>[!NOTE]
>
>Learn more about supported and unsupported capabilities, and interoperability between Campaign Web user interface and Campaign client console [in this page](../get-started/capability-matrix.md)
>

## Terminology {#terminology}

Most concepts are similar between Campaign v8 and Campaign Standard. However, there are a few differences. Here are some examples of terminology differences between Campaign Standard and the Campaign v8:
-->
<!--
* Profiles are **Recipients** in the console. [Learn more](../audience/gs-audiences-recipients.md).
* Test profiles are **Seed addresses**. [Learn more](../preview-test/test-deliveries.md).
* The delivery preparation is the **Delivery analysis**. [Learn more](../monitor/prepare-send.md).
* Audiences are **Lists**. [Learn more](../audience/gs-audiences-recipients.md).
-->

<!--
* Custom resources are **Schemas**
* Messages are referred as **Deliveries**
* Roles are configured with **Named Rights**
* Security Groups are **Operator Groups**
* Organizational units are managed through **Folder Permissions**
* Product users are **Operators** in the client console
* Delivery preparation is the **Delivery analysis** in the client console

## Specific features {#new-features}

For you to transition smoothly to Campaign v8, key Campaign Standard capabilities have been added to Campaign v8. They are detailed in [this documentation](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html){target="_blank"}, and are only available to users transitioning from Campaign Standard.

* **Dynamic Reporting**: Dynamic Reporting provides fully customizable and real-time reports to measure the impact of your marketing activities. It adds access to profile data, enabling demographic analysis by profile dimensions such as gender, city and age in addition to functional email campaign data like opens and clicks. [Learn more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html){target="_blank"}.

* **Centralized branding**: Every company has brand visual and technical guidelines. With Adobe Campaign, you can define a set of specification to present a consistent brand to your customers, from logos to technical aspects, such as email sender, URL or domains. [Learn more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html)

* **Rest APIs** - As a Campaign Stardard migrated user, you can use Rest APIs to create integrations for Adobe Campaign and build your own ecosystem by interfacing Adobe Campaign with the panel of technologies that you use. [Learn more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html){target="_blank"}.

* **Landing pages** - Some improvements have been brought to Campaign v8 landing pages to ensure feature parity with Campaign Standard. Learn more in the [release notes](../rn/release-notes.md#new-24-4) and the landing page [documentation](../landing-pages/get-started-lp.md).

* **Visual fragments** - Visual fragments are reusable visual components that can be referenced in one or more email deliveries or in content templates. When modifying a fragment, every content using it is updated. This functionality allows to prebuild multiple custom content blocks that can be used by marketing users to quickly assemble message contents in an improved design process. [Learn more](../content/use-visual-fragments.md)

 <!--
* Delivery Alerting: In addition to viewing notifications directly in Campaign, Adobe Campaign also provides an email alerting system to trigger email alerts to users or external stakeholders of important system activities. Create, manage, and receive customizable alerts and dashboards to keep track of delivery successes or failures. Adobe Campaign Delivery Alerting boosts efficiency by keeping all involved Adobe Campaign users in a company automatically informed about the delivery execution status, via email and dashboard. 

* Landing Pages: Landing pages are web forms that can be used to capture information on your audiences, offer subscriptions to a service, display data and grow your database. Landing pages can also be used for acquiring or updating existing profiles, and to set up a double opt-in mechanism, allowing you to to protect the platform from wrong or invalid email addresses, or spambots. [Learn more](../landing-pages/get-started-lp.md)
-->
