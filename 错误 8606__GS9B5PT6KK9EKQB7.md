---
title: 错误 8606
doc_id: GS9B5PT6KK9EKQB7
source: https://sellercentral.amazon.com/help/hub/reference/external/GS9B5PT6KK9EKQB7
language: zh-CN
fetched_at: 2026-10-30 13:50:29
---

# 错误 8606

## 错误 8606
## 错误消息
组件 SKU“${component_skus}”全部映射到捆绑商品“${bundle_sku}”中的同一 ASIN，这是不允许的。请按照以下指示进行操作，然后重新提交上传数据： 1) 删除上述列出的所有组件 SKU，只保留其中一个。2) 指定一个数量，以便多次包含该组件。

## 导致错误 8606 的原因
导致此错误的原因如下：
- 捆绑商品中的多个组件 SKU 映射到同一 ASIN，导致在单个捆绑商品配置中创建了重复的 ASIN 引用。
- 系统检测到捆绑商品 SKU 中列出的所有组件均引用相同的商品编码。
- 您试图将同一商品作为单独的组件发布，而不是指定单个组件的数量，导致多次将同一商品包含在捆绑商品中。

## 解决错误 8606
要解决此错误，请按照以下步骤操作：
1. 查看上传数据处理汇总报告，以确定 bundle_sku 中的哪些 component_sku 值映射到同一 ASIN。
2. 从您的上传数据中删除映射到同一 ASIN 的重复组件 SKU。对于捆绑商品中的每个唯一 ASIN，仅保留一个 SKU 引用。
3. 如果您打算在捆绑商品中包含多件相同的商品，请删除重复的 SKU 条目，改为使用该单个组件 SKU 的数量字段指定所需的数量。
4. 更新组件 SKU 后，请重新提交上传数据文件。

**注意： **捆绑商品组件必须是唯一的 ASIN，才能维持正确的目录结构和库存追踪。系统会防止组件重复，以免在订单处理和配送过程中产生混淆。在创建捆绑商品之前，请务必确认您的组件 SKU 映射到不同的 ASIN，或在需要多件相同的商品时使用数量属性。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GS9B5PT6KK9EKQB7
