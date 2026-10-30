---
title: "为包含 AI 生成人物的媒体添加标签"
doc_id: GFXHCHYZRGJRBZA5
source: https://sellercentral.amazon.com/help/hub/reference/external/GFXHCHYZRGJRBZA5
language: zh-CN
fetched_at: 2026-10-30T13:35:01
---

# 为包含 AI 生成人物的媒体添加标签

如果您的图片或视频包含由 AI 生成的人物，请了解如何更新元数据。

为了遵守要求在商品媒体中披露 AI 生成人物的司法管辖区规定，亚马逊要求销售伙伴在上传前对适用的媒体添加标签。

如果您的媒体包含 AI 生成的人物，则必须将 contains-synthetic-performer 关键词添加到 XMP dc:subject 字段。具体而言，元数据必须在 XMP dc:subject rdf:Bag 内包含一个值为 contains-synthetic-performer 的 rdf:li。

许多支持 XMP 的工具可供使用，具体取决于您的操作系统和工作流程。以下说明涵盖了适用于 macOS 和 Windows 的内置工具，以及适用于其他系统的命令行选项。

## 在 macOS 上为图片添加标签

使用“预览”添加关键词：

- 在【预览】中打开该文件。

- 使用 【Cmd+I】 打开检查器（或选择【工具】，然后选择【显示检查器】）。

- 点击【关键词】选项卡。

- “关键词”窗格最初将显示“无关键词”。（图 1）

![](https://m.media-amazon.com/images/G/01/Vendor_Editorial/contains-synthetic-performer/AI_Fig1.png)

图 1

- 点击窗格底部的 【+】 按钮。

- 键入 

［
contains-synthetic-performer
］
并点击 【Enter】。

- 结果： 关键词会显示在列表中。（图 2）

![](https://m.media-amazon.com/images/G/01/Vendor_Editorial/contains-synthetic-performer/AI_Fig2.png)

图 2

## 在 Windows 上为图片添加标签

使用文件资源管理器添加关键词：

- 右击该文件，然后选择【属性】。

- 前往【详细信息】选项卡。

- 在“说明”部分中，找到“标记”字段。（【主题】和【标记】字段会写入不同的元数据位置。请仅使用“标记”字段）

- 在

［
标记
］
字段中输入 【contains-synthetic-performer】。

- 保留【主题】字段不变。

- 选择【确定】。

- 结果： 您会看到该关键词已添加。（图 3）

![](https://m.media-amazon.com/images/G/01/Vendor_Editorial/contains-synthetic-performer/AI_Fig3.png)

图 3

## 使用命令行工具为媒体添加标签

其他跨平台命令行工具也可为不同系统类型（例如，Linux 发行版）中的图片和视频添加 XMP 标签。

以下示例使用 exiftool。

**为单个文件添加标签**

要添加关键词，请先检查当前状态，然后写入并验证：

exiftool -G1 javelinas.png | grep Subject
# (no output — Subject is empty)

exiftool -XMP-dc:Subject+=contains-synthetic-performer javelinas.png
# 1 image files updated

exiftool -G1 javelinas.png | grep Subject
# [XMP-dc] Subject: contains-synthetic-performer

**批量为文件添加标签**

要为多个文件同时添加标签，请使用相同的命令并指定更广泛的文件目标：

为当前文件夹中的所有 PNG 图片添加标签：

exiftool -XMP-dc:Subject+=contains-synthetic-performer *.png
# 5 image files updated

为特定文件单独添加标签：

exiftool -XMP-dc:Subject+=contains-synthetic-performer image1.png image2.jpg video.mp4 
# 3 image files updated

**有关 += 运算符的重要详细信息：**

- 该运算符会附加到关键词包中，而不覆盖现有关键词。

- 运行同一命令两次会将该关键词写入两次。

- 重复项不会破坏标记，但会不必要地增加 XMP 数据包的大小。

## 验证标签

添加关键词后，验证 XMP dc:subject 字段中是否存在 contains-synthetic-performer 值。请使用任何可以显示显式 XMP dc:subject 字段的工具。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GFXHCHYZRGJRBZA5
