---
title: 错误 8066
doc_id: GNZVG487LVKE6YDW
source: https://sellercentral.amazon.com/help/hub/reference/external/GNZVG487LVKE6YDW
language: zh-CN
fetched_at: 2026-10-30 13:46:16
---

# 错误 8066

**什么原因会导致错误 8066**

如果您在商品模板中引用的父 SKU 未被正确设置为父商品，则会出现此错误。常见原因如下所示：
- 您对变体中的父 SKU 输入了错误的 SKU。
- 您输入了正确的 SKU，但在创建此 SKU 时未将其指定为父 SKU。
- 您输入了正确的 SKU，但有其他错误导致无法正确设置父 SKU。
- 您在 【Parent SKU】 列中为本身也是父 SKU 的商品输入了一个值。（父 SKU 不能同时也是某个父 SKU 的子商品。）

**错误消息**

在设置变体关系之前，请指明商品是父变体。

**如何解决和避免错误 8066**

要使用商品模板解决此错误，请按照以下步骤操作：
1. 确保在商品模板的 【Parent SKU】 列中输入正确的 SKU。
2. 查找父 SKU 所在的行，并确保其在 【Parentage】 列中的值为“parent”。
3. 查看之前的错误报告，了解与此父 SKU 有关的错误，并按需更正错误。
4. 重新提交商品模板。

**注意： **如果商品未被归类为“parent”（父商品），且此字段留空，则默认值为“child”。 只有通过一次完整的更新，删除并重新创建此 SKU 后，错误才能得到更正。在这种情况下，请在删除后等待 24 小时，再执行重新创建操作。

父 SKU 必须符合以下各项要求：
- 商品分类为“parent”
- 具有与此系列的所有子 SKU 一致的有效【变体主题】值
- 没有对实际商品进行定义的属性（例如，条形码、商品价格，或尺码、颜色等变体属性）
- 具有适用于所有子 SKU 的通用属性（例如，商品类型或品牌）

有关设置变体的更多信息，请参阅[创建和管理商品变体](https://sellercentral.amazon.com/gp/help/external/GEKYC26YEZX2VSHM)。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GNZVG487LVKE6YDW
