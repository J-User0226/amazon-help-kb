---
title: "错误 90004117"
doc_id: GHA8BFE4EQWSTHQG
source: https://sellercentral.amazon.com/help/hub/reference/external/GHA8BFE4EQWSTHQG
language: zh-CN
fetched_at: 2026-10-30T14:21:07
---

# 错误 90004117

## 错误消息

属性 ${attribute_name} 最多允许出现 ${max_count} 次，但当前出现 ${actual_count} 次。

## 导致错误 90004117 的原因

由于以下原因导致出现此错误：

- 指定属性的出现次数超过了允许的限制。

- 只允许一个条目时，上传数据中却包含同一属性的重复条目。

- 只允许一个变体时，却提交了同一属性的多个变体。

## 解决错误 90004117

要解决此错误，请按照以下步骤操作：

- 查看您的上传数据处理汇总报告，并查看突出显示的属性及其允许的实际出现次数和最大出现次数。

- 删除该属性的任何重复或冗余实例，仅保留最相关的条目。

- 修改您的数据上传结构，确保每个属性的出现次数不超过其允许的出现次数限制。

- 使用有效值更新后，重新提交文件。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GHA8BFE4EQWSTHQG
