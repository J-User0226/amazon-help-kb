---
title: "错误 6000： TimeValue 超出可接受范围"
doc_id: G32601
source: https://sellercentral.amazon.com/help/hub/reference/external/G32601
language: zh-CN
fetched_at: 2026-10-30T13:16:25
---

# 错误 6000： TimeValue 超出可接受范围

*TimeValue* 超出了 *time-type* 的可接受范围。

如果您提交的时间单位出现格式错误，则会发生此错误。时间点必须使用六位数值表示，且无分隔符。有效的时间范围为 000000 至 235959，不超过 24 小时制的时间范围。

对于 XML 上传数据，如果要提交的时间为晚上 11:59:59，则格式应为：

- <Time>235959</Time>

要更正此错误，请确保您的库存文件或上传数据 (XML) 的日期格式正确且在有效日期范围内，然后重新提交此库存文件或上传数据。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/G32601
