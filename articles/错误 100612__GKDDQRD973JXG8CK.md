---
title: 错误 100612
doc_id: GKDDQRD973JXG8CK
source: https://sellercentral.amazon.com/help/hub/reference/external/GKDDQRD973JXG8CK
language: zh-CN
fetched_at: 2026-10-30 15:26:45
---

# 错误 100612

## 错误消息
Amazon.com 上存在此 SKU。您必须为亚马逊 Haul 使用不同的 SKU。请删除此 SKU 的亚马逊 Haul 商品，然后创建一个新的 SKU。

## 导致错误 100612 的原因
出现此错误的原因如下：
- 您尝试在 Amazon.com 和亚马逊 Haul 上使用相同的 SKU。系统拒绝此操作，因为每个商城都需要唯一的 SKU。
- 您在亚马逊 Haul 上上传的库存文件包含已在 Amazon.com 上使用的 SKU。
- 您在未更改 SKU 值的情况下将商品信息从 Amazon.com 复制到了亚马逊 Haul。
- 您删除了 Amazon.com 上的商品信息，并在系统完成删除处理之前就立即尝试在亚马逊 Haul 上重新使用该 SKU。

## 解决错误 100612
要解决此错误，请按照以下步骤操作：
1. 通过找到错误消息中提到的 SKU 删除现有亚马逊 Haul 商品，按亚马逊 Haul 商城进行筛选，然后删除冲突的商品。
2. 为您的亚马逊 Haul 商品生成一个与您的 Amazon.com SKU 不同的 SKU 编码。例如，如果您的 Amazon.com SKU 为“PROD-12345”，则应为亚马逊 Haul 创建“HAUL-PROD-12345”或“PROD-12345-AH”，以保持明确的区分。
3. 使用新的 SKU 在亚马逊 Haul 上重新发布商品。确保所有商品详情、图片和属性均符合[亚马逊 Haul](https://sellercentral.amazon.com/help/hub/reference/GMULTR2SMZ6WWX57) 的要求。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GKDDQRD973JXG8CK
