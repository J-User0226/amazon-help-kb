---
title: "创建和编辑亚马逊 Haul 商品信息"
doc_id: GN8NWNGP9JUA763Y
source: https://sellercentral.amazon.com/help/hub/reference/external/GN8NWNGP9JUA763Y
language: zh-CN
fetched_at: 2026-10-30T13:45:16
---

# 创建和编辑亚马逊 Haul 商品信息

要创建和编辑亚马逊 Haul 商品信息，请使用卖家平台中的批量上传商品工具或商品信息 API。目前，您无法使用发布商品工具创建或编辑亚马逊 Haul 商品信息。

**重要： **目前，编辑亚马逊 Haul 商品信息中商品价格的唯一可接受方式是通过上传或亚马逊 Haul 支持的 API。如果您尝试通过其他系统编辑商品价格，将导致意外创建 Amazon.com 商品报价。Amazon.com 商品报价随后将被拒绝。

## 通过上传

要通过上传创建或编辑您的亚马逊 Haul 商品信息，请按照以下步骤操作：

- 从卖家平台的下拉菜单中选择【目录】，然后选择【添加商品】。

- 在【发布商品】页面上，点击【电子表格】，然后点击【下载空白模板】。

- 选择【亚马逊 Haul】 电子表格和所需商品类型。

- 填写必填信息以及任何其他可选信息，然后输入您的亚马逊 Haul 商品详情（例如商品价格）。

**注意： **您必须为亚马逊 Haul 商品使用不同的 SKU。如果您重复使用 Amazon.com 商品的 SKU（在售或非在售），您的亚马逊 Haul 商品将被停售。我们建议您使用一个前缀（例如 Haul-SKU），以便您在卖家平台中轻松识别商品。

- 检查您的商品信息是否符合[允许在亚马逊 Haul 中销售的商品](https://sellercentral.amazon.com/gp/help/external/GAK9UAJGQRN3Y87A)中列出的商品要求。请确保您输入了商品的尺寸和重量信息，且品牌名称为**无品牌**。如果商品价格高于亚马逊 Haul 价格限额，您将在模板中看到一条错误消息，指示您降低商品价格。有关亚马逊 Haul 商品信息政策的更多信息，请参阅模板的 【Haul 指南】选项卡。

**重要： **请务必时常查看[允许在亚马逊 Haul 中销售的商品](https://sellercentral.amazon.com/gp/help/external/GAK9UAJGQRN3Y87A)帮助页面，确认最新的价格限额。如果您使用的是先前下载的模板，则该信息可能已过时。

- 填写完模板后，请上传模板进行处理。如果您的某些商品在上传过程中失败，您可以从[电子表格上传状态](https://sellercentral.amazon.com/listing/status)页面下载处理一览，查看原因。

要查看商品详情，请前往[管理所有库存](https://sellercentral.amazon.com/myinventory/inventory?fulfilledBy=all&page=1&pageSize=10&sort=sales_desc&status=all&ref_=xx_invmgr_dnav_xx)。对于亚马逊 Haul 商品，Haul 标记将显示在【商品价格和运费】列中。

## 通过 API

要通过 API 创建或编辑您的亚马逊 Haul 商品信息，请按照以下步骤操作：

- 使用[商品类型定义 API](https://sellercentral.amazon.com/help/hub/reference/GD76M4FUWL4NEU32) 访问具有亚马逊 Haul 功能的 JSON 模式。

- 在 【sellerID】 参数中提供您的卖家编号，以确保亚马逊 Haul 功能可用。

- 使用[商品类型定义 API v2020-09-01](https://developer-docs.amazon.com/sp-api/docs/product-type-api-faq#do-product-type-definition-json-schemas-include-custom-vocabulary)，输入“BZR”作为 【Audience】 属性，以表明您打算在亚马逊 Haul 中发布您的商品报价。

- 使用 Listings Items API 或 JSON Listings Feed 构建并提交有效载荷。

- 在 【is_value_stores_item】 属性中输入“true”，以表明您的 ASIN 正在参与亚马逊 Haul。

- 继续输入您的商品信息，就像现在输入商品信息一样。请勿在您的有效载荷中输入外部分配的商品编码（例如 UPC）、卖家建议的 ASIN 或配送渠道属性。

有关更多信息，请参阅[使用销售伙伴 API 管理商品信息](https://developer-docs.amazon.com/sp-api/docs/manage-product-listings-guide)。

## 图片指南

亚马逊 Haul 的搜索体验变更可能会导致图片被裁剪。为获得最佳效果，请注意正方形图片每边最多可裁剪 13%，纵向图片最多可从图片底部裁剪 18%。

![](https://m.media-amazon.com/images/G/01/haul/sx/Crop_Picture_1.png)

![](https://m.media-amazon.com/images/G/01/haul/sx/Crop_Picture_2.png)

我们制定了图片的技术和内容要求，确保买家能够看到准确且有帮助的高品质图片。当您上传图片文件时，我们会对其进行检查，确认其符合亚马逊的要求。

如果您的图片不符合内容要求或违反了[销售政策和卖家行为准则](https://sellercentral.amazon.com/help/hub/reference/external/G1801)，我们可能会将其移除。如果您未遵循这些要求，我们可能会在搜索结果中禁止显示您的商品信息，直到您提供合规图片为止。在某些情况下，我们还可能会更改图片的位置或修改图片，以满足要求。与您的商品关联的所有图片都将显示在[图片管理器](https://sellercentral.amazon.com/imaging/manage)中。

图片必须符合[商品图片要求](https://sellercentral.amazon.com/help/hub/reference/external/G1881)中注明的要求。图片还必须符合下列要求。如果商品图片要求与下列要求发生冲突，则以下列要求为准。

- 至少提供一张生活风格的图片，最好作为首张图片。

- 如果可以的话，在图片中展示使用商品的人。对于某些商品，这可能仅为一个人。

- 使用真实的背景。

- 使用比例合适且真实可信的图片。

- 使用没有文本、不会分散买家注意力的背景。首张图片不能包含任何文本。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GN8NWNGP9JUA763Y
