---
title: 重新发布“非在售”Amazon Handmade 商品
doc_id: G2YC8BRR324G39TY
source: https://sellercentral.amazon.com/help/hub/reference/external/G2YC8BRR324G39TY
language: zh-CN
fetched_at: 2026-10-30 13:15:51
---

# 重新发布“非在售”Amazon Handmade 商品

您的 Amazon Handmade 销售权限恢复后，您将发现您的 ASIN 仍处于“非在售”状态。

## 手动重新启售商品
重新启售商品最简单的方法是通过对每个 ASIN 进行简单的编辑，尝试手动重新启售。
1. 前往[管理库存](https://sellercentral.amazon.com/hz/inventory)页面。
2. 点击每个 Amazon Handmade 商品右侧的**编辑**。
3. 通过在您的描述中添加空格或标点符号来进行小更新。
4. 点击【保存并完成】

您的 Amazon Handmade 商品应该会在几分钟内变为在售状态。如果这些步骤不起作用，请按照以下说明使用库存加载工具。

## 使用库存加载工具
如果您有很多 ASIN 要重新启售或手动重新启售不起作用，您可以尝试使用库存加载工具重新上传商品信息。以下说明可引导您完成此流程。

**第 1 步： 创建非在售商品报告**
1. 前往[库存报告](https://sellercentral.amazon.com/listing/reports/ref=xx_invreport_dnav_home)。
2. 从【选择报告类型】下拉菜单中，选择【非在售商品报告】。
3. 点击【请求报告】。
4. 在报告准备就绪后，点击【下载】。
5. 将此文件保存到您的桌面。

**第 2 步： 下载并填写库存文件**
1. 下载[库存加载工具模板](https://s3.amazonaws.com/seller-templates/ff/na/us/Flat.File.InventoryLoader_b2b.xls)
2. 从您在第 1 步中下载的【非在售商品】报告中复制以下信息，并将其粘贴到您的库存加载工具模板中。
  - SKU
  - 商品编码 = *输入与您的商品关联的 ASIN*
  - 商品编码类型 = 1
  - 商品价格
  - 商品状况 = 11 – *这表示该商品是新品*
  - 数量 *– 如果商品是亚马逊物流商品，请将此字段留空*
  - 添加删除 = a *- 表示您在添加新商品，而非删除商品*
  - 运营中心编码 – *仅限 ASIN 为亚马逊物流商品时填写*

3. 所有必填字段信息填写完成后，请保存文件。

**第 3 步： 上传库存文件**
1. 前往[批量上传商品](https://sellercentral.amazon.com/listing/upload?ref_=xx_upload_tnav_download)。
2. 选择【上传您的库存文件】选项卡。
3. 上传文件：
  - 从【文件类型】字段，选择【库存加载工具文件】。
  - 在【文件上传】字段，选择【选择文件】并上传您已更新/保存的文件。
  - 在【电子邮件提醒】字段中输入您的电子邮件地址。上传您的文件后，我们将通过此电子邮件地址与您联系。
  - 选择您希望处理报告（输出）的格式采用 Excel 格式（推荐使用）还是文本格式。
  - 点击【上传】。

**注意： **上传后，您可以查看处理报告，了解有关识别任何潜在的库存文件上传错误的说明。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/G2YC8BRR324G39TY
