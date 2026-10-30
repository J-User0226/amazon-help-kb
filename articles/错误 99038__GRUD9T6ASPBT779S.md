---
title: "错误 99038"
doc_id: GRUD9T6ASPBT779S
source: https://sellercentral.amazon.com/help/hub/reference/external/GRUD9T6ASPBT779S
language: zh-CN
fetched_at: 2026-10-30T13:50:00
---

# 错误 99038

## 错误消息：

字段 {0} 中包含一个无效值：{}

## 一般信息：

“商品描述”“商品名称”“商品名”“要点”“主要商品特性”等属性中的值带有 HTML 标记。

HTML 标记有一对起止符（<、>），用于定义商品的独特特性和描述。

HTML 标记必须成对使用，以便系统验证标记，否则您将收到错误消息。

仅允许使用的 HTML 标记为：“p”“br”“b”“em”“i”“ol”“ul”“li”和“strong”。

HTML 语句示例：

错误值示例 - 颜色名称：暖白<br/包装内容：<br/>1 个 LED 吊灯<br/>1 个遥控器<br/>1 个配件包<br/>1 本说明书<br/>

正确值示例 - 颜色名称：暖白<br/>包装内容：<br/>1 个 LED 吊灯<br/>1 个遥控器<br/>1 个配件包<br/>1 本说明书<br/>

## 解决错误的步骤：

- 下载上传的模板。

- 检查模板中以橙色高亮显示的受影响的属性。

- 对必要数据使用成对的 HTML 标记，然后重新提交文件，确保提交成功。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GRUD9T6ASPBT779S
