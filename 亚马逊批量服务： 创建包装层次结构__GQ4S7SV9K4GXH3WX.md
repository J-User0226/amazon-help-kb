---
title: 亚马逊批量服务： 创建包装层次结构
doc_id: GQ4S7SV9K4GXH3WX
source: https://sellercentral.amazon.com/help/hub/reference/external/GQ4S7SV9K4GXH3WX
language: zh-CN
fetched_at: 2026-10-30 14:15:03
---

# 亚马逊批量服务： 创建包装层次结构

## 创建包装层次结构
在创建包装层次结构前，确定您希望采用两种或多种包装配置（单件商品、大包装或托拍装）进行销售或计划进行销售的相关商品。例如，假设您销售一盒 10 支的钢笔（单件装）以及一箱 10 盒的商品（大包装），或者您销售一盒 10 支的钢笔（单件装）且希望销售一托拍 100 盒的托拍装商品，则可以使用包装层次结构关联这些配置。请注意，销售托拍不是必须使用的。您只需提供两种或多种包装配置，即可使用包装层次结构。

然后，您可以按照这 4 个步骤来创建包装层次结构。

## 步骤 1： 下载模板
1. 在卖家平台中，前往[下载商品电子表格](https://sellercentral.amazon.com/product-search/bulk/generate/add-product)。（【目录】 > 【添加商品】 > [下载空白模板](https://sellercentral.amazon.com/listing/download) > [下载商品表格](https://sellercentral.amazon.com/product-search/bulk/generate/add-product)）
2. 下载模板：
  1. 选择正确的商品类型。您可以选择多种商品类型。
  2. 选择商城。
  3. 点击【生成电子表格】。

该模板包含多个选项卡： “说明”“图片”“示例”“数据定义”“有效值”，用于帮助您填写该模板。您需要在“Template”工作表中输入信息。

## 第 2 步： 填写模板
填写模板时，有两种可能的场景：
- **商品已发布在亚马逊商城**： 例如，钢笔的单件装和大包装均已在亚马逊商城发布。在这种情况下，您只需在模板中填写信息即可创建包装层次结构：
  1. 填写 【item_sku】 和 【external_product_id】。同一商品的每个配置（单件装、大包装、托拍装）均应具有不同的外部商品编码（例如，GTIN 或 UPC 等）。
  2. 按照下方的模板变体部分中的【填写包装层次结构属性】所示，填写包装层次结构属性。
  3. 将 update_delete 属性设置为 【Update】。

- **商品未在亚马逊商城发布**： 例如，钢笔的单件装已发布在亚马逊商城，但未发布托拍装。在这种情况下，除了提供信息以创建包装层次结构之外，您还需要提供信息以创建相应的托拍装的商品信息：
  1. 在第一部分，需要至少填写所有必填字段，包括 【item_sku】 和 【external_product_id】。同一商品的每个配置（单件装、大包装、托拍装）均应具有不同的外部商品编码（例如，GTIN 或 UPC）。
  2. 按照下方变体部分中的【填写包装层次结构属性】所示，填写包装层次结构属性。
  3. 将 update_delete 属性设置为 【Update】。

## 填写包装层次结构属性
下表概述了如何在卖家平台模板中为单件装商品、原厂包装商品和托拍装商品填写包装层次结构属性：

关系类型 包装级别 package_contains_quantity package_contains_identifier
**对于单件装**

unit

**对于大包装** package_contains case 该大包装商品中包含的卖家 SKU 的数量 大包装包含的卖家 SKU
**对于托拍装** package_contains pallet 该托拍装商品包含的卖家 SKU 的数量 托拍装包含的卖家 SKU
【示例：】

关系类型 包装级别 package_contains_quantity package_contains_identifier
**包含 5 件 Unit_SKU 的 Case_SKU** package_contains case 5 Unit_SKU
**包含 10 个 Case2_SKU 的 Case1_SKU** package_contains case 10 Case2_SKU
**包含 15 件 Unit_SKU 的 Pallet_SKU** package_contains pallet 15 Unit_SKU
**包含 10 个 Case_SKU 的 Pallet_SKU** package_contains pallet 10 Case_SKU

## 第 3 步： 上传模板
1. 在卖家平台上，前往【目录】 > 【添加商品】 > 【上传文件】。
2. 在第 3 步中上传已完成的模板。

## 第 4 步： 在处理报告中确认
上传模板后，请前往【目录】 > 【添加商品】 > 【检查上传状态】下载处理报告。检查并更正处理报告中的任何错误。与包装层次结构相关的错误消息显示在【错误消息】部分。如果没有错误，则表示已成功创建包装层次结构。

**注意： **可能需要一些时间才能将状态更改为“上传状态完成”。

## 常见问题
#### 1. 什么是包装层次结构？
包装层次结构是[亚马逊批量销售服务](https://sellercentral.amazon.com/gp/help/external/GXNDQS697S3JVFK6)计划的核心。通过包装层次结构关联同一商品的多个包装配置后，您即可使用增强的功能，改善卖家和买家体验。层次结构可以由单件装、大包装和托拍装组成，定义如下：
- 单件装： 商品的最小可售包装，例如，一“盒”钢笔（含 10 支）。
- 大包装： 包含多件商品的包装，例如，含 10“盒”商品的“大包装”。
- 托拍装： 单件装商品或大包装商品堆叠在木质或塑料框架上，便于运输和储存。例如，含 100 件“大包装”的“托拍装”。

同一商品的不同包装配置（单件装、大包装、托拍装）可以通过多层父子关系的包装层次结构来表示。以下是最常见的包装层次结构类型：

**父** **子**
包含多个单件装商品的大包装 大包装 单件装
大包装中包含单件装商品
包含多个单件装商品的托拍装 托拍装 单件装
托拍装中包含单件装商品
托拍装中包含多个大包装商品，且每个大包装中包含多个单件装商品

托拍装

大包装

大包装

单件装

托拍装中包含大包装商品，且大包装中包含单件装商品

还可以使用许多其他层次结构，例如：
- 1 号大包装包含 2 号大包装商品，而 2 号大包装中包含单件装商品
- 托拍装包含 1 号大包装商品，1 号大包装包含 2 号大包装商品，而 2 号大包装包含单件装商品
- 1 号大包装包含 10 件单件装商品，而 2 号大包装包含 20 件单件装商品

#### 2. 包装层次结构与变体之间有什么区别？
包装层次结构与变体关系不同。[变体](https://sellercentral.amazon.com/gp/help/external/8831)是指在尺寸、颜色和风格等方面相互关联的一组商品。在包装层次结构中，不同的包装配置（单件装/大包装/托拍装）通过既定层次结构相互关联。一些旨在改善卖家和买家体验的功能（包括作为亚马逊批量销售服务计划的一部分所推出的销售佣金折扣），适用于使用包装层次结构关联的商品，但不适用于变体。包装层次结构和变体关系可以并存，即：同一商品可以既属于某一变体关系，又属于某一包装层次结构。

变体 包装层次结构

父

绿色商品 蓝色商品 黄色商品
托拍装中包含大包装商品，且大包装中包含单件装商品

#### 3. 我可以利用卖家平台上的哪些机制来创建或更改包装层次结构？
可针对以下情况创建包装层次结构：
- 为已发布在亚马逊商城的商品创建，或
- 在发布新商品时创建

目前，您可以使用卖家平台上的模板创建包装层次结构。今后将会推出对基于 Web 的界面和 API 集成的支持。

#### 4. 什么是用于创建包装层次结构的新属性？
用于启用包装层次结构的三个新属性，这些属性已加入现有卖家平台模板：
- Package level： 指明商品为单件装商品、大包装商品或者是托拍装商品
- Package contains identifier： 指明该包装中所含商品的 SKU。如果“package level”为“unit”，则此字段留空。
- Package contains quantity： 指明该包装中所含的 SKU 数量。如果“package level”为“unit”，则此字段留空。

例如：
大包装中含 10 件单件装商品
大包装对应的卖家 SKU： Case_SKU

单件装对应的卖家 SKU： Unit_SKU

**对于大包装**：
- Package level = case
- Package contains identifier = Unit_SKU
- Package contains quantity = 10

**对于单件装**：
- Package level = unit
- Package contains identifier = *留空*
- Package contains quantity = *留空*

托拍装包含 5 个大包装商品，且每个大包装包含 20 件单件装商品
托拍装对应的卖家 SKU： Pallet_SKU

大包装对应的卖家 SKU： Case_SKU

单件装对应的卖家 SKU： Unit_SKU

**对于托拍装**：
- Package level = pallet
- Package contains identifier = Case_SKU
- Package contains quantity = 5

**对于大包装**：
- Package level = case
- Package contains identifier = Unit_SKU
- Package contains quantity = 20

**对于单件装**：
- Package level = unit
- Package contains identifier = *留空*
- Package contains quantity = *留空*

#### 5. 如果我在提交模板时输入了错误的属性，我该如何更改包装层次结构属性？
如果您已经创建了包装层次结构并且想要更改任何包装层次结构属性，请按照以下步骤填写模板：
1. 填写所有必填字段，包括 【item_sku】 和 【external_product_id】。
2. 填写所有包装层次结构属性，以反映所需的更改。
3. 将 【update_delete】 属性设置为 【Update】。

#### 6. 如何在包装层次结构中删除 ASIN？
删除包装层次结构中的 ASIN 将移除该 ASIN 与相应包装层次结构之间的关系。例如，如果存在一个托拍装 - 大包装 - 单件装的层次结构，且您删除大包装 ASIN，那么相关大包装 ASIN 将被移除。此外，与相关托拍装和相关单件装对应的该包装层次结构关系也会被移除。

要执行删除操作，请按照以下步骤填写模板：
1. 填写 【item_sku】 和 【external_product_id】。
2. 将 【update_delete】 属性设置为 【Delete】。

#### 7. 我在上传模板时收到了错误消息。这表示什么？
下表列出了您在创建包装层次结构时可能遇到的错误：

错误代码和消息 错误原因
**99010：** 该组的一个或多个必填列缺少值：[Relationship Type]、[package_level]、[package_contains_identifier]、[package_contains_quantity]。 当 【Relationship Type】 设置为“package_contains”，且 【package_level】 设置为“Case”或“pallet”时，【package_contains_identifier】 和 【package_contains_quantity】 字段为必填字段。
**99008**： “Relationship Type”字段中的值 (Variation) 与“package_contains_identifier”字段中的值冲突。 仅当 【Relationship type】 的值为 【package_contains】 时，【package_contains_identifier】 属性才能有填充值。
**99008**： “Relationship Type”字段中的值 (package_contains) 与“package_level”字段中的值 (unit) 冲突。 如果 【package_level】 的值为“unit”，那么 【package_contains_identifier】 应留空。
**99008：** “Relationship Type”字段中的值 (Variation) 与“package_level”字段中的值 (case/unit) 冲突。 仅当 【Relationship type】 的值为 【package_contains】 时，【package_contains_identifier】 属性才能有填充值。
**990101**： 父 SKU ${sku} 与子 SKU ${child_id} 的 ${relationship_type} 关系被拒绝，原因是父 (${duplicate_gtins}) 上的一个或多个 GTIN 值与子 (SKU：${duplicate_gtin_child_id}) 的 GTIN 值相同。 层次结构中的每个 SKU 都必须具有唯一的外部商品编码（例如，GTIN 或 UPC）。
**990100**： 我们检测到“package_contains_identifier”属性可能存在错误。如果您看到与“package_contains_identifier”相关的其他错误或警告，请更正错误并重新提交。否则，您的请求可能仍在处理中，此错误将自行解决。 如果没有与 【package_contains_identifier】 相关的其他错误或警告消息，则此错误将自行关闭。否则，请修复相关错误或警告。

## 其他资源
[亚马逊批量销售服务](https://sellercentral.amazon.com/gp/help/external/GXNDQS697S3JVFK6)

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GQ4S7SV9K4GXH3WX
