---
title: "错误 90000644"
doc_id: GCPSED6VQHDV7GTA
source: https://sellercentral.amazon.com/help/hub/reference/external/GCPSED6VQHDV7GTA
language: zh-CN
fetched_at: 2026-10-30T14:20:51
---

# 错误 90000644

## 错误消息

属性 ${attribute_name} 的值 ${attribute_value} 的小数位过多。该值有 ${actual_scale} 位小数，但允许的最大小数位为 ${threshold}。

## 导致错误 90000644 的原因

导致此错误的原因如下：

- 您通过上传数据或手动输入等方式提交的数值包含多于属性允许的小数位数。

- 商品重量、包裹尺寸或建议零售价等属性具有严格的小数级限制，一旦超出允许的阈值（例如，为 ${threshold} 为 2 的属性提交“2.5678”或“0.3333”），就会触发此错误。

## 解决错误 90000644

要解决此错误，请按照以下步骤操作：

- 查看上传数据处理汇总报告，了解突出显示的 attribute_name、属性值以及 actual_value。

- 将值四舍五入或缩减为允许的小数位数，使其包含不超过 ${threshold} 位小数。确保四舍五入后的数值能准确反映商品的规格，不会传递错误的商品信息。

- 更新库存文件中突出显示的 attribute_value，并重新提交更正后的商品信息。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GCPSED6VQHDV7GTA
