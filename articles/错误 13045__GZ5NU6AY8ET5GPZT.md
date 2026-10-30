---
title: 错误 13045
doc_id: GZ5NU6AY8ET5GPZT
source: https://sellercentral.amazon.com/help/hub/reference/external/GZ5NU6AY8ET5GPZT
language: zh-CN
fetched_at: 2026-10-30 14:22:32
---

# 错误 13045

## 错误消息
“is_originating_currency”和“currency”（“list_price”的关联字段）的值必须与亚马逊目录中相应 ASIN 的信息相符。请进行必要的更改并重新提交。

## 导致错误 13045 的原因
导致此错误的原因如下：
- 目录货币不一致： 您在“is_originating_currency”“list_price”或任何“currency”字段中提交的货币代码与已在我们目录中为该 ASIN 注册的货币不同。例如，在“is_originating_currency”中提交了“USD”，但根据目录记录，该 ASIN 已将“CAD”指定为加拿大商城的原始货币。
- 字段间冲突： “is_originating_currency”和“currency”字段均已提交，但彼此不一致。
- 货币代码无效或无法识别： 您提交的货币代码无法用于指定商城或 ASIN，或者使用的代码格式不正确。例如，使用“US”而非“USD”，或者使用“EURO”而非“EUR”。

## 解决错误 13045
要解决此错误，请按照以下步骤操作：
1. 验证在亚马逊目录中为 ASIN 注册的货币值，并确保“is_originating_currency”和“currency”与目录记录完全一致。
2. 更新您的上传数据或提交内容，以便“list_price”属性中的“is_originating_currency”和“currency”字段与亚马逊为该 ASIN 记录的当前货币信息完全一致。这两个字段都必须使用正确的 ISO 4217 三字母货币代码，例如“USD”“EUR”“GBP”“CAD”以及“JPY”。
3. 更新正确的货币值后，请重新提交上传数据文件。
4. 让系统有时间处理更新后的提交。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GZ5NU6AY8ET5GPZT
