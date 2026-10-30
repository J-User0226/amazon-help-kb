---
title: "错误 100398"
doc_id: GMGJ43YG3DLEJDP4
source: https://sellercentral.amazon.com/help/hub/reference/external/GMGJ43YG3DLEJDP4
language: zh-CN
fetched_at: 2026-10-30T13:43:28
---

# 错误 100398

## 错误消息

SKU '${sku}' 已在其他亚马逊商城中存在。使用新的 SKU，然后重新提交您的商品信息。

## 导致错误 100398 的原因

出现此错误的原因如下：

- 您提交的 SKU 已在其他亚马逊商城中存在。亚马逊要求每个 SKU 在您卖家账户的所有商城中都是唯一的。这适用于以下情况：

- 您使用已在其他商城中使用的 SKU 创建新商品信息。

- 您的批量上传模板或库存文件上传数据中包含与其他商城 SKU 存在冲突的 SKU。

- 您重复使用了之前在其他商城中已被删除或停售商品的 SKU。即使删除后，该 SKU 仍可能与您的卖家账户关联

## 解决错误 100398

要解决此错误，请按照以下步骤操作：

- 前往您拥有活跃账户的各个商城的卖家平台，找到存在冲突的 SKU。前往【库存】 > 【库存】。搜索冲突的 SKU 并注明其属于哪个商城。记录商城和商品详情以供参考。

- 通过更新您的 SKU 以包含商城特定编码，创建新的唯一 SKU。这有助于确保每个 SKU 在所有商城中都是唯一的。

- 通过编辑商品信息草稿、模板文件上传或 API 有效负载来更新您提交的商品信息。使用新的唯一 SKU 替换存在冲突的 SKU。 验证新 SKU 是否与您所有商城中的现有 SKU 存在冲突。

- 保存您的更改，然后重新提交商品信息。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GMGJ43YG3DLEJDP4
