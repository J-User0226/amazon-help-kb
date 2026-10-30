---
title: 卖家平台中财务报告的细微更改
doc_id: GSTBL8HHTMPF3DCT
source: https://sellercentral.amazon.com/help/hub/reference/external/GSTBL8HHTMPF3DCT
language: zh-CN
fetched_at: 2026-10-30 13:51:15
---

# 卖家平台中财务报告的细微更改

为了提供更加一致的财务报告体验，我们对交易一览、结算报告 V1、结算报告 V2 和日期范围报告进行了细微的显示更新。这些变更使财务数据在各个界面之间上的呈现方式保持一致。您无需执行任何操作。

## 交易一览变更
我们已从**商品详情**字段中移除了亚马逊物流买家退货费用、亚马逊物流运输费用等交易的商品分类信息（例如：服装和鞋靴）。您仍可在[库存报告](https://sellercentral.amazon.com/listing/reports/)下的**分类商品**报告中查看此信息。

## 结算报告 V1、结算报告 V2 和日期范围报告变更
**amount-description 字段中的额外详细信息**

我们已在结算报告 V1、结算报告 V2 和日期范围报告的 amount-description 字段中加入了额外的详细信息。现在明确显示基本费用、促销和税费部分，让您更清楚地了解每笔费用的计算方式。

表 1. 上一步
**transaction-type** **amount-type** **amount-description** **amount**
other-transaction 多渠道配送货到付款费用 本金 -35.00
other-transaction 多渠道配送货到付款费用 CGST -3.15
other-transaction 多渠道配送货到付款费用 SGST -3.15

表 2. 现在
**transaction-type** **amount-type** **amount-description** **amount**
AmazonFees 多渠道配送货到付款费用 基本费用 -35.00
AmazonFees 多渠道配送货到付款费用 费用税 - CGST -3.15
AmazonFees 多渠道配送货到付款费用 费用税 - SGST -3.15

**交易名称已移至 amount-type 字段**

我们已将交易名称移至 amount-type 字段，并在结算报告 V1、结算报告 V2 和日期范围报告的 amount-description 字段中加入了额外的详细信息。现在明确显示基本费用、促销和税费部分，让您更清楚地了解每笔费用的计算方式。

表 3. 上一步
**transaction-type** **amount-type** **amount-description** **amount**
FBAFees — 入库缺陷处理费 - 已删除或已弃置的货件 -11.00

表 4. 现在
**transaction-type** **amount-type** **amount-description** **amount**
FBAFees 入库缺陷处理费 - 已删除或已弃置的货件 基础 -11.00

**order-id 和 shipment-id 字段中的标准化交易标识符**

我们已统一交易标识符在结算报告 V1 和结算报告 V2 中的显示位置。此前，与亚马逊物流相关的交易会在 **order-id** 字段中显示其标识符，而非亚马逊物流交易则使用 shipment-id 字段。现在，所有标识符值都显示在 **shipment-id** 字段下，因此您可以在同一位置找到交易标识符。当一笔交易带有两个不同的标识符时，**order-id** 和 **shipment-id** 字段都会填入值。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GSTBL8HHTMPF3DCT
