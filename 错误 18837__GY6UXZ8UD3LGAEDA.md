---
title: 错误 18837
doc_id: GY6UXZ8UD3LGAEDA
source: https://sellercentral.amazon.com/help/hub/reference/external/GY6UXZ8UD3LGAEDA
language: zh-CN
fetched_at: 2026-10-30 14:18:11
---

# 错误 18837

## 错误消息
捆绑商品的商品信息类型无效。要解决此问题，请执行以下操作： (1) 验证仅使用一种商品信息类型；(2) 确保“offer_listing_type”设为“purchasable_bundle”；(3) 删除所有相互冲突的商品类型；(4) 使用正确的捆绑商品配置重新提交。

## 导致错误 18837 的原因
由于以下原因导致出现此错误：

- 多个商品信息类型会被分配到单个捆绑商品信息中。
- 捆绑商品配置未将“purchasable_bundle”指定为商品类型。
- 捆绑商品的各组成商品存在相互冲突的商品信息类型。
- 捆绑商品设置包含不兼容的商品信息分类。

## 解决错误 18837
要解决此错误，请按照以下步骤操作：

1. 检查您的捆绑商品配置并删除所有其他商品类型，每个捆绑商品仅保留一种类型。
2. 在您的商品信息设置中将“offer_listing_type”设置为“purchasable_bundle”。
3. 检查捆绑商品的所有组成商品，确保它们被正确配置为捆绑商品信息的一部分。
4. 确认所有设置均符合可购买的捆绑商品要求后，提交更新后的捆绑商品配置。

有关更多信息，请参阅[商品捆绑销售政策](https://sellercentral.amazon.com/help/hub/reference/G200442350)。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GY6UXZ8UD3LGAEDA
