---
title: 错误 100641
doc_id: GPCANQFEQ7M5T49B
source: https://sellercentral.amazon.com/help/hub/reference/external/GPCANQFEQ7M5T49B
language: zh-CN
fetched_at: 2026-10-30 13:46:36
---

# 错误 100641

## 错误消息
您正在尝试向此 SKU 添加亚马逊 Haul 商品，但此 SKU 不属于亚马逊 Haul。如果此 SKU 已在 Amazon.com 上使用，请删除您的亚马逊 Haul 商品，然后创建一个新的 SKU。如果此 SKU 未在使用，请确保在创建商品信息时为 is_value_stores_item 选择“是”。

## 导致错误 100641 的原因
出现此错误的原因如下：
- 您尝试向原为未指定亚马逊 Haul 的标准 Amazon.com 商城商品信息创建的现有 SKU 添加亚马逊 Haul 报价。
- 您提交的商品信息试图通过添加特定于 Haul 的属性或定价将现有的非 Haul SKU 转换为亚马逊 Haul 报价，但系统检测到该 SKU 在创建期间未使用所需的 is_value_stores_item 标记进行初始化。
- 您使用 Amazon.com 库存中已存在且未指定亚马逊 Haul 的 SKU 编码创建新商品信息，并尝试将同一 SKU 用于 Haul 报价。
- 您提交的批量上传上传数据或 API 包含之前创建的 SKU 的亚马逊 Haul 商品数据，但这些数据未在初始商品信息创建流程中将 is_value_stores_item 属性设置为“是”。
- 您试图使用正在用于标准 Amazon.com 商品的 SKU 在亚马逊 Haul 中发布商品，从而导致系统无法确定该 SKU 应被视为常规商城商品信息还是亚马逊 Haul 计划商品信息的冲突。

## 解决错误 100641
要解决此错误，请按照以下步骤操作：
- 确定您的 SKU 当前是否正在使用中：导航至【库存】，然后在卖家平台中选择【管理库存】。搜索错误消息中提及的 SKU，并检查其是否显示在您的在售库存中，且现有报价、销售历史记录或库存数量显示其正在用于标准商品信息。
- 如果 SKU 已在使用中，请删除亚马逊 Haul 报价尝试。在您的库存控制面板中找到失败的 Haul 商品信息，选择该商品信息，然后点击【删除】选项，以移除错误的 Haul 报价尝试。确认删除，将该错误从您的账户中清除。
- 专门为亚马逊 Haul 创建新的 SKU：前往【目录】并选择**添加商品**。输入当前未在您的库存中使用的唯一 SKU 编码，开始新的商品信息创建流程。
- 使用适当的属性完成亚马逊 Haul 商品信息：填写所有必需的商品信息，包括商品名称、描述、图片和符合亚马逊 Haul 要求的定价（通常为基于价值的定价），以及任何 Haul 特定属性。在提交前验证 【is_value_stores_item】 标记是否设置为【是】，并使用正确指定的 SKU 保存新的 Haul 商品信息。
- 验证新的 Haul 商品信息为在售状态：检查您的库存控制面板以确认新的 SKU 显示为【在售】状态，且被正确指定为亚马逊 Haul 报价。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GPCANQFEQ7M5T49B
