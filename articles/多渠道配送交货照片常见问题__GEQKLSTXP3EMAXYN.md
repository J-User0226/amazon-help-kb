---
title: "多渠道配送交货照片常见问题"
doc_id: GEQKLSTXP3EMAXYN
source: https://sellercentral.amazon.com/help/hub/reference/external/GEQKLSTXP3EMAXYN
language: zh-CN
fetched_at: 2026-10-30T13:31:42
---

# 多渠道配送交货照片常见问题

**常见问题**

**什么是交货照片？**

对于 Amazon Logistics 交付的货件，我们会在最终投件地点提供交货照片作为交货证明。您可以通过 Swiship 追踪网站查看交货照片并将其提供给买家。

**如何向买家提供交货照片？**

您可以通过 Swiship 追踪网站（[链接](http://swiship.com/)）、卖家平台的多渠道配送订单 (MCF) 详情页面或调用 getFulfillmentOrder API 向买家提供交货照片。

买家输入邮政编码进行验证后，即可通过“查看交货照片”链接在 Swiship 上查看这些照片。多渠道配送会自动将其追踪编码对应的特定 Swiship 链接分享给买家。如果您选择不将买家的电子邮件地址分享给多渠道配送，您仍可通过在 Swiship 上输入追踪编码和邮政编码来访问该图片，然后直接将其传递给买家。

也可通过以下方式查看交货照片：依次前往“卖家平台 > 订单 > 管理订单页面”。在管理订单页面，搜索单个订单或点击需要交付证据的订单。点击“货件”选项卡，展开“配送活动详情”。 “查看交货照片”链接（如果有）将显示在“活动详情”列中。您还可以通过 getFulfillmentOrder API 获取照片，路径为：fulfillmentShipmentPackage > deliveryInformation > documentType： “DELIVERY_IMAGE”。 请遵循此教程（[链接](https://developer-docs.amazon.com/sp-api/docs/retrieve-proof-of-delivery)），完成提取交货照片的步骤。

**我能否查看所有订单的交货照片？**

只有使用 Amazon Logistics 作为最后一英里承运人的货件，我们才会提供交货照片。照片还需要符合我们的内部要求，可显示给买家（例如照片质量高且不包括人员）。

对于由承运人而非 Amazon Logistics 配送的货件，您可以直接联系承运人索要交付证据。对于 UPS/Fedex，请参阅本常见问题页面的“我该如何查看 UPS/Fedex 配送货件的交货照片”部分，获取更多指导。

**我如何自动将交货照片分享给买家？**

要直接将包裹交货照片分享给买家，我们建议您在创建订单时通过以下方式之一添加买家的电子邮件地址（如尚未添加）：

- 卖家平台“创建多渠道配送订单”页面 - 字段名称为“买家电子邮件地址”

- 卖家平台“多渠道配送批量创建订单”- 字段名称为“NotificationEmail”

- 配送出库 API - 通过 CreateFulfillmentOrderRequest 调用 notificationEmails

**如果没有交货照片，我能够要求赔偿？**

无论是否有交货照片，多渠道配送费用和订单中标记为由该承运人配送的商品均不符合赔偿要求。

**我该如何查看 UPS/Fedex 配送货件的照片？**

对于由 UPS 和 FedEx 等外部承运人配送的包裹，您可以通过承运人的追踪页面查看交货照片。要查看追踪信息，请在卖家平台的货件详情页面点击追踪编码，从而打开 Swiship 追踪页面。在此页面，点击 UPS 追踪编码链接（或将其复制粘贴到 [UPS 追踪页面](https://www.ups.com/track?loc=en_US&requester=ST/)）。如有交货照片，将显示“有交货照片”横幅。输入您货件的邮政编码，即可查看照片。对于 FedEx 货件，在 Swiship 页面复制追踪编码，然后在 [FedEx 追踪页面](https://www.fedex.com/en-us/tracking.html)搜索该编码，此时，若有照片的话，便会显示照片。

**注意： **并非所有配送服务都会提供照片。如果没有提供照片或您对交付证据存有疑问，请直接联系承运人寻求帮助。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GEQKLSTXP3EMAXYN
