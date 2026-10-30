---
title: "错误 8684"
doc_id: GKDKNT3DP4MMUGCK
source: https://sellercentral.amazon.com/help/hub/reference/external/GKDKNT3DP4MMUGCK
language: zh-CN
fetched_at: 2026-10-30T13:41:03
---

# 错误 8684

**错误消息**

SKU [actual sku value] 错误地与多个 GCID 关联。请为此 SKU 以及 merchant_suggested_asin 属性具有同一属性值的所有其他 SKU 发送一个执行“删除”操作的上传数据，然后重新提交这些 SKU。

**错误 8684 产生原因**

您提交的 SKU 与多个 ASIN 关联。根据 GCID，检查您尝试提交的 SKU 是否在卖家的目录中存在重复问题。

**使用案例**

**案例 1： 适用于新提交的内容**

提供一个唯一的 SKU 值。如果您提交的 SKU 正确无误，并且必须用于创建新 ASIN，那么请提供一个唯一的 SKU 值。如果您提交的 SKU 正确无误，并且必须用于创建新 ASIN，那么请为之前提交的 SKU 发送一个执行“删除”操作的上传数据，然后重新提交。

**案例 2： 适用于更新之前提交的内容**

对于您尝试提交且已与 ASIN 链接的 SKU，请为该 SKU 的 merchant_suggested_asin 提供值，以便系统识别该 SKU，避免出现错误。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GKDKNT3DP4MMUGCK
