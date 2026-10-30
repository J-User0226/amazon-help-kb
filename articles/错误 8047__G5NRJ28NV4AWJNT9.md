---
title: 错误 8047
doc_id: G5NRJ28NV4AWJNT9
source: https://sellercentral.amazon.com/help/hub/reference/external/G5NRJ28NV4AWJNT9
language: zh-CN
fetched_at: 2026-10-30 13:19:18
---

# 错误 8047

**什么原因会导致错误 8047**

当 SKU 作为子变体提交，但它与父变体的 ASIN 匹配时，就会出现此错误。当提供错误的 ASIN 作为外部商品编码时，通常会发生这种情况。

**错误消息：**

SKU 作为子变体提交，但它与父变体的 ASIN 匹配。当提供错误的 ASIN 作为外部商品编码时，通常会发生这种情况。请使用除 ASIN 之外的其他商品编码（例如 UPC 或 ISBN）重新提交您的商品。

**如何解决和避免错误 8047**

要解决此错误，请使用除 ASIN 以外的正确商品编码（如 UPC 或 ISBN）或亚马逊商城中现有的正确子 ASIN 重新提交 SKU。

**注意： **如果您希望将此 ASIN 用于新的商品信息，请重新提交商品信息，并在 【Parentage】 字段中填写“parent”。或者，对于新的商品信息，请先删除 SKU，然后重新创建商品信息，并在 【Parentage】 字段中填写“parent”。

请按照以下步骤解决错误：
1. 在 【SKU】 列中输入要删除的 SKU。除 【Update delete】 列之外，其他列为非必填项。
2. 在 【Update delete】 列中输入“delete”。
3. 提交修改后的商品模板。此时，系统将从亚马逊删除所有在售报价。您可能需要等待 24 小时才能重新使用此 SKU。
4. 在商品模板中将此 SKU 的商品数据更改为新值，并将您在 【Update delete】 列中输入的“delete”值更改为“update”。 **注意： **请确保商品价格和数量的值正确无误。更改为“update”值后，系统将重新创建您的 SKU 并发布此商品进行销售。

5. 提交更新后的商品模板。

有关其他商品编码的信息，请参阅[查找商品编码 (GTIN)](https://sellercentral.amazon.com/gp/help/external/G200211450)。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/G5NRJ28NV4AWJNT9
