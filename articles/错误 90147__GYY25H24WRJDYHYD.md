---
title: "错误 90147"
doc_id: GYY25H24WRJDYHYD
source: https://sellercentral.amazon.com/help/hub/reference/external/GYY25H24WRJDYHYD
language: zh-CN
fetched_at: 2026-10-30T14:21:39
---

# 错误 90147

## 错误消息

'${left_attribute_name}' 的值 '${left_attribute_value}' 未小于或等于 '${right_attribute_name}' 的值 '${right_attribute_value}'。

## 导致错误 90147 的原因

出现此错误的可能原因如下：

- 左侧属性值未小于右侧属性值（例如：cost_price 的值 126.1 未小于 list_price 的值 33.21）

- 在日期校验场景中，开始日期晚于或等于结束日期（例如：start_date“2024-04-01”晚于 end_date“2024-03-31”）

## 解决错误 90147

- 查阅上传数据处理汇总报告，找到突出显示的错误属性。

- 确保左侧属性值在数值上小于右侧属性值。

- 对于日期范围，核实开始日期是否早于结束日期（例如：start_date： 2024-01-01 必须早于 end_date： 2024-12-31）。

- 检查所有数量字段，确认最小值均小于或等于最大值。

- 更新属性值后，重新提交上传数据文件。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GYY25H24WRJDYHYD
