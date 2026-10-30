---
title: "错误 8045"
doc_id: G49V6WDHJRCNSU9D
source: https://sellercentral.amazon.com/help/hub/reference/external/G49V6WDHJRCNSU9D
language: zh-CN
fetched_at: 2026-10-30T13:17:43
---

# 错误 8045

## 什么原因会导致错误 8045？

商品分类是指如何将 SKU 设置为一种关系。对于每个 SKU，可以是“父项”或“子项”。这在商品上传数据的“父子关系”列中定义。如果留空，则默认为“子项”。

当某个 SKU 提交的商品分类与现有值冲突时，会导致错误 8045。例如，SKU [ABC] 在美国商城中被分类为“父项”，而您提交的上传数据中，同一 SKU 被分类为“子项”。

## 错误消息：

SKU 在一个或多个商城中为父变体，但在另外一个或多个商城中为子变体。一个 SKU 应该在所有商城中具有相同的父子关系。请重新提交具有正确父子关系的 SKU，确保其在所有商城中保持一致。

## 解决和避免错误 8045 的步骤：

提交商品上传数据时，请确保 SKU 具有一致的商品分类。如果您必须将 SKU 分类从子项更改为父项，则必须在所有在售商城中删除该 SKU，然后重新创建 SKU。请务必在删除后等待 24 小时，再重新创建。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/G49V6WDHJRCNSU9D
