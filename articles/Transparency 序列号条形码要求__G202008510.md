---
title: "Transparency 序列号条形码要求"
doc_id: G202008510
source: https://sellercentral.amazon.com/help/hub/reference/external/G202008510
language: zh-CN
fetched_at: 2026-10-30T12:59:26
---

# Transparency 序列号条形码要求

现在，部分制造商使用 Transparency 2D 条形码或序列号条形码为其商品贴标，以便更好地追踪商品库存，同时达到防伪的目的。如果您要在亚马逊商城销售已加入 Transparency 计划的商品，则这些商品必须相应地贴有 Transparency 码或品牌提供的序列号条形码。您从供应商处采购的已加入 Transparency 计划的 ASIN 也必须包含 Transparency 码或序列号条形码。

点击[此处](https://brandservices.amazon.com/transparency)，了解有关 Transparency 的更多信息。

## 识别已加入 Transparency 计划的商品序列号

若商品已加入 Transparency 计划，其包装上将带有序列号。

这些序列号可能采用 5 种格式。以下是最常见的两种格式：

- 以“AZ:”或“ZA:”开头的 26 位字母数字编码。例如，AZ:L1Z2H38F4C5Q6R7E5K6Z1C2K3E，总长度为 29 个字符。

- 序列化全球贸易项目代码。例如，0100376204200301214P1OZMT7D8B81EMF4WW4，总长度为 38 个字符。

【Transparency 码示例】

![](https://d1n436oh1t0g4d.cloudfront.net/G3TJ7D79PGC48LGD_Global_zh-CN.gif)

![](https://d1n436oh1t0g4d.cloudfront.net/GUSZKWBMV5JDTLD3_Global_zh-CN.gif)

![](https://d1n436oh1t0g4d.cloudfront.net/G5VWFFJK64N4XEFH_Global_zh-CN.gif)

![](https://d1n436oh1t0g4d.cloudfront.net/GB5Y8T9CNFVJ962E_Global_zh-CN.gif)

【序列号示例】

如果您找不到带有 【T】 标志的代码，请查找长度为 7 至 20 个字符的序列号代码。序列号可能是 1D、2D 或二维码，并且可能会包含前缀“SN”。序列号代码将会与 GTIN (UPC/EAN/ISBN) 条形码粘贴在包装的同一侧。

**注意： **输入序列号时，请勿包含前缀（如 【SN】）或【服务标签】，而应从序列号本身的字符开始输入。

![](https://d1n436oh1t0g4d.cloudfront.net/GTAG3PHSS5N44JZ6_Global_zh-CN.png)

## 如何在买家订单中识别已加入 Transparency 计划的序列号

您可以通过两种方式识别已加入 Transparency 计划的商品：

已注册 Transparency 计划的 ASIN 会以蓝色 Transparency 标记 
![](https://m.media-amazon.com/images/G/31/rainier/IMG13.png)
或橙色序列号标记 
![](https://d1n436oh1t0g4d.cloudfront.net/GKJGK6SNE6NCCQVS_Global_zh-CN.png)
突出显示在卖家平台中的【管理订单】页面上。对于这些 ASIN，您必须在确认发货时提供 Transparency 码或序列号。

您还可以前往[订单报告](https://sellercentral.amazon.com/order-reports-and-feeds/reports)：

- 在【订单报告】中，点击页面标题下方的[添加或移除订单报告列](https://sellercentral.amazon.com/order-reports-and-feeds/column-picker)链接。

- 在【添加或移除订单报告列】中的【选填列】下方，启用 【Transparency】 列。

完成上述操作后，当您下载报告时，Transparency 字段将会自动显示。

如果订单报告中此字段（“is-Transparency”）的值设置为“True”，那么您必须在确认发货时为这些 ASIN 上传 Transparency 码。

如果没有 Transparency 码，您需要上传序列号。请查找长度为 7 至 20 个字符的序列号代码。序列号可能是 1D、2D 或二维码，并且可能会包含前缀 【SN】。序列号代码将会与 GTIN (UPC/EAN/ISBN) 条形码粘贴在包装的同一侧。

**注意： **您上传的 Transparency 码或序列号的数量必须与订单中已加入 Transparency 计划的商品数量保持一致。例如，如果已加入 Transparency 计划的商品数量为 3，请确保上传 3 个唯一的 Transparency 码或序列号。

在亚马逊销售伙伴 API 中检索订单详情时，请使用 getOrderItems API 找出包含已加入 Transparency 计划的商品订单。有关更多信息，请参阅 [getOrderItems](https://developer-docs.amazon.com/sp-api/docs/orders-api-v0-reference#getorderitems)。

## 使用发货确认文件上传 Transparency 码或序列号

请按照以下步骤在卖家平台中下载相应的文件模板。

- 前往【订单】选项卡，然后从下拉菜单中选择【上传订单相关文件】

- 在【“1. 准备您的发货确认文件”】下方，点击【下载模板】

- 填写好此模板后，点击【选择文件】（位于 【2. 上传您的发货确认文件】下方）

即使通过其他工具（如销售伙伴 API (SP-API) 或第三方软件）确认了发货，您也可以使用此模板上传 Transparency 码或序列号（如果没有 Transparency 码）。

## 在卖家平台中上传 Transparency 码或序列号

已注册 Transparency 计划的 ASIN 会以蓝色 Transparency 标记 
![](https://m.media-amazon.com/images/G/31/rainier/IMG13.png)
或橙色序列号标记 
![](https://d1n436oh1t0g4d.cloudfront.net/GKJGK6SNE6NCCQVS_Global_zh-CN.png)
突出显示在卖家平台中的[管理订单](https://sellercentral.amazon.com/orders-v3?page=1)页面上。

请按照以下步骤，对带有 Transparency 码或序列号的商品进行确认、上传和发货：

- 前往[管理订单](https://sellercentral.amazon.com/orders-v3?page=1)，找到带有 Transparency 或序列号标记的订单。

- 点击【订单编号】，前往【订单详情】页面。

- 点击【购买配送】或【确认发货】，在底部打开一个新的版块。在底部的新版块中输入 Transparency 码或序列号。

- 在【订单详情】页面底部的【数量】字段正下方有一个 【T】 标记。点击【输入 Transparency 码或序列号】链接。在文本框中输入或扫描 Transparency 码或序列号。

- 输入代码或序列号后，您可以继续配送订单。

## 在销售伙伴 API CreateFeed API 中确认发货并上传 Transparency 码

如果您在亚马逊销售伙伴 API 中确认发货，则可以使用 CreateFeed API 为包含已加入 Transparency 计划的 ASIN 的订单上传 Transparency 码。有关更多信息，请参阅 [CreateFeed](https://developer-docs.amazon.com/sp-api/docs/feeds-api-v2021-06-30-reference#createfeed)。

**注意： **您只能使用 【CreateFeed API】 上传 Transparency 码。对于带有序列号的商品，请通过【订单详情】页面或使用【发货确认】文件上传序列号。

## 在销售伙伴 API CreateShipment API 中购买配送服务并上传 Transparency 码

如果您在亚马逊销售伙伴 API 中购买配送服务，则可以使用 【CreateShipment API】 为包含已加入 Transparency 计划的 ASIN 的订单上传 Transparency 码。有关更多信息，请参阅 [CreateShipment](https://developer-docs.amazon.com/sp-api/docs/merchant-fulfillment-api-v0-reference#createshipment)。

**注意： **您只能使用 【CreateFeed API】 上传 Transparency 码。对于带有序列号的商品，请通过【订单详情】页面或使用【发货确认】文件上传序列号。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/G202008510
