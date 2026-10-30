---
title: 错误 90232
doc_id: GRZKQGN5J3PDK45P
source: https://sellercentral.amazon.com/help/hub/reference/external/GRZKQGN5J3PDK45P
language: zh-CN
fetched_at: 2026-10-30 13:50:18
---

# 错误 90232

## 错误消息
属性“${attribute_name}”的值“${attribute_value}”的小数位过多。该值有 ${actual_scale} 位小数，但允许的最大小数位为“${threshold}”。

## 导致错误 90232 的原因
由于以下原因导致出现此错误：
- 输入的小数值的位数多于系统允许的位数。
- 商品测量值或定价数据超过了最大小数位数阈值。

## 解决错误 90232
要解决此错误，请按照以下步骤操作：

- 查看上传数据处理汇总报告，了解突出显示的属性、值和允许的最大阈值。
- 对数值进行四舍五入以匹配阈值中指定的最大允许小数位数。
- 更新值后，重新提交文件。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GRZKQGN5J3PDK45P
