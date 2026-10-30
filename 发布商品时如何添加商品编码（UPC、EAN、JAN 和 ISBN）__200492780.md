---
title: 发布商品时如何添加商品编码（UPC、EAN、JAN 和 ISBN）
doc_id: 200492780
source: https://sellercentral.amazon.com/help/hub/reference/external/200492780
language: zh-CN
fetched_at: 2026-10-30 12:26:47
---

# 发布商品时如何添加商品编码（UPC、EAN、JAN 和 ISBN）

大多数商品分类均要求您提供 GTIN（全球贸易项目代码，也称为商品编码），以便在亚马逊上创建新的商品信息和报价。

如果您在创建新商品信息时未提供 UPC、EAN、JAN 或 ISBN 等商品编码，您将收到一条错误消息。如果您的商品没有商品编码，请参阅[如何发布没有商品编码（UPC、EAN、JAN 或 ISBN）的商品](https://sellercentral.amazon.com/gp/help/external/200426310)。

无论您使用的是“添加新商品”工具、批量上传商品还是 XML 上传数据，“商品编码”字段均为必填字段。有关更多详细信息，请参阅下方。

## 添加新商品
[添加新商品](https://sellercentral.amazon.com/productsearch)工具允许您每次创建一个商品详情页面和一件商品。如果您在该工具中搜索某款商品，且该商品已位于我们的目录中，则系统将自动为您输入商品编码，以便您继续创建商品。如果您创建新的商品信息，则可在完成商品分类后在【添加新商品】页面上输入商品编码。

## 批量上传商品
**Individual sellers：** 此功能仅适用于参与专业销售计划的卖家。有关更多信息，请参阅[销售计划对比](https://sellercentral.amazon.com/gp/help/external/64491)。

【批量上传商品】工具可让您使用预先设定格式的电子表格输入多个商品的数据，然后向亚马逊上传填写完毕的文件。我们会将您的数据与我们目录中的现有商品匹配；如果未找到匹配项，则会创建一个新的商品页面。

准备[库存文件模板](https://sellercentral.amazon.com/gp/help/external/1641)时，请在以下两个字段中输入数据：

- 【product-id：】 商品的唯一标识，即实际的 UPC（12 位数字）、EAN、JAN 或 ISBN（后三种标识均为 13 位数字）。
- 【product-id-type：】 product-id 字段中输入的唯一标识类型，即 UPC、EAN、JAN 或 ISBN。 **注意： **根据您使用的模板，这些字段的名称可能稍有不同。例如，您的模板可能具有 【standard-product-id】 或 【StandardProductID】 字段，而不是 【product-id】 字段。

## XML 上传数据
**Individual sellers：** 此功能仅适用于参与专业销售计划的卖家。有关更多信息，请参阅[销售计划对比](https://sellercentral.amazon.com/gp/help/external/64491)。

如果您使用 [XML 上传数据](https://sellercentral.amazon.com/gp/help/external/221)，请在 【StandardProductID】 元素中提供 UPC。例如：
<StandardProductID> <Type>UPC</Type> <Value>009309013872</Value> </StandardProductID>

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/200492780
