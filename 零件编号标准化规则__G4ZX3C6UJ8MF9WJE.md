---
title: 零件编号标准化规则
doc_id: G4ZX3C6UJ8MF9WJE
source: https://sellercentral.amazon.com/help/hub/reference/external/G4ZX3C6UJ8MF9WJE
language: zh-CN
fetched_at: 2026-10-30 13:18:12
---

# 零件编号标准化规则

了解我们如何在匹配 ACES 文件和目录数据中的零件编号之前，对其进行标准化处理。

在匹配之前，我们对目录中的 ASIN 和 ACES 提交内容进行以下转换。**这些步骤按顺序应用。** 这意味着连字符、斜杠、点和其他特殊字符将被完全删除。

**步骤** **转换** **示例**
1 取消转义 HTML 实体 &amp; → &
2 转换为大写 abc123 → ABC123
3 删除除字母、数字、逗号、分号以外的所有字符 ABC-123 → ABC123, Part/456 → Part456
4 用空格替换逗号和分号 A;B,C → A B C
5 删除文本开头和空格后的前导零 00123 → 123
6 去除空格 ABC → ABC

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/G4ZX3C6UJ8MF9WJE
