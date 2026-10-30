---
title: 错误 100618
doc_id: GP7M8UG8HGEVTXAF
source: https://sellercentral.amazon.com/help/hub/reference/external/GP7M8UG8HGEVTXAF
language: zh-CN
fetched_at: 2026-10-30 13:46:25
---

# 错误 100618

## 错误消息
您不能使用此 UPC ${contribution_upc} 创建商品信息。再次提交无 UPC 的商品信息。

## 导致错误 100618 的原因
导致此错误的原因如下：
- ${contribution_upc} 中提供的 UPC 值已被确定为不符合用于创建新商品信息的要求。
- 您试图在以下分类中使用 UPC 创建商品信息：需要申请 UPC 豁免的分类，或品牌所有者已在亚马逊 Brand Registry 中注册并限制第三方使用其 UPC 的分类。
- 您试图提交一个无效、无法识别或格式错误的 UPC。
- ${contribution_upc} 中的 UPC 已与亚马逊目录中的现有 ASIN 关联，系统会阻止使用同一 UPC 创建重复的商品信息。

## 解决错误 100618
要解决此错误，请按照以下步骤操作：
1. 检查亚马逊目录中是否已有此商品。如果存在匹配的 ASIN，请将您的商品添加到现有商品信息，而不是创建新商品。
2. 确认 UPC 是否有效、格式正确且已注册到您的商品。若是，请更正存在的问题并重新提交。若无效或未注册，请从提交内容中移除 UPC 值，并重新提交不含商品编码的版本。
3. 对于模板文件或库存上传数据提交，请打开上传模板并清除“external_product_id”字段，然后将受影响 SKU 的“external_product_id_type”字段留空。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GP7M8UG8HGEVTXAF
