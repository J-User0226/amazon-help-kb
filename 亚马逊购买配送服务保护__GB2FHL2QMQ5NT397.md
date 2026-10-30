---
title: 亚马逊购买配送服务保护
doc_id: GB2FHL2QMQ5NT397
source: https://sellercentral.amazon.com/help/hub/reference/external/GB2FHL2QMQ5NT397
language: zh-CN
fetched_at: 2026-10-30 13:28:07
---

# 亚马逊购买配送服务保护

亚马逊购买配送服务有两种类型的保护： 索赔保护和准时送达率保护。

对于索赔保护： 如果满足以下所有条件，则亚马逊购买配送服务货件有资格针对“包裹未送达”索赔获得亚马逊商城交易保障和 SAFE-T 索赔保护：
1. 亚马逊就未收到包裹已向买家进行赔偿。
2. 货件标签是通过亚马逊购买配送服务购买的，是“索赔保护”配送服务。在购买前，“索赔保护”标记会显示在亚马逊购买配送服务用户界面中，在购买标签后，则会显示在订单详情页面的【货件标签购买】部分中。（请注意： 带有“延迟送达风险”的标签不符合保护的要求）。 **注意： **根据亚马逊对数百万货件的了解，我们非常确信“索赔保护”配送服务将会按时送达。“延迟送达风险”配送服务是指根据亚马逊的预计送达日期，该订单准时送达几率较低。

3. 订单已准时发货，将会考虑承运人首次扫描的时间，而不是您确认发货的时间。

如果满足上述所有条件，亚马逊将会为买家提供赔偿，并且买家提出的索赔不会计入您的订单缺陷率。

对于由您管理买家支持的订单，亚马逊将遵循亚马逊商城交易保障索赔流程。有关更多信息，请参阅[亚马逊商城交易保障索赔](https://sellercentral.amazon.com/help/hub/reference/G27951)。

对于亚马逊通过 Customer Service by Amazon (CSBA) 或卖家自配送 Prime 计划管理买家支持的情况，将会遵循 SAFE-T 索赔流程。要了解更多信息，请参阅 [Customer Service by Amazon (CSBA) 退款赔偿政策](https://sellercentral.amazon.com/help/hub/reference/G7KCD8BYQER79WWJ)和[卖家自配送 Prime 退款赔偿政策](https://sellercentral.amazon.com/help/hub/reference/G202109110)。

对于准时送达率保护： 如果您在亚马逊购买配送服务中购买的货件标签带有“准时送达率保护”标记，并且使用了自动备货时间和配送设置自动化，那么您的准时送达率不会受到延迟送达的负面影响。有关更多信息，请参阅[准时送达](https://sellercentral.amazon.com/help/hub/reference/G200847280)。

**注意： **目前，卖家平台和亚马逊公司 [Veeqo](http://go.amazonsellerservices.com/veeqo-otdr-launch) 上会显示“准时送达率保护”“索赔保护”和“延迟送达风险”标记。通过 API 或从多渠道集成商处购买“购买配送服务”标签时，将提供“索赔保护”标签，如果适用，还将提供“准时送达率保护”。带有“延迟送达风险”的标签将被筛选掉。但是，在某些情况下，即使带有“延迟送达风险”的标签没有准时送达率保护，您可能仍希望访问这些标签。在这种情况下，要通过 API 访问带有“延迟送达风险”的标签，请参阅以下说明。
目前，无法通过多渠道集成商访问带有“延迟送达风险”的标签，但亚马逊正在努力通过其他多渠道集成商启用此功能。

#### 要访问卖家平台或[亚马逊公司 Veeqo](http://go.amazonsellerservices.com/veeqo-otdr-launch) 上的带有“延迟送达风险”的标签（没有“准时送达率保护”）：
您无需执行任何操作，您已可以使用这些带有“准时送达率保护”“索赔保护”和“延迟送达风险”标记的货件标签。

#### 使用 API 访问带有“延迟送达风险”的货件标签（没有“准时送达率保护”）
要通过购买配送 API 访问没有“准时送达率保护”的带有“延迟送达风险”的标签，请参阅以下内容：
1. 使用您的卖家记号向 [buy-shipping-feedback-us@amazon.com](mailto:%20buy-shipping-feedback@amazon.com) 发送电子邮件请求（请参阅[此链接](https://sellercentral.amazon.com/sw/AccountInfo/MerchantToken)）。您的账户将在 72 小时内添加此功能。
2. **如果您使用[配送 V2 API](https://developer-docs.amazon.com/amazon-shipping/docs/shipping-api-v2-reference)**： 一旦我们允许您的账户购买带有“延迟送达风险”的标签，当您调用 [getRates](https://developer-docs.amazon.com/amazon-shipping/docs/shipping-api-v2-reference#getrates) API（作为 [GetRatesResult](https://developer-docs.amazon.com/amazon-shipping/docs/shipping-api-v2-reference#getratesresult) 的一部分）时，该 API 将同时返回符合要求和不符合要求的配送服务报价。“延迟送达风险”配送服务报价将作为 [GetRatesResult](https://developer-docs.amazon.com/amazon-shipping/docs/shipping-api-v2-reference#getratesresult) 的符合要求的服务的一部分可供购买，且 [ExcludedBenefits](https://developer-docs.amazon.com/amazon-shipping/docs/shipping-api-v2-reference#excludedbenefits) 清单将包含 CLAIMS_PROTECTED 和 OTDR_PROTECTED 权益，原因代码清单中将包含 LATE_DELIVERY_RISK。
3. **如果您使用[卖家自配送 API](https://developer-docs.amazon.com/sp-api/docs/merchant-fulfillment-api-v0-reference)**： 一旦我们允许您的账户购买带有“延迟送达风险”的标签，当您使用 [getEligibleShipmentServices](https://developer-docs.amazon.com/sp-api/docs/merchant-fulfillment-api-v0-reference#geteligibleshipmentservices) 操作时，[GetEligibleShipmentServicesResponse](https://developer-docs.amazon.com/sp-api/docs/merchant-fulfillment-api-v0-reference#geteligibleshipmentservicesresponse) 下的输出中将包含符合要求和不符合要求的配送方式。现在，您可以在符合要求的配送方式下找到带有“延迟送达风险”的标签（原因代码中带有“LATE_DELIVERY_RISK”标签，在 [ExcludedBenefits](https://developer-docs.amazon.com/sp-api/docs/merchant-fulfillment-api-v0-reference#excludedbenefit) 中会包含 CLAIMS_PROTECTED 和 OTDR_PROTECTEED 标签）。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GB2FHL2QMQ5NT397
