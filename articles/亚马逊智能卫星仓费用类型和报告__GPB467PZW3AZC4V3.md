---
title: "亚马逊智能卫星仓费用类型和报告"
doc_id: GPB467PZW3AZC4V3
source: https://sellercentral.amazon.com/help/hub/reference/external/GPB467PZW3AZC4V3
language: zh-CN
fetched_at: 2026-10-30T13:46:34
---

# 亚马逊智能卫星仓费用类型和报告

亚马逊智能卫星仓有三类费用：仓储费、处理费和运输费。

## 仓储费

我们会根据您的库存在我们的分拨中心占用的空间来收取亚马逊仓储和分拨服务月度仓储费。月度仓储费的计算方法是将适用的仓储费费率乘以储存的所有包装箱在当月使用的平均体积。

要查看适用的仓储费费率，请参阅[亚马逊仓储和分拨服务费用](https://sellercentral.amazon.com/gp/help/external/GAYG62Q3MPE6STFS)。该费用在每月 6 日收取。

**计算示例：**

- 每立方英尺的仓储费：$0.57

- 某一货件和 FNSKU 在一整月内的平均仓储体积： 100 立方英尺

仓储费的计算方式：$0.57 x 100 = $57

## 处理费

当我们的分拨中心收到您的库存时，我们将在入库时单独收取处理费，当补货订单成功送至我们的配送网络或其他销售渠道时，我们将在出库时再次收取处理费。

要查看处理费费率，请参阅[亚马逊仓储和分拨服务费用](https://sellercentral.amazon.com/gp/help/external/GAYG62Q3MPE6STFS)。

**计算示例：**

- 每个包装箱的处理费（分别在入库和出库时收取）：$1.40

- AWD 分拨中心收到的箱数： 25

- 针对补货订单配送的箱数： 10

入库时的处理费计算方式：$1.40 x 25 = $35

出库时的处理费计算方式为：$1.40 x 10 = $14

## 运输费

补货订单成功送至我们的配送网络或您的其他销售渠道时，将收取运输费。该费用的计算方法是将适用的运输费费率乘以作为补货订单运送至亚马逊物流的包装箱总体积（以立方英尺为单位）。要查看运输费费率，请参阅[亚马逊仓储和分拨服务费用](https://sellercentral.amazon.com/gp/help/external/GAYG62Q3MPE6STFS)。

**计算示例：**

- 每立方英尺的运输费：$1.40

- 补货订单中包装箱的总体积： 100 立方英尺

运输费的计算方式：$1.40 x 100 = $140

**注意： **对于从 AWD 向亚马逊物流的自动补货，不单独收取贴标费用。运往分拨中心的货件箱上粘贴的标签可用于自动补货。有关更多信息，请参阅[将货件运送至亚马逊仓储和分拨服务中心](https://sellercentral.amazon.com/gp/help/external/GTPL7PGKU7WUKJSW)。

## 费用报告

我们会分别为仓储费、处理费和运输费提供相应的月度报告：

- [月度仓储费报告](https://sellercentral.amazon.com/awd/fee/reporting)显示了每个 FNSKU 的仓储费明细。

- [月度处理费报告](https://sellercentral.amazon.com/awd/reports/fee?reportType=AwdProcessingFee)和[月度运输费报告](https://sellercentral.amazon.com/awd/reports/fee?reportType=AwdOutboundTransportationFee)会整理汇总一整月所有补货订单的处理费和运输费。自 2025 年 4 月 1 日起，月度处理费报告将分别提供入库处理费和出库处理费的详细信息。

- [月度多渠道分拨运输费报告](https://sellercentral.amazon.com/awd/reports/fee?reportType=AwdMcdTransportationFee)整理了整个月的多渠道分拨订单的运输费。

在每月 8 日之前，我们将更新上个月的费用报告。

您可以在[付款控制面板](https://sellercentral.amazon.com/payments/dashboard/index.html/ref=xx_payments_dnav_xx)中查看亚马逊智能卫星仓仓储费、处理费和运输费交易情况。下载并打开报告后，交易类型将显示为“服务费用”，商品详情将显示为“亚马逊智能卫星仓仓储费”“亚马逊智能卫星仓处理费”“亚马逊智能卫星仓运输费”或“亚马逊智能卫星仓多渠道分拨运输费”。

**费用指标报告（之前称为自动补货率报告）**： 亚马逊智能卫星仓费用指标报告提供关键费用指标的每日追踪信息，包括总历史供货天数、自动补货率和自定义功能使用标记。该报告于每周三生成，每份报告反映的是上一周的数据。

## 费用报告术语表

## 月度仓储费报告（自 2025 年 4 月起的费用报告）

| 列标题 | 描述 | 示例值 |
| --- | --- | --- |
| merchant_customer_id | 与您的卖家账户相关联的唯一编号。 | 80457449302 |
| inbound_purchase_order_id | 为您运送至仓储和分拨服务中心的货件所生成的货件追踪编号。 | 3LX3PGHW |
| inbound_carrier_type | 用于将库存入库至亚马逊仓储和分拨服务的承运人的名称。 | 合作承运人计划、亚马逊全球物流、SEND 或第三方 |
| asin | ASIN 由 10 个字母或数字组成，是用于识别商品的唯一编码。 | B07FZ8S74R |
| fnsku | 配送网络 SKU 是亚马逊物流为您的商品分配的唯一标识。 | X000A8GG1A |
| msku | 仓储和分拨服务的分拨中心编码。 | B1P5012BT7-8UPC |
| country_code | 分拨中心所在的国家/地区。 | 美国 |
| warehouse_id | 仓储和分拨服务的分拨中心编码。 | IUSL |
| monthly_average_utilized_volume | 某一入库订货单编号和 FNSKU 在一整月的包装箱平均体积。 | 102.56 |
| chargeable_volume | 用于收费的体积量。如果您使用亚马逊仓储和分拨服务预留仓储容量，并且使用的体积小于最低保证体积，则此数字将反映用于收费的最低保证体积。 | 102.56 |
| volume_units | 包装箱体积的计量单位，以立方英尺为单位。 | Cu_ft |
| fee_type | 仓储和分拨服务的费用类型。 | STORAGE_FEE |
| fee_amount | chargeable_volume 乘以 fee_rate 计算得出的费用金额。 | 49.22 |
| promotion_amount | 作为折扣提供的金额。 | 0 |
| tax_amount | 税费金额。 | 0 |
| total_charged_amount | 基于费用金额、促销金额和税费金额计算得出的收费总额。 | 30 |
| currency | 仓储费使用的货币单位。 | 美元 |
| fee_rate_type | 对 chargeable_volume 应用的费率类型。 | BASE_RATE、 STORAGE_RESERVATION_RATE、SMART_STORAGE_RATE、AMS_RATE |
| fee_rate | 用于计算费用的适用费率值。每种费用类型都有不同的值。 | 0.48 |
| fee_rate_units | 计费单位。 | $ PER_CUFT |
| myp_order_id | 付款控制面板上显示的订单编号，该编号映射到亚马逊仓储和分拨服务仓储费。 | 2025-02-A1ZEBA98JHW8LI |

## 处理费用报告（自 2025 年 4 月起的费用报告）

| 列标题 | 描述 | 示例值 |
| --- | --- | --- |
| merchant_customer_id | 与您的卖家账户相关联的唯一编号。 | 80457449302 |
| charge_type | 将要收取费用的入库或出库处理类型。 | 入库、出库 |
| inbound_carrier_type | 用于将库存入库至亚马逊仓储和分拨服务的承运人的名称。 | 合作承运人计划、亚马逊全球物流、SEND 或第三方 |
| purchase_order_id | 为亚马逊仓储和分拨服务入库或出库货件生成的采购订单编号。根据收费类型，系统将填充相应的订单编号。 | 3LX3PGHW |
| outbound_order_id | 在亚马逊仓储和分拨服务出库时创建的亚马逊订单编号。 | repl-53ca9d8b-1367-4063-bc6b-f985f9547015 |
| shipment_id | 为入库或出库订单中创建的每个货件生成的货件编号，用于追踪货件。 | 出库 - repl-ship-06e14427-d6d9-4874-b0c1-6bfa84034c35 入库 - STAR-TPWFTX3ZF5UXA |
| outbound_shipment_tracking_id | 对于出库订单，系统会生成货件追踪编码，用于在一个货件编号下追踪多个不同货件。 | FBA16YR3R2Z4 |
| transaction_date | 接收入库货件的日期或确认出库货件发货的日期。此日期决定了为交易选择的费率。 | MM/DD/YYYY |
| asin | ASIN 由 10 个字母或数字组成，是用于识别商品的唯一编码。 | B07FZ8S74R |
| fnsku | 配送网络 SKU 是亚马逊物流为您的商品分配的唯一标识。 | X000A8GG1A |
| msku | 卖家为某个 SKU 提供的唯一编码。 | B1P5012BT7-8UPC |
| warehouse_id | 提供仓储和分拨服务的分拨中心编号，货件在此入库或出库。 | IUSL |
| destination_code | 补货订单的销售渠道。“AFN”代表亚马逊物流渠道，“Non-AFN”代表亚马逊以外的地点。 | AFN 或 Non-AFN 入库费用类型留空 |
| month_of_charge | 收取处理费的月份。 | 5 月 |
| year_of_charge | 收取处理费的年份。 | 2025 |
| box_qty | 入库订单或出库订单中的总箱数。 | 15 |
| fee_type | 仓储和分拨服务的费用类型。 | PROCESSING_FEE |
| fee_rate | 用于计算费用的适用费率值。每种费用类型都有不同的值。 | 1.4 |
| fee_rate_units | 计费单位。 | $ PER_BOX |
| fee_rate_type | 适用于箱数的费率类型。 | BASE_RATE、STORAGE_RESERVATION_RATE |
| calculated_fee_amount | 总费用的计算方法是每个包装箱的单价乘以补货订单或入库订单中的总箱数。 | 21 |
| promotion_amount | 作为折扣提供的金额。 | 0 |
| tax_amount | 税费金额。 | 0 |
| charged_amount | 根据费用金额、促销金额和税费金额计算得出的收费金额。 | 21 |
| currency | 处理费使用的货币单位。 | 美元 |
| myp_order_id | 付款控制面板上显示的订单编号，该编号映射到亚马逊仓储和分拨服务处理费。 | repl-3bdf5127-f5c3-4551-a2a2-5b47f9b2c22f, IB_2025-04-02_STAR-TPWFTX3ZF5UXA |

## 运输费用报告（自 2025 年 4 月起的费用报告）

| 列标题 | 描述 | 示例值 |
| --- | --- | --- |
| merchant_customer_id | 与您的卖家账户相关联的唯一编号。 | 80457449302 |
| inbound_carrier_type | 用于将库存入库至亚马逊仓储和分拨服务的承运人的名称。 | 合作承运人计划、亚马逊全球物流、SEND 或第三方 |
| inbound_purchase_order_id | 为入库至亚马逊仓储和分拨服务的货件生成的采购订单编号。 | 3LX3PGHW |
| replenishment_order_id | 从仓储和分拨服务中心运往亚马逊物流的补货订单的唯一标识。每个订单可以含有多个订货单编号。 | repl-53ca9d8b-1367-4063-bc6b-f985f9547015 |
| shipment_id | 为补货订单中创建的每个货件生成的货件追踪编号。 | repl-ship-06e14427-d6d9-4874-b0c1-6bfa84034c35 |
| shipment_tracking_id | 为补货订单中创建的每个货件生成的唯一货件编号，用于追踪货件。 | FBA16YR3R2Z4 |
| transaction_date | 确认出库货件发货的日期。此日期决定了为交易选择的费率。 | MM/DD/YYYY |
| asin | ASIN 由 10 个字母或数字组成，是用于识别商品的唯一编码。 | B07FZ8S74R |
| fnsku | 配送网络 SKU 是亚马逊物流为您的商品分配的唯一标识。 | X000A8GG1A |
| msku | 卖家为某个 SKU 提供的唯一编码。 | B1P5012BT7-8UPC |
| outbound_purchase_order_id | 为从仓储和分拨服务中心运往亚马逊物流的货件生成的出库订货单编号。 | 3LX3PGHW |
| warehouse_id | 仓储和分拨服务的分拨中心编码。 | IUSL |
| destination_code | 补货订单的销售渠道。“AFN”代表亚马逊物流渠道，“Non-AFN”代表亚马逊以外的其他地点。 | AFN 或 Non-AFN |
| month_of_charge | 收取运输费的月份。 | 12 月 |
| year_of_charge | 收取运输费的年份。 | 2023 |
| length_per_box | 某一出库订货单编号和 FNSKU 的包装箱长度。 | 10.45 |
| width_per_box | 某一出库订货单编号和 FNSKU 的包装箱宽度。 | 29.89 |
| height_per_box | 某一出库订货单编号和 FNSKU 的包装箱高度。 | 30.34 |
| measurement_units | 包装箱尺寸的计量单位，以英寸为单位。 | IN |
| total_box_volume | 某一出库订货单编号和 FNSKU 的补货订单中的包装箱总体积。 | 54.84 |
| volume_units | 包装箱体积的计量单位，以立方英尺为单位。 | Cu_ft |
| box_qty | 补货订单中的总箱数。 | 10 |
| fee_type | 仓储和分拨服务的费用类型。 | TRANSPORTATION_FEE |
| fee_rate | 用于计算费用的适用费率值。每种费用类型都有不同的值。 | 1.4 |
| fee_rate_type | 对 chargeable_volume 应用的费率类型。 | BASE_RATE、STORAGE_RESERVATION_RATE、AMS_RATE |
| fee_rate_units | 计费单位。 | $ PER_CUFT |
| total_charged_amount | 总费用的计算方法是每个包装箱的单价乘以补货订单中的总箱数。 | 76.77 |
| promotion_amount | 作为折扣提供的金额。 | 1 |
| tax_amount | 税费金额。 | 0 |
| charged_amount | 根据费用金额、促销金额和税费金额计算得出的收费金额。 | 75.77 |
| currency | 运输费使用的货币单位。 | 美元 |
| myp_order_id | 付款控制面板上显示的订单编号，该编号映射到亚马逊仓储和分拨服务运输费。 | repl-3bdf5127-f5c3-4551-a2a2-5b47f9b2c22f |

## 亚马逊仓储和分拨服务费用指标报告（之前称为自动补货率报告）

| 列标题 | 描述 | 示例值 |
| --- | --- | --- |
| snapshotDate | 计算费用指标的日期。 | 9/20/2024 |
| asin | ASIN 由 10 个字母或数字组成，是用于识别商品的唯一编码。 | B07FZ8S74R |
| fnsku | 配送网络 SKU 是亚马逊物流为您的商品分配的唯一标识。 | X000A8GG1A |
| autoReplenishmentRatio Percentage | 自动补货率等于自动补货的货件数量除以发往亚马逊物流的货件总数。它包括最近 90 天内通过亚马逊仓储和分拨服务自动运送和手动运送的货件，以及直接运往亚马逊物流的货件。 | 70.42% |
| Combined Historical Days of Supply | 总历史供货天数是将亚马逊仓储和分拨服务与亚马逊物流中的日均库存量除以亚马逊物流的平均配送商品数量。我们分两个时间段评估此指标：最近 30 天（短期）和最近 90 天（长期），然后使用二者中较高的值。 | 98.10 天 |
| AR Max Limit Usage flag | 如果在最近 90 天内设置了自动补货的最大限制，则该标记将设置为 1。否则，它为 0。 | 1 或 0 |
| AR Min Limit Usage flag | 如果在最近 90 天内设置了自动补货的最低限制，则该标记将设置为 1。否则，它为 0。 | 1 或 0 |
| FBA LILF fee exempt | 指明在快照日期，是否免除亚马逊物流低库存水平费用。 | 是/否 |
| FBA SUS fee exempt | 指明在快照日期，是否免除亚马逊物流仓储利用率附加费。 | 是/否 |
| FBA AIS fee exempt | 指明在快照日期，是否免除亚马逊物流超龄库存附加费。 | 是/否 |

## 常见问题

#### 如何使用亚马逊智能卫星仓费用指标报告？

亚马逊智能卫星仓费用指标报告是一份每周报告，用于追踪关键费用指标，如总历史供货天数、自动补货率和自动补货自定义功能（最小和最大）使用标志。该报告显示了每日趋势，可帮助您及时做出库存调整决定。

【亚马逊物流费用适用性】列根据自动补货率和自定义功能使用标记，显示您的 SKU 在指定日期是否需要缴纳亚马逊物流附加费。

不同亚马逊物流费用的确定周期不同，因此您可以在[亚马逊物流库存](https://sellercentral.amazon.com/inventoryplanning/manageinventoryhealth?ref_=xx_invplan_favb_xx)、[月度仓储费报告](https://sellercentral.amazon.com/reportcentral/STORAGE_FEE_CHARGES/1)和[超龄库存附加费报告](https://sellercentral.amazon.com/reportcentral/LONGTERM_STORAGE_FEE_CHARGES/0)中查看实际费用。

#### 如何核对付款控制面板上的费用与亚马逊智能卫星仓费用报告中的费用的差异？

亚马逊智能卫星仓费用报告包含与付款控制面板交易视图中的订单编号匹配的“myp_order_id”列。

虽然付款控制面板通常在一行中显示合并的费用，但技术处理有时可能会将这些费用拆分为多个交易。在这种情况下，相关订单编号会使用特定格式表示拆分订单。例如，“2025-04-A1ZEBA98JHW8LI_1of2”表明一个交易分成了两个部分，这是第一部分。此功能可帮助您轻松核对亚马逊智能卫星仓报告与付款控制面板的费用差异。

#### 赔偿金额在获得批准后会显示在什么位置？

您可以前往[付款控制面板](https://sellercentral.amazon.com/payments/dashboard/index.html/ref=xx_payments_dnav_xx)上的【交易一览】选项卡查看赔偿。从【账户类型】下拉菜单中选择【标准订单】，然后从【交易类型】下拉菜单中选择【其他】。选择这些选项后，查看赔偿金额被归类为【其他】的【商品详情】。

#### 计算费用时会取小数点后几位？

我们在计算费用和卖家平台报告时取小数点后两位。

#### 如何确定和收取处理费费率？是否按货件计算，是否还包括托拍？

自 2025 年 4 月 1 日起，当我们的分拨中心收到您的库存时，我们将在入库时收取处理费，当补货订单成功送至我们的配送网络或其他销售渠道时，我们将在出库时再次收取处理费。要查看处理费费率，请参阅[亚马逊智能卫星仓费用](https://sellercentral.amazon.com/gp/help/external/GAYG62Q3MPE6STFS)。处理费按箱计算。虽然我们支持在亚马逊智能卫星仓西海岸托拍装运地区通过托拍入库，但是我们会按箱收取处理费。

#### 从亚马逊智能卫星仓向亚马逊配送网络自动补货时，是否收取单个 ASIN 的标签费用？ 如果是，是否可在卖家平台报告中单独追踪此费用？

从亚马逊智能卫星仓运往亚马逊物流的出库补货无需支付单独的贴标费用。在入库操作时粘贴在包装箱上的标签还可用于出库补货。补货无需单独贴标。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GPB467PZW3AZC4V3
