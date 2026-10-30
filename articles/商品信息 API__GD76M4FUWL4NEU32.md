---
title: 商品信息 API
doc_id: GD76M4FUWL4NEU32
source: https://sellercentral.amazon.com/help/hub/reference/external/GD76M4FUWL4NEU32
language: zh-CN
fetched_at: 2026-10-30 15:25:34
---

# 商品信息 API

商品信息 API（应用程序编程接口）是一套全新的现代化[销售伙伴 API](https://developer-docs.amazon.com/sp-api/)，可供卖家和第三方（例如目录服务提供商）构建程序化集成，以便在亚马逊商城中选择商品信息。API 可提供构建模块功能，帮助卖家或集成商自动执行各种商品信息工作流程，从而有效地创建和管理商品信息。卖家可以使用这些 API 构建应用程序，从而减少目录管理工作量、减少商品信息错误并提高业务绩效。

## 自动发布商品
您可以通过以下选项自动发布商品：
- **直接集成：** 卖家负责开发集成（需要技术专业知识和技能来进行集成）
- **目录服务提供商：** 卖家可以利用亚马逊合作伙伴网络中的现有解决方案（可以在[销售伙伴应用商店](https://sellercentral.amazon.com/selling-partner-appstore)中下载。）

这两种备选方式均使用我们的 API 来检索和发布数据。借助目录服务提供商，您可以通过使用多个提供商来满足您的业务需求。

要求 选项一： 直接集成 选项二： 目录服务提供商
技术能力 能够使用 JSON* 格式编写代码 不需要
与第三方合作 否 是
额外费用 否 是
维护 API 渠道 需要 目录服务提供商提供支持（基于目录服务提供商的服务包）
内部资源 是 大部分工作由目录服务提供商承担
跨多个渠道集中数据和联合 否 是

## 构建和管理商品信息工作流程
我们为卖家提供了[构建商品信息管理工作流程指南](https://developer-docs.amazon.com/sp-api/docs/building-listings-management-workflows-guide#configuring-variation-families)。该指南概括介绍了通过与商品信息 API 集成来构建一流的商品信息创建和管理工作流程的步骤。遵循建议的步骤，卖家能够在创建和管理商品信息时尽可能减少冲突。本指南介绍了有关单个 API 操作和案例的详细信息。相关定义见下文。

**商品信息 API 提供的功能**

我们提供以下 API 和通知，用于进行编程集成。

业务流程 API 名称和内容 案例 案例指南链接
商品信息 商品类型定义 API 搜索和检索商品类型定义。 [https://developer-docs.amazon.com/sp-api/docs/product-type-api-use-case-guide](https://developer-docs.amazon.com/sp-api/docs/product-type-api-use-case-guide)
上架商品 API 创建、编辑和删除商品信息 (SKU)，包括图片 [https://developer-docs.amazon.com/sp-api/docs/listings-items-api-v2021-08-01-use-case-guide](https://developer-docs.amazon.com/sp-api/docs/listings-items-api-v2021-08-01-use-case-guide)
目录商品 API 在我们目录中检索商品信息 [https://developer-docs.amazon.com/sp-api/docs/catalog-items-api-v2020-12-01-use-case-guide](https://developer-docs.amazon.com/sp-api/docs/catalog-items-api-v2020-12-01-use-case-guide)
商品信息限制 API 提供有关亚马逊目录商品的商品信息限制的详细信息 [https://developer-docs.amazon.com/sp-api/docs/listings-restrictions-api-v2021-08-01-use-case-guide](https://developer-docs.amazon.com/sp-api/docs/listings-restrictions-api-v2021-08-01-use-case-guide)
通知 通知 API 包括商品状态的变化 [https://developer-docs.amazon.com/sp-api/docs/notifications-api-v1-use-case-guide](https://developer-docs.amazon.com/sp-api/docs/notifications-api-v1-use-case-guide)

## 商品类型定义 API
这是一个基础 API，允许卖家搜索和检索最新的商品类型定义。商品类型定义描述了亚马逊目录商品的属性和数据要求。这些架构表示的格式与上架商品 API、目录商品 API 和 JSON_LISTINGS_FEED 使用的是同一格式。

**主要特性**

- 能够根据地理区域商城和关键词搜索可用的商品类型
- 能够检索特定卖家、商品类型和地理区域商城的商品类型定义和相关架构
- 能够检索以下架构版本：
  - LATEST
  - RELEASE_CANDIDATE（提供商品类型架构的预发布版本。）

此版本通常包含即将推出的更改，以便让您提前做好准备。

- 能够检索以下方面的架构要求：
  - LISTING（包含商品事实和销售条款的要求。）
  - LISTING_OFFER_ONLY（仅包含销售条款的要求。）
  - LISTING_PRODUCT_ONLY（仅包含商品事实的要求。）

- 能够通过架构检索仅必填和有条件必填属性，或者检索可选和必填属性
- 能够在适用的情况下有效显示所有可用属性值（属性值选择列表）

## 上架商品 API
此 API 可与上述商品类型定义 API 配合使用，允许卖家创建、编辑和删除商品信息 (SKU)，包括商品详情（如商品名称和要点）以及销售条款（如商品价格、费用和库存）。使用商品类型定义 API 提供的架构，您可以验证是否满足数据要求，然后通过上架商品 API 提交数据。

**主要特性**

- 能够创建新的商品信息，全面更新现有商品信息
- 能够创建仅报价商品信息
- 能够提交纯商品属性，以部分创建“非在售”商品信息，其中不包含报价属性，这些信息可以在稍后添加
- 能够为商品信息提交图片
- 能够更新和删除现有商品信息的一个或多个单个属性
- 能够删除现有商品信息
- 在提交后能够收到实时验证错误，例如缺少必需属性
- 能够通过本地化问题消息接收所有目录渠道问题的列表
- 能够检索卖家 SKU 的所有属性信息

## 目录商品 API
此 API 允许卖家搜索和检索亚马逊目录中有关商品 (ASIN) 的信息。此 API 可查询 ASIN 提供的信息。该信息等同于详情页面上显示的信息。

**主要特性**

- 能够指定需要检索有关 ASIN 的信息
  - 所有商品属性的列表（适用于在商品所属品牌中拥有[销售角色](https://sellercentral.amazon.com/help/hub/reference/GJ84K745AL3R5N3Q)[品牌代表或转销商]的卖家）
  - 外部商品编码，如 EAN、UPC 或 ISBN
  - 图片
  - 商品类型
  - 商品销售排名数据： 每个销售排名都包含分类名称、商品排名以及指向零售网站上的销售排名页面的链接。
  - 商品变体数据： 包含与此商品相关的商品 ASIN 的列表以及此商品是子商品还是父商品。
  - 卖家可用的商品数据： 包含商品补货信息、品牌信息和制造商信息。

- 能够使用商品编码列表搜索 ASIN，搜索关键词和检索匹配的 ASIN 列表
- 能够按品牌和细化分类检索 ASIN 列表

## 商品限制 API
商品限制 API 可让卖家检查在亚马逊目录中是否存在阻止商品信息创建的限制。如果商品受限，您可以采取其他步骤请求批准创建商品信息。如果不存在限制，您可以调用上架商品 API 创建仅报价商品信息。

**主要特性**

- 提供有关按 ASIN 识别的现有目录商品的商品信息限制（如果有）的详情
- 提供根据状况类型筛选相关限制的选项
- 支持通过一次调用检查多个地理区域商城中的商品信息限制
- 当需要批准时，此 API 将提示后续步骤链接，以便您可以申请亚马逊批准创建商品信息

## 通知 API
通知 API 可让卖家订阅各种通知，以便卖家能够近乎实时地收到相关事件的通知。

我们目前提供以下通知：
- **LISTINGS_ITEM_ISSUES_CHANGE 通知**： 只要与您拥有的特定 SKU 相关的问题发生变化，我们就会发送 LISTINGS_ITEM_ISSUES_CHANGE 通知。问题会指出上架商品存在问题，可能导致商品变为非在售状态，在搜索结果中禁止显示，或者有其他质量问题。此通知可触发通过上架商品获取 API 提取有关问题的所有信息。
- **PRODUCT_TYPE_DEFINITIONS_CHANGE 通知**： 亚马逊添加新商品类型时，或任何商品类型的架构定义有更新时，系统就会发送此通知。此通知可触发通过上述商品类型定义 API 刷新并获取最新的架构要求。

## JSON_Listings_Feed API
您可通过上述上架商品 API 一次更新单个商品。对于某些卖家和集成商而言，上传数据 API（批量）仍然是首选的集成方式。JSON_LISTINGS_FEED 可与商品类型定义 API 配合使用，并允许集成商使用与上架商品 API 所使用的数据格式相同的格式创建、编辑和删除亚马逊商城上架商品 (SKU)，但可以批量处理。上架商品数据可在上架商品 API 与 JSON_LISTINGS_FEED 上传数据类型之间通用，允许卖家使用最适合其商品信息工作流程的机制或组合。

## 分类和地理区域商城的可用性
商品信息 API 现在可用于所有分类： 全球所有地理区域商城的硬百货、软百货、消费品、图书和媒介类商品。您可以为任何上架商品提交库存、价格或报价更新，无论其商品类型如何。

## 直接集成
以下是与上架商品 API 直接集成的一些注意事项：
- 通过直接集成，开发工作将始终由内部员工完成。
- 数据直接从卖家传输至亚马逊。
  - 数据交换无中间商
  - 卖家拥有的任何数据源均可映射并用于 API 集成中。

- 不依赖于第三方。
  - 解决方案可根据卖家自己的业务需求进行定制。
  - 灵活地开发新功能，并快速集成到新的 API 发布中

- 直接集成可能需要更长的设置时间以及在构建功能方面进行前期投资。
- 集成需要由卖家维护和运作。

在较高级别开启直接集成的流程需要卖家组织内的技术团队执行以下步骤：
1. 注册开发者资料。
2. 创建所需的 AWS 资源和销售伙伴 API 应用程序。
3. 开发与各种 API 集成的功能。
4. 测试应用程序。
5. 发布和维护。

## 技术文件
以下是技术文件的实用链接列表：
- [销售伙伴 API 网站](https://developer-docs.amazon.com/sp-api/docs/what-is-the-selling-partner-api)
- [使用销售伙伴 API 的主要步骤](https://developer-docs.amazon.com/sp-api/docs/what-is-the-selling-partner-api)
- [商品类型定义 API](https://developer-docs.amazon.com/sp-api/docs/product-type-definitions-api-v2020-09-01-reference)
- [上架商品 API](https://developer-docs.amazon.com/sp-api/docs/listings-items-api-v2021-08-01-reference)
- [目录商品 API](https://developer-docs.amazon.com/sp-api/docs/catalog-items-api-v2020-12-01-reference)
- [商品信息限制 API](https://developer-docs.amazon.com/sp-api/docs/listings-restrictions-api-v2021-08-01-reference)
- [通知 API](https://developer-docs.amazon.com/sp-api/docs/notifications-api-v1-reference)
- [上传数据 API](https://developer-docs.amazon.com/sp-api/docs/feeds-api-v2021-06-30-reference)

有关开发者资料注册、新用户培训或 API 集成的技术问题，请前往[获取帮助和资源](https://developer.amazonservices.com/support)或使用卖家助手，然后点击【向开发者支持提交问题单】。

有关与目录提交相关的问题以及提交过程中遇到错误的支持问题，请前往[获取帮助和资源](https://developer.amazonservices.com/support)或使用卖家助手，然后点击【其他资源】。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GD76M4FUWL4NEU32
