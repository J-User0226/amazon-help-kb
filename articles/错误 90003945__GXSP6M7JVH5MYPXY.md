---
title: "错误 90003945"
doc_id: GXSP6M7JVH5MYPXY
source: https://sellercentral.amazon.com/help/hub/reference/external/GXSP6M7JVH5MYPXY
language: zh-CN
fetched_at: 2026-10-30T14:21:37
---

# 错误 90003945

## 错误消息

根据“${preconditions}”的数据，属性“${attribute_name}”字段“${field}”中的“${value}”不是有效值。请提供一个有效值。

## 错误原因

更新后的字段名称值无效。如果您提交的信息（前提条件）中具有特定值组合，则您将无法提供值。

## 示例

错误消息：

根据“[shapewear_size#?.size_class, shapewear_size#?.size_system, age_range_description.value, target_gender.value]”的数据，属性“[shapewear_size]”字段“size”中的值“numeric_80”不是有效值。请提供一个有效值。

在上述示例中，根据为前提条件选择的属性值 [塑身衣尺码等级、年龄范围描述和目标群体性别属性]，不能将尺码值选为 80。

## 解决此错误的步骤

- 检查前提条件。

- 移除无效值，并根据前提条件使用有效值进行更新。请参考模板中的“有效值”工作表。

- 重新上传此上传数据文件进行提交。

如果您使用 Excel 文件发布商品，可参阅模板中的【有效值】工作表。您可以从[库存文件模板](https://sellercentral.amazon.com/gp/help/external/1641)下载最新模板。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GXSP6M7JVH5MYPXY
