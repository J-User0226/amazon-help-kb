---
title: 错误 100720
doc_id: G7MRMGTC84QYT5JS
source: https://sellercentral.amazon.com/help/hub/reference/external/G7MRMGTC84QYT5JS
language: zh-CN
fetched_at: 2026-10-30 13:33:04
---

# 错误 100720

## 错误消息
商城 ${marketplace_id} 中为属性 ${attribute_list} 提供的语言数据无效。

## 导致错误 100720 的原因
出现此错误的原因如下：
- 您提交的商品数据中的语言值在目标商城不受支持（例如，在美国商城中为需要英文的属性提交日语文本）。
- 您要更新的属性需要特定语言的信息，但提供的语言代码与商城可接受的语言代码不匹配。
- 您为属性提供了翻译内容，而使用的语言在特定商城未启用或无法识别。
- 商城中必填属性的语言数据格式不正确或不完整。

## 解决错误 100720
要解决此错误，请按照以下步骤操作：
1. 查看错误消息以确定导致验证失败的商城 (${marketplace_id}) 和具体属性 (${attribute_list})，并查看此商城的语言要求。
2. 确保指定属性中的所有文本都使用的是目标商城可接受的主要语言（例如 amazon.com 商城使用英语，amazon.de 商城使用德语，amazon.co.jp 商城使用日语）
3. 所有商品属性（例如商品名称、要点和描述）都必须与您的商品发布语言匹配。
4. 对于多个商城，请确保为每个商城提供的语言数据都正确。
5. 更正指定属性中所有与语言相关的问题后，重新提交您的商品信息。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/G7MRMGTC84QYT5JS
