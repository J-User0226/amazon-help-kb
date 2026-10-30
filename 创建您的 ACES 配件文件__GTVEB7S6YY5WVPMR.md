---
title: 创建您的 ACES 配件文件
doc_id: GTVEB7S6YY5WVPMR
source: https://sellercentral.amazon.com/help/hub/reference/external/GTVEB7S6YY5WVPMR
language: zh-CN
fetched_at: 2026-10-30 13:56:39
---

# 创建您的 ACES 配件文件

构建并验证您的 ACES XML 配件文件，包括标头元素、申请记录和上传数据类型。

## ACES 标准
- **格式：** 嵌套 XML，每个品牌一个文件
- **数据：** 零件数据（品牌名称、零件编号、零件类型）以及申请信息，如哪种车辆、哪些车辆属性以及零件适合安装在车辆上的哪个位置
- **车辆：** Auto Care 的车辆配置数据库 (VCdb) 包含车辆、属性和配置的标准列表。ACES 文件将零件映射到 VCdb 车辆。VCdb 每月更新一次，可供会员在 [autocare.org](https://www.autocare.org) 上获取。
- **零件类型：** 零件配置数据库 (PCdb) 包含零件类型和分类的标准列表，例如“刹车片”“火花塞”。PCdb 也是每月更新一次，并可在 [autocare.org](https://www.autocare.org) 上获取。
- **品牌名称：** Auto Care 维护着一个父级标签、品牌所有者标签、品牌标签和子品牌标签的存储库。每个标签都分配了一个代码，用于在 ACES 文件中传达品牌信息。您可以通过 [Auto Care VIP 门户](https://autocarevip.com)访问这些信息，或直接通过 technology@autocare.org 与 Auto Care 联系。
- 有关 ACES 标准的更多信息，请访问[汽车护理协会网站](https://www.autocare.org)。

## ACES 文件剖析
ACES 文件是带有架构定义的 XML 文件 (XSD)。主要元素如下：
**元素** **描述**
<ACES> 根元素
<Header> 文件元数据，包括品牌代码、发送者和文档标题
<App> 申请记录 - 将零件映射到车辆
<Footer> 要验证的记录数

**架构定义区分大小写，并且元素的顺序很重要。**元素必须按架构所定义的顺序显示： [亚马逊 ACES XML 架构参考](https://sellercentral.amazon.com/help/hub/reference/GUL78KEJEPGJUXVA)。

## ACES 标头示例
标头必须按以下顺序包含下列元素。标有“必填”的元素必须存在；其他元素为可选。

<Header> <Company>Your Company Name</Company> <!-- required --> <SenderName>Your Name</SenderName> <!-- required --> <SenderPhone>555-123-4567</SenderPhone> <!-- required --> <TransferDate>2026-04-30</TransferDate> <!-- required --> <BrandAAIAID>ABCD</BrandAAIAID> <!-- required for Amazon --> <DocumentTitle>My ACES File</DocumentTitle> <!-- required --> <EffectiveDate>2026-04-30</EffectiveDate> <!-- required --> <SubmissionType>UPDATE</SubmissionType> <!-- required: FULL, UPDATE, or TEST --> <MapperCompany>Epicor Software</MapperCompany> <!-- recommended when a third party manages submission --> <MapperContact>Jane Smith</MapperContact> <!-- recommended when a third party manages submission --> <MapperPhone>555-987-6543</MapperPhone> <!-- recommended when a third party manages submission --> <MapperEmail>jane@epicor.com</MapperEmail> <!-- recommended when a third party manages submission --> <VcdbVersionDate>2026-03-29</VcdbVersionDate> <!-- required --> <QdbVersionDate>2026-03-29</QdbVersionDate> <!-- required --> <PcdbVersionDate>2026-03-29</PcdbVersionDate> <!-- required --> </Header> **注意： **当第三方代表品牌管理 ACES 提交内容时，应填写 Mapper* 字段（MapperCompany、MapperContact、MapperPhone、MapperPhoneExt、MapperEmail）。例如，如果 Epicor 代表品牌 X 提交配件数据，则 Company 和 SenderName 字段标识品牌 X，而 Mapper* 字段将 Epicor 标识为提交方。

## 申请记录示例
在每个 <App> 元素内，子元素的顺序必须遵循架构。一般顺序为：车辆识别 → 车辆属性 → <Qty> → <PartType> → <Position>（可选）→ <Part>。

## 使用 BaseVehicle 元素
**添加记录**

<App action="A" id="1"> <BaseVehicle id="2345"/> <EngineBase id="678"/> <Qty>1</Qty> <PartType id="7120"/> <Part>ABC123</Part> </App>

**删除记录**

<App action="D" id="3"> <BaseVehicle id="2345"/> <EngineBase id="678"/> <Qty>1</Qty> <PartType id="7120"/> <Part>ABC123</Part> </App>

- 删除记录必须与发送至亚马逊的原始添加记录完全匹配。
- 添加记录和删除记录可以包含在同一 XML 文件中： 将 action="D" 记录放在 action="A" 记录之前。

## FULL 与 UPDATE 上传数据
上传数据类型 说明
**更新** UPDATE 是最常见的提交类型。使用 action="A" 添加记录，使用 action="D" 删除记录。
**FULL** FULL 将替换文件中包含的每个 {provider, brand code, part number} 组合的所有记录。提交内容中不包含的记录不受影响。也就是说，FULL 替换的是您提到的内容，而不是您曾发送给我们的全部内容。
在隐式替换后，我们将支持并处理 FULL 上传数据中的删除记录。

**注意： **如果您要更改零件编号，则新零件编号的 FULL 上传数据不会删除旧零件编号下的记录。您仍必须使用 action="D" 的 UPDATE 上传数据显式删除旧记录。

**TEST** TEST 上传数据执行完整验证，但不保留任何记录。我们生成的处理报告与 FULL 或 UPDATE 上传数据的处理报告相同。在正式提交前，使用 TEST 验证您的文件是否会被接受。在标头中设置为 <SubmissionType>TEST</SubmissionType>。

## 架构验证
提交之前，请根据我们自定义的 ACES 架构验证您的 ACES 文件： [亚马逊 ACES XML 架构参考](https://sellercentral.amazon.com/help/hub/reference/GUL78KEJEPGJUXVA)。将架构另存为 aces.xsd，并运行：xmllint --schema aces.xsd your_aces_file.xml –noout。或者，使用您选择的任何 XML 验证器。

在提交前进行验证将发现结构性错误，并在上传数据因结构性原因被拒绝时加快故障排除。如果上传数据因其他原因（例如 VCdb 验证失败）而被拒绝，请在 AFM 控制面板中查看错误报告。

**我们使用 ACES 3.2 架构的自定义修补版本。符合其他架构版本的文件将被拒绝。**虽然汽车护理协会已经发布了更新版本的 ACES 标准，但是我们不支持这些版本。您必须使用我们提供的架构验证并提交您的文件。

## 针对亚马逊的 ACES 要求
1. **BrandAAIAID 在标头中为必填元素**。它必须包含您为要其提交配件数据的品牌在[品牌表](http://brandtable.pricedex.com/)中的品牌代码（而不是父代码或品牌所有者代码）。
2. **区域 ID：** 1 = 美国，2 = 加拿大，3 = 墨西哥。如果已指定，配件信息仅适用于该区域。如果省略此选项，则数据仅在记录值有效的区域适用。
3. BodyType 值映射到“unknown”“U/K”“N/R”“N/A”“N/S”或“-”的申请记录将引发验证错误并被拒绝。
4. **FULL 上传数据**将替换文件中存在的每个 {provider, brand code, part number} 组合的所有记录。提交中未包含的零件编号或品牌的记录不受影响。FULL 上传数据中的删除记录会进行处理。**我们首选在您初始 FULL 文件后接收净更改 ACES 文件（通过 UPDATE 上传数据添加和删除）。**
5. 与您的品牌代码关联的品牌名称必须与您的 ASIN 上的品牌名称一致。我们通过品牌名称到品牌代码的映射表来解析品牌。如果您的品牌名称已随时间发生变化，请提交支持 TT，并请求我们更新您品牌代码的别名。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GTVEB7S6YY5WVPMR
