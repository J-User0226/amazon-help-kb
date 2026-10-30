---
title: "向亚马逊提交配件数据"
doc_id: GRB9TXB3SNPTVCKW
source: https://sellercentral.amazon.com/help/hub/reference/external/GRB9TXB3SNPTVCKW
language: zh-CN
fetched_at: 2026-10-30T13:49:38
---

# 向亚马逊提交配件数据

通过 AFM 或配件工具直接向亚马逊提交汽车配件数据，或通过第三方数据提供商提交。

您可以通过两种方式向我们提交配件数据：

- **直接： **您负责通过汽车配件管理器 (AFM) 或配件工具在卖家平台提交配件数据“直接”方法是首选方法。

- **间接： **您依靠第三方数据提供商代表您创建配件数据并将其提交给亚马逊。

上传配件数据后，请留出时间，等待其与商品匹配并显示在零件查找器上。我们目录中已有商品的配件数据最长可能需要 1 周才会显示。如果您要为新创建的商品上传配件数据，最长可能需要 3 周。

## 直接数据提交

**第 1 步： 满足所有先决条件**

- 先决条件在[汽车配件入门](https://sellercentral.amazon.com/help/hub/reference/G201710040)中进行了概述中进行了概述。

**第 2 步： 访问您的提交工具、AFM 或配件工具。**

- 在卖家平台中，前往【库存】，然后选择【管理汽车配件数据】。

**第 3 步： 提交您的配件数据**

- **通过[汽车配件管理器 (AFM)](https://sellercentral.amazon.com/automotive-mfm/) 批量提交**

- 请按照[构建 ACES 配件文件](https://sellercentral.amazon.com/help/hub/reference/GTVEB7S6YY5WVPMR)中所述的格式准备 ACES XML 文件中所述的格式准备 ACES XML 文件。

- 使用 XMLlint 或其他 XML 验证器根据 ACES 架构验证文件。请参阅[亚马逊 ACES XML 架构参考](https://sellercentral.amazon.com/help/hub/reference/GUL78KEJEPGJUXVA)。

- 通过 AFM 控制面板上传一个或多个文件。注意： 亚马逊每次提交仅接受最大 1 GB 的文件，因此您可能需要将大文件拆分后分多次上传。

- 在 AFM 控制面板中监控处理状态。请查看被拒记录的错误报告。

- **通过[配件工具](https://sellercentral.amazon.com/automotive/fitment/)单独提交**

- 在配件工具控制面板中，点击右上角的**添加 ASIN**。

- 对于您具有在售报价的任何 ASIN，输入 ASIN 代码，然后点击**提交**。

- 在模板页面上，添加车辆申请，包括年份、品牌、型号和车辆类型。

- 添加完申请后，选择**保存并提交**。

- **针对特殊使用案例的 S3 直接访问**

- 如果您是具有 AWS 服务（如 IAM 角色和 S3）使用经验的大批量提供商，我们可以通过 S3 设置直接 ACES 文件提交。要申请 S3 直接访问，请通过卖家平台向**汽车数据质量**提交支持问题单。

**第 4 步： 监控和维护**

- **查看错误报告。** 请在每次提交后检查 AFM 控制面板。如果上传数据因结构性原因被拒绝，请根据架构重新验证。如果上传数据未通过 VCdb 验证，请查看报告中的具体错误消息。

- **在配件数据发生变化时发送更新。** 在 UPDATE 上传数据中同时包含添加 (action="A") 和删除 (action="D")。您还可以提交 FULL 上传数据，以替换给定的 {provider, brand code, part number} 组合的所有记录。

- **要更正零件编号**，请先删除旧记录 (action="D")，然后添加更正后的记录 (action="A")。这两个步骤可以位于同一个 XML 文件中。注意： 仅提交新记录而不删除旧记录，会导致错误记录与新记录一同保留在系统中。

**最佳实践**

- **请勿过度映射：** 请仅提交使商品与车辆匹配所需的配件信息。请勿包含不必要的属性，如引擎或车身款式，除非需要区分配件。

- **请勿为通用型商品提交特定于车辆的配件记录。** 如果商品适用于所有车辆，提交过多的配件信息可能会导致我们移除您提交的内容。

## 间接数据提交

您可以使用第三方汽车数据供应商代为创建并提交 ACES 配件数据。我们目前与以下提供商合作。请直接联系这些公司来安排提交您的配件数据。

- Epicor Software Corporation

- SEMA Data Co-op

- OptiCat

- DCI (Direct Communications Incorporated)

有关这些提供商和其他提供商的更多信息，请访问 [autocare.org](https://www.autocare.org)。如果您对使用哪个提供商有疑问，请联系 automotive-dataprovider@amazon.com。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GRB9TXB3SNPTVCKW
