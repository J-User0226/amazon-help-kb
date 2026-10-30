---
title: Send to Amazon： 箱内物品信息 Excel 文件常见错误
doc_id: GX4SH82SZQNYUHCY
source: https://sellercentral.amazon.com/help/hub/reference/external/GX4SH82SZQNYUHCY
language: zh-CN
fetched_at: 2026-10-30 14:12:24
---

# Send to Amazon： 箱内物品信息 Excel 文件常见错误

本页面列出了您在使用 Send to Amazon 中的 Excel 文件上传方法上传箱内物品信息时可能出现的主要错误。

下表可帮助您认识错误字符串并了解其含义以及发生错误的原因，以便您采取措施来解决问题。

字符串编号 字符串 解读
AGFS_STA_Error_CLIFileUpload_CLI_**Mismatch** Excel 电子表格中提供的箱内物品信息与装箱组的 SKU 不匹配 箱内物品信息中的物品与装箱组中的物品不匹配。例如，如果您上传的已完成文件是用于其他装箱组的，就有可能出现这种情况。
AGFS_STA_Error_CLIFileUpload_**TamperedFile** 上传的文件无效。请使用通过以上链接生成的 Excel 电子表格提供箱内物品信息。 此 Excel 文件是加密的，编辑某些字段时需要输入密码。如果您打开文件所用的不是 Excel 电子表格应用程序，密码保护将被解除。您可以上传没有密码的文件，但是如果您误改了格式，或者上传了不同的文件类型（如 .pdf 或 .csv），您将看到此错误。
AGFS_STA_Error_CLIFileUpload_**ExpectedQuantity_Mismatch** 某些 SKU 的商品总件数与预期数量不符 当箱内商品总件数与预期数量不符时将显示此错误。
AGFS_STA_Error_CLIFileUpload_**InvalidInput** 一个或多个单元格包含无效信息。请更正错误，然后重新上传文件。 当输入的数据格式不正确（例如，为数量、重量或尺寸输入了非数值）时将显示此错误。
AGFS_STA_Error_CLIFileUpload_**BoxWeightMissing** 一个或多个包装箱缺少包装箱重量详情 当一个或多个包装箱缺少包装箱重量值时将显示此错误。
AGFS_STA_Error_CLIFileUpload_**BoxDimensionMissing** 一个或多个包装箱缺少包装箱尺寸详情 当一个或多个包装箱缺少包装箱尺寸值时将显示此错误。
AFGS_STA_Exception_**TryAgain** 出错了。请稍后重试。 这可能是暂时性问题，您可以通过刷新页面或稍后重试来解决。如果错误仍然存在，请联系销售伙伴支持。
亚马逊的卖家助手可以通过此主题提供帮助。对于大多数语言设置，卖家助手还可以直接将您转接至销售伙伴支持。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GX4SH82SZQNYUHCY
