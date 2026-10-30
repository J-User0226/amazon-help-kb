---
title: 针对向买家配送的亚马逊物流商品提供序列号追踪服务
doc_id: GQRHXMHF4DLBSJJD
source: https://sellercentral.amazon.com/help/hub/reference/external/GQRHXMHF4DLBSJJD
language: zh-CN
fetched_at: 2026-10-30 13:49:13
---

# 针对向买家配送的亚马逊物流商品提供序列号追踪服务

对于品牌在 [Transparency 计划](https://brandservices.amazon.com/transparency)中注册的所有商品，亚马逊现在可在卖家平台上为卖家提供序列号追踪服务。

在将商品从亚马逊运营中心配送给买家期间，这些商品可针对每个亚马逊物流订单享受序列号扫描服务。

**注意： **目前，已在美国、加拿大、英国、德国、法国、意大利、西班牙、印度、日本和澳大利亚推出 Transparency 计划。

## 如何享受亚马逊物流序列号追踪服务
如果您是知识产权所有者，并且您的品牌已在 Brand Registry 中注册，请首先确保您的商品已在 Transparency 中注册。要开始使用，请参阅我们的[计划页面](https://brandservices.amazon.com/transparency)。

如果您是转销商，您会收到一封电子邮件，告知您销售的商品已注册加入 Transparency 计划。您还会在 Send to Amazon 货件创建工作流程中看到一条通知，告知商品已注册加入该计划。有关更多信息，请参阅 [Transparency 序列号条形码要求](https://sellercentral.amazon.com/gp/help/external/G202008510)。

**重要： **请勿从运送至运营中心的商品上移除商品序列号条形码。所有移除了序列号条形码的商品将无法加入该计划。如果发生这种情况，您会收到电子邮件通知，并在卖家平台中看到所有无法扫描的商品显示有【存在瑕疵】状态。

以下情况会影响向买家配送的亚马逊物流商品的序列号追踪：
- **虚拟追踪**： 对于通过制造商条形码追踪的商品，已扫描并发送给买家的商品可能是来自发布相同 ASIN 的其他卖家。如果您选择了[虚拟追踪](https://sellercentral.amazon.com/gp/help/external/G200141480)，那么我们可以使用不同卖家的同款商品来配送订单。然后，您会获得实际不是您库存的商品的序列号追踪信息。
- 如果您未选择虚拟追踪，那么您只会获得来自您库存的商品的序列号追踪信息。

- **停用 Transparency 检查**： 由于品牌方在粘贴 Transparency 序列号条形码时贴标不当，或者品牌方选择从该计划中退出了其 ASIN，因此停用了 Transparency 检查。在这种情况下，您将无法享受序列号追踪服务。

## 查找您的序列号追踪信息
在对您符合要求的商品完成扫描后，您可以在以下位置找到亚马逊物流序列号追踪信息：
- [管理订单](https://sellercentral.amazon.com/gp/orders-v2/list)和订单详情页面
- [所有订单报告](https://sellercentral.amazon.com/reportcentral/FlatFileAllOrdersReport/1)

**注意： **要在“所有订单”报告中添加或删除序列号追踪列，请转至[订单报告](https://sellercentral.amazon.com/order-reports-and-feeds/reports)，点击【添加或删除订单报告列】，然后选择您想要的列选项。

通过此信息，您可以准确了解某一订单所配送的序列号。

如果您是使用 API 检索订单信息，则可以连接到现有的[销售伙伴 API - Get/orders/orderItems](https://developer-docs.amazon.com/sp-api/docs/orders-api-v0-reference#getorderitems) 以获得序列号信息。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GQRHXMHF4DLBSJJD
