---
title: "错误 8608"
doc_id: GUKGWYQUXGZ9ZRH5
source: https://sellercentral.amazon.com/help/hub/reference/external/GUKGWYQUXGZ9ZRH5
language: zh-CN
fetched_at: 2026-10-30T14:00:29
---

# 错误 8608

## 错误消息

捆绑商品 SKU“${sku}”的组件商品 SKU 不足。捆绑商品必须至少包含两个组件商品。请向捆绑商品添加其他组件商品，然后重新提交上传数据。

## 导致错误 8608 的原因

导致此错误的原因如下：

- 捆绑商品仅包含一个组件商品 SKU，违反了包含两个组件商品的最低要求。

- 捆绑商品中的部分组件商品 SKU 被删除或停售，剩余的在售组件商品少于两个。

- 捆绑商品上传数据文件不完整或缺少组件商品 SKU 条目。

## 解决错误 8608

要解决此错误，请按照以下步骤操作：

- 检查您的捆绑商品配置，并确保您已指定至少两个不同的组件商品 SKU。

- 验证您的目录中是否存在所有组件商品 SKU 且均为在售商品。无效或非在售 SKU 不会计入最低要求。

- 从捆绑商品配置中移除任何重复的组件商品 SKU，因为它们仅会计入最低要求。

- 检查您的商品上传数据格式，确认捆绑商品组件的格式正确且每个组件商品 SKU 均单独列出，然后重新提交文件。要了解有关创建捆绑商品的更多信息，请参阅[商品捆绑销售政策](https://sellercentral.amazon.com/gp/help/external/G200442350)。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GUKGWYQUXGZ9ZRH5
