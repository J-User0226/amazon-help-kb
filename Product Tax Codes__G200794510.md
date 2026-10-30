---
title: Product Tax Codes
doc_id: G200794510
source: https://sellercentral.amazon.com/help/hub/reference/external/G200794510
language: zh-CN
fetched_at: 2026-10-30 12:36:46
---

# Product Tax Codes

**重要： **本页信息不构成税务、法律或其他专业建议，也不得用作此类用途。如有疑问，请咨询您的专业顾问。

税务计算服务需要同时配置[商品税务代码](https://sellercentral.amazon.com/tax/nexus/settings/ptc)和[管辖设置](https://sellercentral.amazon.com/tax/nexus/settings)，才能开始计算。

商品可征税性规则因商品税务代码而异，且与特定司法辖区相关，如[亚马逊商品税务代码清单](https://sellercentral.amazon.com/tax/nexus/settings/ptc)中所述。可在商品级别或默认级别分配商品税务代码。

如果没有在默认级别或商品级别分配商品税务代码，则计算服务会使用“始终不纳税”商品税务代码 A_GEN_NOTAX 对交易中的商品按不纳税进行计算，得到 0% 的计算结果。

**默认级别**： 默认商品税务代码在[税务设置](https://sellercentral.amazon.com/tax/nexus/settings)中设置，用于将一个商品税务代码分配给多个商品，这些商品尚未在特定商品级别分配商品税务代码。如果您使用[自定义税率](https://sellercentral.amazon.com/gp/help/external/G202102080)，您的商品税务代码规则和费率将替换为您的自定义税率。加拿大商城不支持自定义费率。

要查看或编辑默认商品税务代码，请执行以下操作：

1. 在卖家平台中，前往【设置】。
2. 点击【税务设置】。
3. 在【税务计算规则】下，使用【默认商品税务代码】旁边的下拉菜单。
4. 选择您的【默认商品税务代码】
  - 使用下拉菜单旁边的[查看商品税务代码链接](https://sellercentral.amazon.com/tax/nexus/settings/ptc)，查看完整的商品税务代码列表以及每个税务代码的相关规则
  - 商品税务代码不支持特殊字符（例如“&”“"”“'”“<”“>”“/”“|”“;”）和空格。仅使用字母数字字符（A-Z、0-9）和下划线 (_)。

5. 阅读【税费计算方法】和【服务条款】，并选中【确认】框。
6. 点击【保存设置】。

**商品级别**： 商品级别商品税务代码在商品库存页面中设置，用于将特定商品税务代码指定给特定商品。商品级别商品税务代码的使用优先级高于默认商品税务代码。此外，如果您使用[自定义税率](https://sellercentral.amazon.com/gp/help/external/G202102080)，您的商品税务代码规则和费率将替换为您的自定义税率。加拿大商城不支持自定义费率。

要查看或编辑商品级别的商品税务代码，请执行以下操作：

1. 前往【管理库存】
2. 点击与单个商品对应的【编辑】
3. 随后您将转至【编辑商品信息】页面
4. 在【商品选项卡】中，找到“税务代码”字段
5. 点击该字段，并从下拉列表中选择【商品级别商品税务代码】
6. 点击【保存并完成】

以下工具可用于协助更新单件商品的详情页面：

- 要批量编辑多个商品，请使用[库存文件上传](https://sellercentral.amazon.com/hz/inventory/addproducts)。
- 要添加一件新商品，请使用[添加新商品](https://sellercentral.amazon.com/productsearch)工具。
- 商品税务代码不支持特殊字符（例如“&”“"”“'”“<”“>”“/”“|”“;”）和空格。仅使用字母数字字符（A-Z、0-9）和下划线 (_)。

## How a Product Tax Code (PTC) is determined at the time of tax calculation
如果同时在卖家定义的默认级别和商品级别分配了商品税务代码，亚马逊将会使用商品级别税务代码。

如果只在默认级别而未在商品级别分配商品税务代码，亚马逊将会使用卖家定义的默认商品税务代码。

如果未在商品级别或默认级别分配商品税务代码，亚马逊将使用非应税商品税务代码 [A_GEN_NOTAX](https://sellercentral.amazon.com/tax/nexus/settings/ptc/general#A_GEN_NOTAX) 进行计算。

**注意： **自定义税率（如配置）将会覆盖商品税务代码的可征税性规则，A_GEN_NOTAX 除外。要了解更多信息，请参阅[自定义税率](https://sellercentral.amazon.com/gp/help/external/G202102080)。加拿大商城不支持自定义费率。

税务计算设置更新通常会在 15~20 分钟内生效，且对订单没有追溯力。如果您发现税务计算结果存在问题，请检查您的设置（税务设置和商品级别设置）和库存文件上传是否存在错误（如果您使用的是库存文件上传）。如果计算问题仍然存在，请联系销售伙伴支持。

**注意： **亚马逊的卖家助手可以通过此主题提供帮助。对于大多数语言设置，卖家助手还可以直接将您转接至销售伙伴支持。

除了计算、代缴和申报您义务范围内的所有税费外，您还应负责确定自己的纳税义务，无论您是否参与亚马逊的税务计算服务。有关更多信息，请参阅我们的[税务政策](https://sellercentral.amazon.com/gp/help/external/G200405820)。

## Related Pages
[设置税务计算服务](https://sellercentral.amazon.com/gp/help/external/201706700)

[税务计算服务](https://sellercentral.amazon.com/gp/help/external/200787660)

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/G200794510
