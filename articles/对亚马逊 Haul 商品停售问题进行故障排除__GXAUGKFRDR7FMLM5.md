---
title: "对亚马逊 Haul 商品停售问题进行故障排除"
doc_id: GXAUGKFRDR7FMLM5
source: https://sellercentral.amazon.com/help/hub/reference/external/GXAUGKFRDR7FMLM5
language: zh-CN
fetched_at: 2026-10-30T14:13:14
---

# 对亚马逊 Haul 商品停售问题进行故障排除

**注意： **亚马逊 Haul 商品须遵循与 Amazon.com 商品相同的政策，以及专门针对亚马逊 Haul 的额外政策。要了解更多信息，请参阅[允许在亚马逊 Haul 中销售的选品](https://sellercentral.amazon.com/gp/help/external/GAK9UAJGQRN3Y87A)。无论是亚马逊 Haul 商品还是 Amazon.com 商品，只要是因违反 Amazon.com 政策而导致商品被停售，都会影响您的账户状况评级。而违反专门针对亚马逊 Haul 的政策不会影响您的账户状况评级。要了解更多信息，请参阅[账户状况评级涉及的政策](https://sellercentral.amazon.com/gp/help/external/GQ5DSES264XVXNX7)。本页面介绍了违反专门针对亚马逊 Haul 政策而导致的停售。有关与通用 Amazon.com 政策相关的停售信息，请参阅[计划政策](https://sellercentral.amazon.com/gp/help/external/G521)。

## 确定美国商城的停售商品

要确定亚马逊 Haul 商品是否被停售，请按照以下步骤操作：

- 从卖家平台的下拉菜单中，选择【库存】，然后选择[管理所有库存](https://sellercentral.amazon.com/myinventory/inventory)。

- 点击【在搜索结果中禁止显示的商品和非在售商品】。

如果您对亚马逊 Haul 商品使用了唯一的 SKU 前缀，请在搜索字段中输入该前缀，以筛选已停售的亚马逊 Haul 商品。否则，请按 ASIN 或 SKU 搜索。

按照以下步骤为每个亚马逊 Haul 特定问题类型进行故障排除。

| 错误代码 | 消息 | 解决方案 |
| --- | --- | --- |
| 100721 | 您的商品存在跨境运输限制。目前，亚马逊 Haul 不接受此类商品。 | 请转至下表以获取更多指导。 |
| 100613 | 我们发现亚马逊 Haul 定价错误。商品价格超出亚马逊 Haul 中此商品类型的最高可用商品价格。请通过上传更新商品价格。了解更多信息：https://sellercentral.amazon.com/help/hub/reference/GAK9UAJGQRN3Y87A | 请更新您的商品价格，以符合亚马逊 Haul 中的最高可用商品价格点。 |
| 100721 | 对于储存在亚马逊运营中心的亚马逊 Haul 商品，尺寸测量值不能超过 14 x 8 x 5 英寸（非服装）或 14 x 12 x 5 英寸（服装）。 | 确认您的商品信息是最新且准确的。如果您对亚马逊的尺寸测量值有异议，请联系我们。 |
| 100721 | 对于存储在亚马逊运营中心的亚马逊 Haul 商品，重量不能超过 1 磅（0.45 千克）。 | 确认您的商品信息是最新且准确的。如果您对亚马逊的尺寸测量值有异议，请联系我们。 |
| 100721 | 您的商品已被分类为危险品。目前，亚马逊 Haul 不接受此类商品。 | 亚马逊 Haul 仅接受干电池。请参阅可能的危险品示例。 |
| 100642 | 亚马逊 Haul 中仅可销售状况为全新的商品。如果选错了状况类型，请更正您的商品信息。 | 对于二手商品，没有相应的解决途径。亚马逊 Haul 仅接受状况为全新的商品。 |
| 100644 | 亚马逊 Haul 中仅可销售商品类型符合要求的商品。此商品类型不符合要求。如果选错了商品类型，请更正您的商品信息。 | 如果您的商品分类有误，请联系我们。否则，此商品将不符合亚马逊 Haul 的要求。 |
| 100643 | 只有品牌为 【无品牌】 的商品才允许在亚马逊 Haul 中销售。请更正您的商品信息。 | 将您的品牌名称更新为【无品牌】。 |
| 100721 | 目前，我们获得的信息不足，无法确定亚马逊 Haul 的跨境资格。请确保您的商品信息（包括商品名称、商品描述和要点）完整且最新。 | 我们根据商品信息来确定是否符合计划资格。检查您的商品信息是否提供了完整的商品详情。 |
| 100723 | 不能在亚马逊 Haul 中呈现外部分配的商品编码。请移除外部分配的商品编码，然后重新提交商品信息。 | 删除商品的 UPC、GTIN 或 EAN。 |
| 100640 | 此 ASIN 在亚马逊 Haul 中已被使用。不能使用亚马逊 Haul 的 ASIN 发布 Amazon.com 商品。请删除您的 Amazon.com 商品。您的亚马逊 Haul 商品不受此问题的影响。 | 此错误表示您正尝试在 Amazon.com 和亚马逊 Haul 之间交叉发布某个 SKU。 如果您看到此错误，则表示您的 Amazon.com 商品已被拒绝。只要没有其他问题影响您的亚马逊 Haul 商品，您的亚马逊 Haul 商品将会一直保持在售状态。 如果您想要移除非在售的 Amazon.com 商品，请删除并重新发布此 SKU。重新发布 SKU 时，请务必使用【全部更新】而不是【部分更新】。 |
| 100641 | 您正在尝试向此 SKU 添加亚马逊 Haul 商品，但此 SKU 不属于亚马逊 Haul。如果此 SKU 已在 Amazon.com 上使用，请删除您的亚马逊 Haul 商品，然后创建一个新的 SKU。如果此 SKU 未在使用，请务必在创建商品信息时为 【is_value_stores_item】 选择 【是】。 | 此错误表示您正尝试在 Amazon.com 和亚马逊 Haul 之间交叉发布某个 SKU。 如果您打算创建新的亚马逊 Haul ASIN，请执行以下操作： 如果您使用的是 API，请确保为 【is_value_stores_item】 输入“true”。 如果您使用的是非 Haul 商品电子表格，请确保为 【Is Amazon Haul item】 输入“yes”。 如果您意外交叉发布某个 Amazon.com SKU，则表示您的亚马逊 Haul 商品已被拒绝。只要没有其他问题影响您的亚马逊 Haul 商品，您的亚马逊 Haul 商品将会一直保持在售状态。 如果您想要移除非在售的 Amazon.com 商品，请删除并重新发布此 SKU。重新发布 SKU 时，请务必使用全部更新而不是部分更新。 |
| 100710 | 此 ASIN 已被使用。您在亚马逊 Haul 和 Amazon.com 中必须使用单独的 ASIN 和 SKU。请使用新的 SKU 创建商品信息。 | 此错误表示您正尝试在 Amazon.com 和亚马逊 Haul 之间交叉发布某个 ASIN 或 SKU。您必须使用不同的 ASIN 或 SKU 创建商品信息。 |
| 100612 | Amazon.com 上存在此 SKU。您必须为亚马逊 Haul 使用不同的 SKU。请删除此 SKU 的亚马逊 Haul 商品，然后创建一个新的 SKU。 | 此错误表示您在亚马逊 Haul 中重复使用了 Amazon.com 的 SKU。您必须删除此 SKU 并对亚马逊 Haul 商品使用不同的 SKU。我们建议您使用唯一的 Haul 前缀（例如 Haul-），以免出现此错误。 |

**注意： **亚马逊的卖家助手可以通过此主题提供帮助。对于大多数语言设置，卖家助手还可以直接将您转接至销售伙伴支持。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GXAUGKFRDR7FMLM5
