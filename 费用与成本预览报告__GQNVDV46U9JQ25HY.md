---
title: 费用与成本预览报告
doc_id: GQNVDV46U9JQ25HY
source: https://sellercentral.amazon.com/help/hub/reference/external/GQNVDV46U9JQ25HY
language: zh-CN
fetched_at: 2026-10-30 13:49:11
---

# 费用与成本预览报告

## 费用与成本预览报告
费用与成本预览报告根据历史数据和亚马逊需求预测提供预计费用，以帮助您预估未来的费用，并在未来 120 天内在 MSKU 级别优化商品的单位成本。报告输出包含销售额、支持的费用、支持的广告、每件商品的成本和净收入的预计数据。此报告中用于生成估算值的数据最早可能是 24 小时以前的数据。

按照[费用与成本预览报告](https://sellercentral.amazon.com/cepreport)中的步骤，选择您想要在报告中包含的亚马逊商城、数据汇总级别、日期范围和数据类型。

此报告的可下载文件以 CSV 格式提供。如果 Excel 未自动检测到此格式，并在打开文件时询问您文件是什么格式，请选择“逗号分隔值”或“CSV”。

**重要： **要在报告中包含低库存水平费用，请务必在第 2 步的报告配置选项中选择配送基本费率和附加费。要在报告中包含仓储费，请确保您指定的时间段包含收取仓储费的当月 7 日到 15 日之间的日期范围。

**注意： **目前提供亚马逊物流商品的预计销售数据。对于卖家自配送商品，我们使用 30 天历史平均值来预估未来的销售。要在此报告中预览已宣布的费用变更，请选择包含即将到来的变更日期的日期范围。

## 预估销售数据的定义：
字段名 定义
Sales 下单商品的预估销售额，计算方法：所选时间段内商品的平均售价 × 预估售出的商品数量。
Units sold 所选时间段内亚马逊的需求预测所预估的下单商品数量。
Average sales price 用于计算所选时间段内的销售额的当前价格。
Units returned 所选时间段内的预计退款商品数量，使用每件商品过去 30 天的退货数量计算得出。
Net sales 预计净商品销售额，计算方法是预计商品销售额减去退款商品销售额。
Net units sold 所选时间段内的预计售出商品数量，计算方法是预计下单商品数量减去预计退款商品数量。

## 费用数据的定义：
对于支持的每种费用类型，本报告中包含以下数据（如果适用于该费用类型）。

字段名 定义
Fee quantity 卖家账户中某件商品的预计费用数量。如果费用不是按件收取，则该值可能为空，也可能不是整数。
Fee total 在考虑了促销和税费后，针对此费用类型的预计总收费金额。计算方法：金额 - 促销金额 + 税费金额。
Fee per unit 在考虑了促销和税费后，每件商品的预计收费金额。计算方法：总金额 ÷ 收费的商品数量。当数量为空时，该值将为空。
Fee amount* 根据价目表计算的费用金额（不包括促销或税费）。
Promotion amount* 与此交易类型相关的促销金额。计算总金额时，会从金额中减去该值。
Tax amount* 与此交易类型相关的税费金额。计算总金额时，会向金额中加上该值。
**注意： **标有 * 的字段在下载报告中尚未提供，但可通过与报告相关的销售伙伴 API 获取。

## 支持的费用类型：
字段名 定义
FBA fulfillment fees 亚马逊物流配送费用按件收取。此费用取决于商品分类、尺寸分段和发货重量。
Monthly inventory storage fees 月度仓储费取决于您的库存在亚马逊运营中心的平均每日占用体积。费用取决于商品分类、尺寸分段和当年仓储时间。此费用按月收取。
Low Inventory Level Fee 低库存水平费用按配送的每件商品收取。此费用取决于历史供货天数。历史供货天数是指日均可售库存商品数量与日均配送商品数量的比值。有关此费用的价目表和相关信息，请参阅[低库存水平费用](https://sellercentral.amazon.com/help/hub/reference/GV43F6S76Y9DHYRH)。
Referral fee 销售佣金按售出的每件商品收取。具体金额取决于商品所属的商品分类。此费用根据总销售价格（即买家支付的总金额，包括商品价格以及所有运费或礼品包装费）计算得出。有关更多信息，请参阅[销售佣金](https://sellercentral.amazon.com/help/hub/reference/external/GTG4BAWSY39Z98Z3)。
Monthly inventory storage fees 亚马逊会针对您的库存在运营中心占用的空间来收取月度仓储费。月度仓储费基于按[亚马逊物流政策和要求](https://sellercentral.amazon.com/gp/help/external/G201030350)正确包装且准备发货的商品的尺寸，根据平均每日占用体积（以立方英尺为单位）计算得出。有关更多信息，请参阅[月度仓储费](https://sellercentral.amazon.com/help/hub/reference/G3EDYEF6KUCFQTNM)。
Aged Inventory surcharge 我们会对在亚马逊物流配送网络中存放 181 天及以上的库存商品收取超龄库存附加费（以前称为长期仓储费）。有关更多信息，请参阅[超龄库存附加费](https://sellercentral.amazon.com/help/hub/reference/external/GJQNPA23YWVA4SBD)。
Per-item selling fees 订阅个人销售计划的卖家需要为在亚马逊商城售出的每件商品支付一笔费用以及所有其他适用费用。有关更多信息，请参阅[按件收取的销售费用](https://sellercentral.amazon.com/help/hub/reference/G8TPCFJRDFPKAZ6M)。
Closing fees 亚马逊会对以下分类中的每件售出商品收取交易手续费： 图书、DVD、音乐、软件和电脑/视频游戏、视频游戏机和视频游戏配件。有关更多信息，请参阅[交易手续费](https://sellercentral.amazon.com/help/hub/reference/GKD9U5REK5DKB38Y)。
Returns Processing Fee for Apparel and Shoes 针对“服装”和“鞋靴”类商品中每件买家退货商品的费用。有关更多信息，请参阅[退货处理费](https://sellercentral.amazon.com/help/hub/reference/external/GU3WQAZP7PCNF4AC)。
Returns Processing Fee for non-Apparel and non-Shoes 应用于退货率高于各个商品费用分类特定阈值的符合要求的商品的费用。按件收取的费用取决于商品尺寸分段和发货重量。有关更多信息，请参阅[退货处理费](https://sellercentral.amazon.com/help/hub/reference/external/GU3WQAZP7PCNF4AC)。
FBA inbound placement service fee 亚马逊物流入库配置服务费率的计算依据是商品尺寸分段、发货重量和入库地点。该费用还取决于入库计划中的地点数量分段或货件数量分段。有关更多信息，请参阅[亚马逊物流入库配置服务费](https://sellercentral.amazon.com/help/hub/reference/GC3Q44PBK8BXQW3Z)。
**注意： **目前并非所有费用都包含在费用与成本预览报告中。但是，我们正在努力在未来的版本中加入附加费用预览。

## 广告：
本报告中针对广告费用包含以下数据类型。

字段名 定义
Total amount 在考虑了促销和税费后，针对此费用类型的最终收费金额。计算方法：金额 - 促销金额 + 税费金额。
Amount per unit 在考虑了促销和税费后，每件商品的最终收费金额。计算方法：总金额 ÷ 收费的商品数量。当数量为空时，该值将为空。
Quantity 针对此广告类型收费的商品数量。
Promotion amount 与此交易类型相关的促销金额。计算总金额时，会从金额中减去该值。
Tax amount 与此交易类型相关的税费金额。计算总金额时，会向金额中加上该值。
费用与成本预览报告中目前支持以下广告类型：

Sponsored Products charges 商品推广是一种按点击付费的广告解决方案，通过使用可在亚马逊网站各个醒目位置展示的广告，对您的商品进行推广。

## Off Amazon costs：
卖家按每件商品为此商品提供的亚马逊以外的费用。

本报告中按照每件商品的成本可包含以下数据类型：

字段名 定义
Cost of goods sold 制造或采购商品的成本。该值由卖家提供，同时适用于亚马逊物流商品和卖家自配送商品。
Miscellaneous cost 与此特定商品无关的杂费，如间接费用等。该值由卖家提供，同时适用于亚马逊物流商品和卖家自配送商品。
Fulfillment cost 包含该商品的订单的配送费用，包括人工费、包装材料费、配送至买家的运费以及客户服务费等。该值由卖家提供，适用于卖家自配送商品。
Storage cost 每月存储一件此商品的成本。该值由卖家提供，适用于卖家自配送商品。
**注意： **费用与成本预览报告可以整合您的成本，如所售商品成本、杂费成本、运输成本和卖家自配送成本，以更准确地计算每件商品的净收入。自愿提供此信息，您也可以不提供这些信息而直接使用费用与成本预览报告。您可以通过[其他财务输入](https://sellercentral.amazon.com/seller-inputs)批量提供非亚马逊费用，也可以通过 [SKU 成本](https://sellercentral.amazon.com/help/hub/reference/GNG95QWKFKSAMYJV)和[亚马逊物流收入计算器](https://sellercentral.amazon.com/revcal)一次提供一件商品。要在报告中包含这些成本，需要启用针对“卖家提供的成本”的用户权限。请参阅常见问题了解更多详情。

## Net proceeds：
在某个时间段内，卖家账户中某一商品的净收入。该字段的计算方法：净销售额 - 收取的总费用之和 - 收取的总广告费用之和 -（每件商品的成本 * 售出的净商品数量）。

费用与成本预览报告中的净收入数据类型：

Net proceeds total 在某个时间段内，卖家账户中某一商品的总净收入。
Net proceeds per unit 在某个时间段内，卖家账户中某一商品的每件商品净收入。计算方法：总销售额 ÷ 已售的净商品数量。
**注意： **某些司法辖区可能会要求亚马逊对上述费用收取税费。我们将使用您在卖家账户中提供的信息来确定某项费用是否应纳税，以及应收取的相应增值税、商品及服务税、销售税或其他税费。税务规则和法规因司法辖区而异。更多信息，请在卖家平台帮助中心搜索增值税、商品及服务税、销售税或国家/地区名称。在亚马逊收费表上会显示含税费用与计算好的税费。要了解哪些费用含税，请参阅您所在区域的[亚马逊服务商业解决方案协议](https://sellercentral.amazon.com/gp/help/external/G1791)。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GQNVDV46U9JQ25HY
