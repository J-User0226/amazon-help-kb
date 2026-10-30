---
title: 关键词属性说明
doc_id: GF2C2L6RCFZGWBXC
source: https://sellercentral.amazon.com/help/hub/reference/external/GF2C2L6RCFZGWBXC
language: zh-CN
fetched_at: 2026-10-30 13:32:22
---

# 关键词属性说明

## 概览
下表说明了卖家在管理商品信息时遇到的关键词属性。大部分关键词属性需要有效值，这些值可在[分类树指南 (BTG)](https://sellercentral.amazon.com/gp/help/external/G1641) 中找到。属性 specific_uses_keywords、thesaurus_attribute_keywords 和 target_audience_keywords 主要在美国使用，并且正在逐步停用。可以为 generic_keywords 和 subject_keywords 输入自由文本。subject_keywords 应仅用于媒介类商品。您无需填充 platinum_keywords，因为它们现在是多余的。

字段名 属性名称 描述 值 长度限制（字节） 按搜索索引？ 按浏览使用？
【预期用途】 specific_uses_keywords 描述商品使用的上下文，可以是活动或位置，例如游戏、卧室等。此属性主要在美国使用，并且正在逐步停用。 不适用（正在逐步停用） 150
【商品类型关键字 (ITK)】 item_type_keyword ITK 会自动将商品分配到分类节点，主要在美国使用。 请参阅分类树指南中的有效值。 250
【其他属性】 thesaurus_attribute_keywords 描述商品的特征，如防水、深色闪光。此属性主要在美国使用，并且正在逐步停用。 不适用（正在逐步停用） 不适用
【白金关键词】 platinum_keywords 不再使用。此属性之前用于填充白金卖家店铺，但现在是多余的。 不适用（逐步停用） 不适用
【搜索词】 generic_keywords 描述商品。[请参阅帮助页面](https://sellercentral.amazon.com/gp/help/external/23501)。 自由文本。 249
【特定风格的术语】 style_keywords 描述服装商品，例如脚踝靴、毛皮衬垫。 请参阅分类树指南中的有效值。 100
【主题关键词】 subject_keywords 主题关键词应仅用于描述媒介类商品。 自由文本。 210
仅媒介类商品

【主题】 thesaurus_subject_keywords 描述商品上的描绘内容，例如描绘马的海报。 请参阅分类树指南中的有效值。 250
【目标消费群体】 target_audience_keywords 描述目标最终用户，例如女性、儿童、狗。此属性主要在美国使用，并且正在逐步停用。 不适用（正在逐步停用） 不适用
#### 如何使用这些数据？
卖家填写属性，亚马逊使用这些数据帮助买家找到商品。例如，亚马逊使用这些数据为买家关键词搜索生成搜索结果。该数据还用于自动将商品分配到分类导航中，这是买家查找商品的另一种方式。例如，“style_keywords:sport-sandals”的分类分配查询会将 style_keywords 值为 sport-sandals 的商品分配到“运动凉鞋”分类节点。

#### 我应该使用下拉列表还是自由文本？
在卖家平台中添加或编辑商品信息时看到的“关键词”选项卡上，卖家可以选择一个下拉值或输入自由文本。自由文本必须与分类树指南中列出的有效值匹配，以便在分类查询中使用数据。亚马逊不会发布有效值的完整列表，而是会指导卖家查看与其销售商品分类相对应的分类树指南，以确保他们重点关注与其相关的值。

#### 长度限制
搜索词 (generic_keywords) 的长度应少于 250 个字节（[阅读更多](https://sellercentral.amazon.com/gp/help/external/G23501)）。如果超出限制，亚马逊搜索将完全忽略该属性。

对于上表中的其他长度限制，如果超出限制，亚马逊搜索会在长度限制之前进行索引并忽略任何多余限制。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GF2C2L6RCFZGWBXC
