---
title: "亚马逊 ACES XML 架构参考"
doc_id: GUL78KEJEPGJUXVA
source: https://sellercentral.amazon.com/help/hub/reference/external/GUL78KEJEPGJUXVA
language: zh-CN
fetched_at: 2026-10-30T14:00:43
---

# 亚马逊 ACES XML 架构参考

下载亚马逊 ACES 架构，并查看 App 和 Header 记录所需的元素顺序。

## 重要详情

我们使用定制 ACES 架构（版本 3.2，亚马逊修补版），兼容 ACES 3.2 和 ACES 4.0 所有元素。这是目前我们接受的唯一架构版本。

- **ACES 版本：** 根元素中的版本将被忽略。它并不控制我们如何解析和验证您的文件。

- **操作：** 仅支持 A（添加）和 D（删除）。无效操作会跳过该记录，并生成错误。

- **车辆标识：** 车辆必须通过 <BaseVehicle> 和 <SubModel>（可选）进行标识；或者通过 <Years>、<Make>、<Model> 和 <SubModel>（可选）进行标识。不支持其他车辆标识方法。

- **提交类型：** 可以是 FULL、UPDATE 或 TEST。TEST 上传数据执行完整验证，但不保留任何记录。我们生成相同的处理报告，使 TEST 可用于在正式提交前验证上传数据。

- **数量：** 任何无法转换为正整数的值都会被自动设置为 1。

- **元素顺序很重要。** <App> 中的元素必须按照下面定义的顺序显示。

## App 元素顺序

在每个 <App> 记录中，元素必须按以下顺序显示：

- 车辆识别：<BaseVehicle> 或 <Years>/<Make>/<Model>（可选 <SubModel>）

- 车辆属性（均为可选）：<MfrBodyCode>、<BodyNumDoors>、<BodyType>、<DriveType>、<EngineBase>、<EngineDesignation>、<EngineVIN>、<EngineVersion>、<EngineMfr>、<PowerOutput>、<ValvesPerEngine>、<FuelDeliveryType>、<FuelDeliverySubType>、<FuelSystemControlType>、<FuelSystemDesign>、<Aspiration>、<CylinderHeadType>、<FuelType>、<IgnitionSystemType>、<TransmissionMfrCode>、变速箱组、<TransElecControlled>、<TransmissionMfr>、<BedLength>、<BedType>、<WheelBase>、<BrakeSystem>、<FrontBrakeType>、<RearBrakeType>、<BrakeABS>、<FrontSpringType>、<RearSpringType>、<SteeringSystem>、<SteeringType>、<Region>、<Qual>、<Note>

- <Qty>（必填）

- <PartType>（必填）

- <MfrLabel>（可选）

- <Position>（可选）

- <Part>（必填）

- <DisplayOrder>（可选）

## Header 元素顺序

- <Company>（必填）

- <SenderName>（必填）

- <SenderPhone>（必填）

- <SenderPhoneExt>（可选）

- <TransferDate>（必填）

- <MfrCode>（可选）

- <BrandAAIAID>（亚马逊必填）

- <DocumentTitle>（必填）

- <DocFormNumber>（可选）

- <EffectiveDate>（必填）

- <ApprovedFor>（可选）

- <PartsApprovedFor>（可选）

- <RegionFor>（可选）

- <SubmissionType>（必填： FULL、UPDATE 或 TEST)

- <MapperCompany>（可选，但建议填写）

- <MapperContact>（可选，但建议填写）

- <MapperPhone>（可选，但建议填写）

- <MapperPhoneExt>（可选，但建议填写）

- <MapperEmail>（可选，但建议填写）

- <VcdbVersionDate>（必填）

- <QdbVersionDate>（必填）

- <PcdbVersionDate>（必填）

## 完整架构

**将其另存为 aces.xsd，并用于 XMLlint 或任何 XML 验证器。**

<?xml version="1.0" encoding="UTF-8"?>
<xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema"
elementFormDefault="qualified"
version="3.2_amzn_patched" xml:lang="en">

<!-- Simple type definitions -->
<xs:simpleType name="acesVersionType">
<xs:restriction base="xs:string">
<xs:minLength value="3"/>
<xs:maxLength value="5"/>
</xs:restriction>
</xs:simpleType>

<xs:simpleType name="actionType">
<xs:restriction base="xs:token">
<xs:length value="1"/>
</xs:restriction>
</xs:simpleType>

<xs:simpleType name="assetNameType">
<xs:restriction base="xs:NMTOKEN">
<xs:minLength value="1"/>
<xs:maxLength value="45"/>
</xs:restriction>
</xs:simpleType>

<xs:simpleType name="brandType">
<xs:restriction base="xs:string">
<xs:pattern value="[B-Z-[EIOU]][B-Z-[EIO]][B-Z-[OU]][A-Z]"/>
</xs:restriction>
</xs:simpleType>

<xs:simpleType name="idType">
<xs:restriction base="xs:positiveInteger"/>
</xs:simpleType>

<xs:simpleType name="partNumberBaseType">
<xs:restriction base="xs:token">
<xs:minLength value="0"/>
<xs:maxLength value="45"/>
</xs:restriction>
</xs:simpleType>

<xs:simpleType name="uomType">
<xs:restriction base="xs:token">
<xs:minLength value="1"/>
<xs:maxLength value="3"/>
</xs:restriction>
</xs:simpleType>

<xs:simpleType name="yearType">
<xs:restriction base="xs:positiveInteger">
<xs:totalDigits value="4"/>
<xs:minInclusive value="1896"/>
</xs:restriction>
</xs:simpleType>

<xs:simpleType name="yesnoType">
<xs:restriction base="xs:token">
<xs:minLength value="2"/>
<xs:maxLength value="3"/>
</xs:restriction>
</xs:simpleType>

<xs:simpleType name="submissionType">
<xs:restriction base="xs:string">
<xs:minLength value="4"/>
<xs:maxLength value="6"/>
</xs:restriction>
</xs:simpleType>

<!-- Complex type definitions -->
<xs:complexType name="approvedForType" mixed="true">
<xs:sequence>
<xs:element name="Country" minOccurs="0" maxOccurs="unbounded">
<xs:simpleType>
<xs:restriction base="xs:token">
<xs:length value="2"/>
</xs:restriction>
</xs:simpleType>
</xs:element>
</xs:sequence>
</xs:complexType>

<xs:complexType name="appItemsBaseType" abstract="true">
<xs:sequence>
<xs:group ref="vehicleIdentGroup"/>
<xs:element ref="MfrBodyCode" minOccurs="0"/>
<xs:element ref="BodyNumDoors" minOccurs="0"/>
<xs:element ref="BodyType" minOccurs="0"/>
<xs:element ref="DriveType" minOccurs="0"/>
<xs:element ref="EngineBase" minOccurs="0"/>
<xs:element ref="EngineDesignation" minOccurs="0"/>
<xs:element ref="EngineVIN" minOccurs="0"/>
<xs:element ref="EngineVersion" minOccurs="0"/>
<xs:element ref="EngineMfr" minOccurs="0"/>
<xs:element ref="PowerOutput" minOccurs="0"/>
<xs:element ref="ValvesPerEngine" minOccurs="0"/>
<xs:element ref="FuelDeliveryType" minOccurs="0"/>
<xs:element ref="FuelDeliverySubType" minOccurs="0"/>
<xs:element ref="FuelSystemControlType" minOccurs="0"/>
<xs:element ref="FuelSystemDesign" minOccurs="0"/>
<xs:element ref="Aspiration" minOccurs="0"/>
<xs:element ref="CylinderHeadType" minOccurs="0"/>
<xs:element ref="FuelType" minOccurs="0"/>
<xs:element ref="IgnitionSystemType" minOccurs="0"/>
<xs:element ref="TransmissionMfrCode" minOccurs="0"/>
<xs:group ref="transGroup" minOccurs="0"/>
<xs:element ref="TransElecControlled" minOccurs="0"/>
<xs:element ref="TransmissionMfr" minOccurs="0"/>
<xs:element ref="BedLength" minOccurs="0"/>
<xs:element ref="BedType" minOccurs="0"/>
<xs:element ref="WheelBase" minOccurs="0"/>
<xs:element ref="BrakeSystem" minOccurs="0"/>
<xs:element ref="FrontBrakeType" minOccurs="0"/>
<xs:element ref="RearBrakeType" minOccurs="0"/>
<xs:element ref="BrakeABS" minOccurs="0"/>
<xs:element ref="FrontSpringType" minOccurs="0"/>
<xs:element ref="RearSpringType" minOccurs="0"/>
<xs:element ref="SteeringSystem" minOccurs="0"/>
<xs:element ref="SteeringType" minOccurs="0"/>
<xs:element ref="Region" minOccurs="0"/>
<xs:element ref="Qual" minOccurs="0" maxOccurs="unbounded"/>
<xs:element ref="Note" minOccurs="0" maxOccurs="unbounded"/>
</xs:sequence>
<xs:attribute name="action" type="actionType" use="required"/>
<xs:attribute name="id" type="idType" use="required"/>
<xs:attribute name="ref" type="xs:string"/>
<xs:attribute name="validate" type="yesnoType" default="yes"/>
</xs:complexType>

<xs:complexType name="appType">
<xs:complexContent>
<xs:extension base="appItemsBaseType">
<xs:sequence>
<xs:element ref="Qty"/>
<xs:element ref="PartType"/>
<xs:element ref="MfrLabel" minOccurs="0"/>
<xs:element ref="Position" minOccurs="0"/>
<xs:element ref="Part"/>
<xs:element ref="DisplayOrder" minOccurs="0"/>
<xs:sequence minOccurs="0">
<xs:element ref="AssetName"/>
<xs:element ref="AssetItemOrder" minOccurs="0"/>
<xs:element ref="AssetItemRef" minOccurs="0"/>
</xs:sequence>
</xs:sequence>
</xs:extension>
</xs:complexContent>
</xs:complexType>

<xs:complexType name="noteType">
<xs:simpleContent>
<xs:extension base="xs:string">
<xs:attribute name="id" type="idType"/>
<xs:attribute name="lang" type="xs:token"/>
</xs:extension>
</xs:simpleContent>
</xs:complexType>

<xs:complexType name="partNumberType">
<xs:simpleContent>
<xs:extension base="partNumberBaseType">
<xs:attribute name="BrandAAIAID" type="brandType"/>
</xs:extension>
</xs:simpleContent>
</xs:complexType>

<xs:complexType name="partTypeType">
<xs:simpleContent>
<xs:extension base="xs:string">
<xs:attribute name="id" type="idType" use="required"/>
</xs:extension>
</xs:simpleContent>
</xs:complexType>

<xs:complexType name="positionType">
<xs:simpleContent>
<xs:extension base="xs:string">
<xs:attribute name="id" type="idType" use="required"/>
</xs:extension>
</xs:simpleContent>
</xs:complexType>

<xs:complexType name="qualType">
<xs:sequence>
<xs:element name="param" type="paramType" minOccurs="0" maxOccurs="unbounded"/>
<xs:element name="text" type="xs:string"/>
</xs:sequence>
<xs:attribute name="id" type="idType" use="required"/>
</xs:complexType>

<xs:complexType name="paramType">
<xs:simpleContent>
<xs:extension base="xs:string">
<xs:attribute name="value" type="xs:string" use="required"/>
<xs:attribute name="uom" type="uomType"/>
<xs:attribute name="altvalue" type="xs:string"/>
<xs:attribute name="altuom" type="uomType"/>
</xs:extension>
</xs:simpleContent>
</xs:complexType>

<xs:complexType name="vehAttrType">
<xs:simpleContent>
<xs:extension base="xs:string">
<xs:attribute name="id" type="idType" use="required"/>
</xs:extension>
</xs:simpleContent>
</xs:complexType>

<xs:complexType name="yearRangeType">
<xs:simpleContent>
<xs:extension base="xs:string">
<xs:attribute name="from" use="required">
<xs:simpleType>
<xs:restriction base="yearType"/>
</xs:simpleType>
</xs:attribute>
<xs:attribute name="to" type="yearType" use="required"/>
</xs:extension>
</xs:simpleContent>
</xs:complexType>

<!-- Document structure -->
<xs:element name="ACES">
<xs:complexType>
<xs:sequence>
<xs:element ref="Header"/>
<xs:element ref="App" minOccurs="0" maxOccurs="unbounded"/>
<xs:element ref="Asset" minOccurs="0" maxOccurs="unbounded"/>
<xs:element ref="Footer"/>
</xs:sequence>
<xs:attribute name="version" type="acesVersionType"/>
</xs:complexType>
</xs:element>

<!-- Header element -->
<xs:element name="Header">
<xs:complexType>
<xs:sequence>
<xs:element name="Company" type="xs:string"/>
<xs:element name="SenderName" type="xs:string"/>
<xs:element name="SenderPhone" type="xs:string"/>
<xs:element name="SenderPhoneExt" type="xs:string" minOccurs="0"/>
<xs:element name="TransferDate" type="xs:date"/>
<xs:element name="MfrCode" type="xs:string" minOccurs="0"/>
<xs:element name="BrandAAIAID" type="brandType" minOccurs="0"/>
<xs:element name="DocumentTitle" type="xs:string"/>
<xs:element name="DocFormNumber" type="xs:string" minOccurs="0"/>
<xs:element name="EffectiveDate" type="xs:date"/>
<xs:element name="ApprovedFor" type="approvedForType" minOccurs="0"/>
<xs:element name="PartsApprovedFor" type="approvedForType" minOccurs="0"/>
<xs:element name="RegionFor" type="RegionType" minOccurs="0"/>
<xs:element name="SubmissionType" type="submissionType"/>
<xs:element name="MapperCompany" type="xs:string" minOccurs="0"/>
<xs:element name="MapperContact" type="xs:string" minOccurs="0"/>
<xs:element name="MapperPhone" type="xs:string" minOccurs="0"/>
<xs:element name="MapperPhoneExt" type="xs:string" minOccurs="0"/>
<xs:element name="MapperEmail" type="xs:string" minOccurs="0"/>
<xs:element name="VcdbVersionDate" type="xs:date"/>
<xs:element name="QdbVersionDate" type="xs:date"/>
<xs:element name="PcdbVersionDate" type="xs:date"/>
</xs:sequence>
</xs:complexType>
</xs:element>

<!-- Vehicle Identification Group -->
<xs:group name="vehicleIdentGroup">
<xs:choice>
<xs:sequence>
<xs:element ref="BaseVehicle"/>
<xs:element ref="SubModel" minOccurs="0"/>
</xs:sequence>
<xs:sequence>
<xs:element ref="Years"/>
<xs:element ref="Make"/>
<xs:choice minOccurs="0">
<xs:element ref="VehicleType"/>
<xs:sequence minOccurs="0">
<xs:element ref="Model"/>
<xs:element ref="SubModel" minOccurs="0"/>
</xs:sequence>
</xs:choice>
</xs:sequence>
</xs:choice>
</xs:group>

<!-- Transmission Group -->
<xs:group name="transGroup">
<xs:choice>
<xs:element ref="TransmissionBase"/>
<xs:sequence>
<xs:element ref="TransmissionType" minOccurs="0"/>
<xs:element ref="TransmissionControlType" minOccurs="0"/>
<xs:element ref="TransmissionNumSpeeds" minOccurs="0"/>
</xs:sequence>
</xs:choice>
</xs:group>

<!-- Element definitions -->
<xs:element name="App" type="appType"/>
<xs:element name="Aspiration" type="vehAttrType"/>
<xs:element name="Asset">
<xs:complexType>
<xs:complexContent>
<xs:extension base="assetType">
<xs:sequence>
<xs:element ref="AssetName"/>
</xs:sequence>
</xs:extension>
</xs:complexContent>
</xs:complexType>
</xs:element>
<xs:element name="AssetItemOrder" type="xs:positiveInteger"/>
<xs:element name="AssetItemRef" type="xs:string"/>
<xs:element name="AssetName" type="assetNameType"/>
<xs:element name="BaseVehicle" type="vehAttrType"/>
<xs:element name="BedLength" type="vehAttrType"/>
<xs:element name="BedType" type="vehAttrType"/>
<xs:element name="BodyNumDoors" type="vehAttrType"/>
<xs:element name="BodyType" type="vehAttrType"/>
<xs:element name="BrakeABS" type="vehAttrType"/>
<xs:element name="BrakeSystem" type="vehAttrType"/>
<xs:element name="CylinderHeadType" type="vehAttrType"/>
<xs:element name="DisplayOrder" type="xs:positiveInteger"/>
<xs:element name="DriveType" type="vehAttrType"/>
<xs:element name="EngineBase" type="vehAttrType"/>
<xs:element name="EngineDesignation" type="vehAttrType"/>
<xs:element name="EngineMfr" type="vehAttrType"/>
<xs:element name="EngineVIN" type="vehAttrType"/>
<xs:element name="EngineVersion" type="vehAttrType"/>
<xs:element name="FrontBrakeType" type="vehAttrType"/>
<xs:element name="FrontSpringType" type="vehAttrType"/>
<xs:element name="FuelDeliverySubType" type="vehAttrType"/>
<xs:element name="FuelDeliveryType" type="vehAttrType"/>
<xs:element name="FuelSystemControlType" type="vehAttrType"/>
<xs:element name="FuelSystemDesign" type="vehAttrType"/>
<xs:element name="FuelType" type="vehAttrType"/>
<xs:element name="IgnitionSystemType" type="vehAttrType"/>
<xs:element name="Make" type="vehAttrType"/>
<xs:element name="MfrBodyCode" type="vehAttrType"/>
<xs:element name="MfrLabel" type="xs:string"/>
<xs:element name="Model" type="vehAttrType"/>
<xs:element name="Note" type="noteType"/>
<xs:element name="Part" type="partNumberType"/>
<xs:element name="PartType" type="partTypeType"/>
<xs:element name="Position" type="positionType"/>
<xs:element name="PowerOutput" type="vehAttrType"/>
<xs:element name="Qty" type="xs:string"/>
<xs:element name="Qual" type="qualType"/>
<xs:element name="RearBrakeType" type="vehAttrType"/>
<xs:element name="RearSpringType" type="vehAttrType"/>
<xs:element name="Region" type="vehAttrType"/>
<xs:element name="SteeringSystem" type="vehAttrType"/>
<xs:element name="SteeringType" type="vehAttrType"/>
<xs:element name="SubModel" type="vehAttrType"/>
<xs:element name="TransElecControlled" type="vehAttrType"/>
<xs:element name="TransferDate" type="xs:date"/>
<xs:element name="TransmissionBase" type="vehAttrType"/>
<xs:element name="TransmissionControlType" type="vehAttrType"/>
<xs:element name="TransmissionMfr" type="vehAttrType"/>
<xs:element name="TransmissionMfrCode" type="vehAttrType"/>
<xs:element name="TransmissionNumSpeeds" type="vehAttrType"/>
<xs:element name="TransmissionType" type="vehAttrType"/>
<xs:element name="ValvesPerEngine" type="vehAttrType"/>
<xs:element name="VehicleType" type="vehAttrType"/>
<xs:element name="WheelBase" type="vehAttrType"/>
<xs:element name="Years" type="yearRangeType"/>

<xs:complexType name="RegionType">
<xs:sequence>
<xs:element ref="Region" maxOccurs="unbounded"/>
</xs:sequence>
</xs:complexType>

<xs:complexType name="assetType">
<xs:complexContent>
<xs:extension base="appItemsBaseType"/>
</xs:complexContent>
</xs:complexType>

<!-- Footer element -->
<xs:element name="Footer">
<xs:complexType>
<xs:sequence>
<xs:element name="RecordCount" type="xs:string"/>
</xs:sequence>
</xs:complexType>
</xs:element>

</xs:schema>

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GUL78KEJEPGJUXVA
