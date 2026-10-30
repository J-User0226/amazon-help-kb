---
title: 错误 99002
doc_id: GZ87UBX9G6NCRRRQ
source: https://sellercentral.amazon.com/help/hub/reference/external/GZ87UBX9G6NCRRRQ
language: zh-CN
fetched_at: 2026-10-30 14:23:00
---

# 错误 99002

## 错误消息
不允许 ${generic_parameter} 使用科学记数法中的 EAN/UPC 值。

## 导致错误 99002 的原因
导致此错误的原因如下：
- 值是从电子表格导入的，电子表格会自动将长数字转换为科学计数。
- 使用科学记数格式（例如 1.23E+12）手动输入条形码编号。

## 解决错误 99002
要解决此错误，请按照以下步骤操作：
1. 将 EAN/UPC 转换为标准数字格式，并确保它们存储为字符串/varchar，以保留前导零。
2. 在导入或输入数据之前，请在电子表格中将 EAN/UPC 列的格式设置为“文本”。
3. 将科学记数值复制到文本编辑器中，将其转换为完整数字形式，然后再重新粘贴。
4. 更新属性值后，请重新提交上传数据文件。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GZ87UBX9G6NCRRRQ
