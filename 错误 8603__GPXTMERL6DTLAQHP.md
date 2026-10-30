---
title: 错误 8603
doc_id: GPXTMERL6DTLAQHP
source: https://sellercentral.amazon.com/help/hub/reference/external/GPXTMERL6DTLAQHP
language: zh-CN
fetched_at: 2026-10-30 13:47:23
---

# 错误 8603

## 错误消息
即使提交包含新值的上传数据，您也无法更改 SKU ${sku} 的 ${attribute}。要更改此属性，请执行以下操作： 1) 提交上传数据，然后删除现有 SKU。2) 提交上传数据，使用更新后的 ${attribute} 重新创建 SKU。

## 导致错误 8603 的原因
出现此错误的原因如下：
- 您正在尝试通过已锁定且无法更新的上传数据提交来获取现有 SKU 的特定属性。例如：product_id 和变体主题。
- 系统检测到有人试图修改受保护商品属性，这需要完成 SKU 删除和重新创建流程。

## 解决错误 8603
要解决此错误，请执行以下步骤：
1. 提交上传数据，然后完全删除现有 SKU。
2. 接着，提交新的上传数据，使用更新后的属性值重新创建 SKU。
  1. 重新创建 SKU 时，请确保除您想要更改的特定属性外，所有其他属性均与原始商品信息匹配。
  2. 在提交新的上传数据模板文件之前，请仔细检查新属性值是否符合亚马逊的要求和指南。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GPXTMERL6DTLAQHP
