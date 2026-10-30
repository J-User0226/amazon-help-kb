---
title: "FSMA 204 数据共享要求"
doc_id: GVL2AASNCD56J329
source: https://sellercentral.amazon.com/help/hub/reference/external/GVL2AASNCD56J329
language: zh-CN
fetched_at: 2026-10-30T14:06:08
---

# FSMA 204 数据共享要求

美国食品药品监督管理局出台的食品可追踪性规则（通常称为 FSMA 204）计划于 2026 年 1 月 20 日生效。FSMA 204 的核心要求是，制造、加工、包装或持有美国食品药品监督管理局[食品可追踪性列表 (FTL)](https://www.fda.gov/food/food-safety-modernization-act-fsma/food-traceability-list) 上食品的供应商必须获取并共享一组定义的关键数据元素 (KDE)，以便这些记录能够快速提供给美国食品药品监督管理局，以应对潜在的食源传播疾病事件。

为了满足 FSMA 204 的食品可追踪性要求，亚马逊认为 **GS1 全球可追踪性标准**是在整个供应链中实现数据共享互操作性的最简单且经济有效的方式。根据[支持 FSMA 204 的 GS1 标准体系](https://documents.gs1us.org/adobe/assets/deliver/urn:aaid:aem:8037d451-b557-4b0f-9fa8-fc94f94e4547/GS1-US-Application-of-GS1-System-of-Standards-to-Support-FSMA-204-Guideline.pdf)的要求，我们要求所有食品可追踪性列表 (FTL) 商品的供应商在 2025 年 8 月 1 日之前遵循以下 FSMA 204 数据共享要求。

- **发货前通知 (ASN)** - 食品可追踪性列表 (FTL) 上的商品的所有已确认采购订单必须具有发货通知单。发货通知单必须包含 FSMA 204 合规性所要求的最低关键数据元素 (KDE)： 

- 采购订单 (PO) 编号

- 发货地址/收货地址

- GTIN（全球贸易项目代码）

- 数量

- 批次编号

- 可追踪性批次代码来源（或）可追踪性批次代码来源参考

- 首选 GS1 全球地点编号 (GLN)，但也可以接受等效的唯一企业编码，如 FFRN、DUNS 或 EIN。

- **托拍牌照标签 (LP) 标签** - 包含食品可追踪性列表 (FTL) 上商品的所有托拍商品必须贴有带有可扫描条形码的牌照 (LP) 标签，如序列装运集装箱代码 (SSCC)（首选）或等效标签，该标签可自动关联到发货通知单 (ASN)。

- **装运箱标签（GS1-128 或等效标签）**- 包含食品可追踪性列表 (FTL) 上商品的所有装运箱必须具有可扫描的 GS1-128 条形码（或等效标签），其中包含以下最低关键数据元素 (KDE) 和应用编码 (AI)：

- (01)： 全球贸易项目代码 (GTIN)

- (13)、(15) 或 (17)： 包装日期、最佳使用日期或保质期

- (10) 批次编号

虽然 GS1-128 装运箱标签已在食品行业广泛应用，但我们也接受具有 GS1 数字链接 URI 的 GS1 数据矩阵、二维码和数据矩阵代码，前提是它们编入了 GTIN、日期代码和批次编号信息。

**其他要求：**

- 单个装货箱只能包含一个批次编号

- 单个托拍的每个 UPC 只能包含一个批次编号

- 如果同一 UPC 有多个批次编号，则每个批次必须通过单独的托拍和/或货件发送

上述所有要求专门适用于美国食品药品监督管理局食品可追踪性列表 (FTL) 上的食品，但我们建议供应商对分配有可追踪性批次代码 (TLC) 的所有食品类商品采用这些标准。

要确定您销售的商品是否受 FSMA 204 管制，我们建议您查看美国食品药品监督管理局的 [FSMA 204 主页](https://www.fda.gov/food/food-safety-modernization-act-fsma/fsma-final-rule-requirements-additional-traceability-records-certain-foods?utm_campaign=On-Demand%20Webinar%20-%20Preparing%20for%20the%20Proposed%20FSMA%20204%20Rule%20with%20Chick-fil-A&utm_medium=email&_hsmi=164184131&_hsenc=p2ANqtz-_rlIVII5W_aTakzQGE0y3roVmvPPMf16Akoeec6WksEehOO985VQ8J_7lN2V4JWe07Xf-2-y6TV4Pkg64o3uI0pseZWA&utm_content=164184131&utm_source=hs_email)和美国食品药品监督管理局的[食品可追踪性列表 (FTL)](https://www.fda.gov/food/food-safety-modernization-act-fsma/food-traceability-list)。

**资源：**

- [GS1 的 FSMA 204 工具包](https://www.gs1us.org/content/dam/gs1us/documents/industries-insights/by-industry/food/GS1-US-FSMA-Rule-204-Toolkit-for-Solution-Provider-July-16-2024-R1.0.pdf)

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GVL2AASNCD56J329
