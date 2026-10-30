---
title: Shopify 的订单管理集成
doc_id: GG656LGTR55BTUX5
source: https://sellercentral.amazon.com/help/hub/reference/external/GG656LGTR55BTUX5
language: zh-CN
fetched_at: 2026-10-30 13:35:04
---

# Shopify 的订单管理集成

如果您在 Shopify 店铺使用订单管理系统 (OMS)，则可能需要配置该系统，才能使用多渠道配送 (MCF)。本页面介绍了如何配置兼容的订单管理系统平台并识别不支持多渠道配送的系统。

## 使用多渠道配送配送部分订单商品
如果购物车包含无法在单个货件中配送的商品，则会拆分为多个货件进行配送。要确保您希望使用多渠道配送的商品正确导入您的订单管理系统，以便在拆分购物车货件中配送，您可能需要对订单管理系统进行细致的自定义设置。

有关 Shopify 拆分配送的更多信息，请参阅 [Shopify 结算中的拆分配送](https://help.shopify.com/en/manual/checkout-settings/split-shipping)。

**支持多个 SKU 地点： **该应用为每个 SKU 添加了新的配送地点。只要在 Shopify 中将名为 [permitsSKUsharing](https://shopify.dev/changelog/fulfillment-service-sku-sharing) 的参数设置为 【false】，您的订单管理系统就可以阻止为 SKU 添加新的配送地点。这会导致无法将亚马逊运营中心添加为额外的配送地点。要使用多渠道配送，请配置您的订单管理系统，将 【permitsSKUsharing】 设置为 【true】。

如果您使用的是 Shopify 订单管理系统，则 【permitsSKUsharing】 将自动设置为 【true】。如果您使用的是 Shopify 多渠道配送应用，依次选择【设置】和【多个地点】，即可设置此配置。

对于所有其他应用，请检查您的订单管理系统文件或咨询您的订单管理系统代表，确定 【permitsSKUsharing】 是否设置为 【truex】。

## 兼容的订单管理系统
完全兼容的订单管理西游（无需操作）：

- Shopify
- 领星
- OrderDesk
- ByteStand
- Shipbob
- WebBee
- Microsoft Dynamic 365
- Shippo
- Listing Mirror

需要调整的兼容订单管理系统：

- ShipStationPipe17
- ShipHero
- Easyship
- NetSuite ERP Connector (FarApp)
- BrightPearl

## ShipStation
当您的网站启用了 ShipStation，每件商品或每个配送订单将会显示一个发货地址。使用 ShipStation 时，系统会在发货地址下拉菜单中预选 ShipStation 的默认发货地址或使用“自动化规则”的发货地址。为避免商品的发货地址出错，请按照以下步骤在创建标签之前调整发货地址：

1. 前往【设置】 > 【销售渠道】 > 【店铺设置】
2. 单击您 Shopify 店铺的操作菜单符号（省略号，即“……”），然后点击【编辑店铺详情】。
3. 在“常规店铺设置”选项卡上，点击“编辑 Shopify 店铺设置”。
4. 在“修改商城设置”弹窗中，打开“将多个未结配送订单映射到请求的配送任务”选项。

**注意： **需要启用此设置，多渠道配送才能正常运转。

有关如何在您的账户中启用此设置的更多问题，请[联系 ShipStation 支持](https://help.shipstation.com/hc/en-us/articles/360025853032#UUID-a9b61350-3974-338f-b82b-488b28385a5d)。

## Pipe17
Pipe17 只会配送地址已映射到 Pipe17 地址的商品。Pipe17 会导入亚马逊配送的行项目，但显示“无需配送”，以免出现重复配送问题。要配置此设置，请执行以下操作：

1. 打开您的 【Pipe17 管理后台】。
2. 前往【集成】选项卡。
3. 选择您的店铺。
4. 选择【设置】。
5. 确认选择【仅拉取分配给与 Pipe17 运营中心关联的库房的订单】这一选项。
6. 返回【集成】选项卡。
7. 选择【位置】。
8. 确认您的亚马逊运营中心未映射到 3PL。“3PL 集成”列应显示为缺失。
9. 确认您的非 Prime 商品所在地址已映射到 3PL 集成。否则，订单将不会显示在 Pipe17 中。

有关其他问题，请联系 [Pipe17 支持](https://support.pipe17.com/hc/en-us)。

## ShipHero
要确认 Shopify 的订单配送状态更新是否准确，请更新以下店铺设置：

- 我的账户
- 店铺
- 店铺设置
- 确认已选择【由 ShipHero 管理我的 Shopify 库存】并确保已选中所有设置。

## EasyShip
[联系卖家支持](https://console.buywithprime.amazon.com/support/create-case?ref=us-oo-sc-pricingpage&utm_medium=website&utm_source=direct&utm_campaign=us-oo-sc-pricingpage&utm_content=home-page%2Csection_knowledge-center)寻求帮助。

## NetSuite ERP Connector (FarApp)
为避免重复配送，请更改以下配置，确保 NetSuite 能够识别您所有的运营中心地点。

首先，请确保您的 Shopify 订单是自动配送的。按照以下说明验证或修改此设置：

1. 打开 Shopify 管理后台。
2. 选择【设置】，然后选择【通用】。
3. 向下滚动至【订单处理】。

接下来，导航至 FarApp，并按照以下说明更新地点映射：

1. 前往 [app.farapp.com](http://app.farapp.com) 并登录。
2. 在侧边菜单中，选择 【Shopify】 > 【映射】 > 【订单】。
3. 选择【订单商品】，然后选择【添加映射】。
4. 在订单商品映射设置中，映射类型将显示为【带翻译的订单行】。在 Shopify 字段/固定值中，它显示为 【options.location_id】。选择【查看/编辑】。
5. 在 Shopify 值中，添加您的[**亚马逊运营中心编号**](https://buywithprime.amazon.com/knowledge-center/buy-with-prime-app-for-shopify/erp-integration?ref=MS&utm_source=ref-domain&utm_medium=website#articleSection-1)**。**
6. 在 NetSuite 值中，添加您用于处理多渠道配送商品的 NetSuite 地点。
7. 依次点击【保存】和【关闭】。

**注意： **如果您刚开始使用多渠道配送，请先在 NetSuite 中为 MCF 商品创建一个地点，然后使用该地点。

## BrightPearl
Brightpearl 是一款订单管理系统 (OMS) 应用，可帮助您在多个销售渠道完成从下单到配送的整个订单生命周期。您可以使用 Brightpearl 和多渠道配送按分销渠道来分配订单。

如果您尚未安装和设置 Brightpearl，请按照以下说明操作：

1. 1. 在您的 Shopify 管理后台，前往【通用设置】，然后选择【不自动配送订单中的任何单项商品】。
2. 2. 在 Shopify app store 中，安装 Brightpearl 应用。
3. 确保【已安装应用】中列出了 【Brightpearl】 应用。

Brightpearl 设置配置

库存设置

1. 前往 Shopify 管理后台中的 Brightpearl Shopify 应用，然后选择【启用库存更新】
2. 在【多库存地点映射】中，选择应填充到 Shopify 各库存地点的 Brightpearl 库房。将【亚马逊物流库存地点】与您为多渠道配送指定的 Brightpearl 库房匹配。

**注意： **如果您没有要分配给多渠道配送的 Brightpearl 库房，请前往[库房](https://help.brightpearl.com/s/article/211279426)创建一个。

订单配置： 在 Shopify 管理后台的 Brightpearl Shopify 应用中，请前往【设置】，然后选择【订单】选项卡。

点击以下参数：

- 启用订单下载
- 启用订单编辑

添加【匿名订单的联系电子邮件】。

配送设置： 前往【配送】选项卡，然后点击【启用配送】。

付款设置： 前往【付款】选项卡，为“Shopify 交易”选择 【Brightpearl 付款方式】。

Brightpearl 平台设置

1. 在 Brightpearl 控制台的【设置】侧边菜单中，前往【渠道】。如果 【Shopify】 尚未设置为渠道，则添加它。
2. 在【设置】侧边菜单中，前往【自动化】，然后选择【规则】选项卡。
3. 点击创建新规则并添加【配送多渠道配送订单】。
4. 选择【配送多渠道配送订单】规则的【条件】。您可以点击【添加条件】，然后选择多个【渠道】和【订单库房】。

**注意： **为防止重复配送，请创建以下条件：排除您指定的亚马逊物流库房。例如： “订单库房不适用于亚马逊物流”。

## 不兼容的订单管理系统
- 店小秘
- Veeqo

如果您看到列出的订单管理系统中没有您的系统，请联系[销售伙伴支持](https://sellercentral.amazon.com/cu/contact-us)，确认特定订单管理系统的兼容性状态。

**注意： **亚马逊的卖家助手可以通过此主题提供帮助。对于大多数语言设置，卖家助手还可以直接将您转接至销售伙伴支持。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GG656LGTR55BTUX5
