---
title: "错误 6000： ValueName 未达到最少字符限制"
doc_id: G31851
source: https://sellercentral.amazon.com/help/hub/reference/external/G31851
language: zh-CN
fetched_at: 2026-10-30T13:16:07
---

# 错误 6000： ValueName 未达到最少字符限制

字段 *FieldName* 中的数值 *ValueName* 所含的字符数少于允许的最少字符数 (*MinimumCharacters*)。

如果您提供的数值的字符数未达到所要求的最少字符数，则会发生此错误。例如，UPC 值应包含 12 个字符。出现该错误的原因有多种：

- 您提供的 ProductIDType 与您为 StandardProductID 输入的数值的类型不同。例如，您输入了一个要求 12 位数的 UPC 值，但实际应该输入要求有 13 位数的 EAN 编号。

- 您的值以一个或多个零开头，Excel 在您导出数据前删除了这些零。例如，您的 OrderID 以“058-”开头，但 Excel 将其更改为以“58-”开头。

要更正此错误，请按照该字段的数据定义中的要求输入正确数量的字符，然后重新提交此数据。

如果使用 Excel 创建数据文件，可能需要将该字段所在列的格式从数值更改为文本。这样可以防止 Excel 更改数据的格式。为此，请执行以下操作：

- 在 Excel 中选中此列。

- 从【格式】菜单中选择【单元格】。

- 从【类别】菜单框中选择【文本】。

- 点击【确定】。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/G31851
