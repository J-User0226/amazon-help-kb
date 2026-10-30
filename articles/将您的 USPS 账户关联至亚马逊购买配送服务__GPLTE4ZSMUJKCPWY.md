---
title: 将您的 USPS 账户关联至亚马逊购买配送服务
doc_id: GPLTE4ZSMUJKCPWY
source: https://sellercentral.amazon.com/help/hub/reference/external/GPLTE4ZSMUJKCPWY
language: zh-CN
fetched_at: 2026-10-30 13:47:02
---

# 将您的 USPS 账户关联至亚马逊购买配送服务

## 开通 USPS 账户的前提条件
## 在卖家平台中启动账户关联步骤之前，请按照以下流程操作
请与您的企业账户代表合作，确保他们完成设置。
1. 卖家必须拥有使用 USPS 创建的企业付款账户 (EPA)。
2. 卖家必须注册 USPS Ship（完成第 1 步后即会进入此步骤）。
3. USPS 的账户代表将负责管理用户的协议服务协议 (NSA) 费率。
4. USPS 的账户代表会将用户的 NSA 费率与其企业付款账户关联，以用于 API 费率查询调用。
5. USPS 的账户代表会向买家提供合同编号。

问题 支持
USPS Ship 注册错误 用户的企业账户代表或 [USPSShipSupport@usps.gov](mailto:USPSShipSupport@usps.gov)
USPS 企业付款系统错误 用户的企业账户代表或 [MSSC@usps.gov](mailto:MSSC@usps.gov)
API 响应中未应用 NSA 费率
用户的企业账户代表和 [apisupport@usps.gov](mailto:apisupport@usps.gov)

如果 USPS 团队不确定问题，或想要获取请求响应 JSON，请联系您在 EasyPost 的技术账户管理员。

印戳公司名称错误 用户企业账户代表或 [USPSShipSupport@usps.gov](mailto:USPSShipSupport@usps.gov) 或 [vendor@usps.gov](mailto:vendor@usps.gov)
USPS API 错误 [apisupport@usps.gov](mailto:apisupport@usps.gov)

## 在卖家平台中关联您的 USPS 账户
要关联您的 USPS 账户，请按照以下步骤操作：
1. 前往[购买配送服务首选项](https://sellercentral.amazon.com/sbr/buyShippingPreferences)，然后选择【管理您的承运人账户】。
2. 点击【关联】，选择 【USPS 模块】，然后输入在 USPS 发票的【配送地址】部分显示的以下信息。除非另有说明，否则所有字段均为必填字段。您可能希望向您的 USPS 代表确认具体详情。
  1. 账号
  2. 买家注册编号 (CRID)
  3. 发件人编号
  4. 货单编号（如果承运人未提供，则该编号将与发件人编号相同）

3. 阅读并同意 USPS 最终用户协议，然后点击【下一步】，您将跳转至 USPS 网站进行账户验证。
4. 输入您的 USPS.com 用户名或电子邮件和账户密码，然后按照提示完成验证过程。

在[管理您的承运人账户](https://sellercentral.amazon.com/carrier-preferences/main)，您会看到【承运人优先次序】部分中 USPS 旁边显示【已关联】状态。

如果您有多个库房或位置，请联系 USPS，了解您必须使用哪个邮政编码（取件地点）进行验证。 **Warning： **混用邮政编码和账户邮政编码有时会导致【管理您的承运人账户】页面上出现错误。验证您在表单中输入的编码并重新提交。

## 通过亚马逊“购买配送服务”购买货件标签
在您的账户与卖家平台关联后，您就可以通过卖家平台上的“购买配送服务”功能、Veeqo、多渠道集成商和 API，使用您与承运人协商的费率购买 USPS 标签。

通过亚马逊“购买配送服务”购买货件标签，可享受准时送达率保护和配送相关索赔的退款。

关联您的 USPS 账户后，您将继续由 USPS 进行账单结算，并且通过亚马逊购买配送服务购买的标签将计入您与 USPS 达成的最低发货量要求。

您还可以灵活地关联多个 USPS 账户，并将其分配到不同的位置。

关联您的承运人账户后，您可以通过亚马逊购买配送服务从卖家平台的[管理订单](https://sellercentral.amazon.com/orders-v3/?shipByDate=all)页面或我们的[配送 API](https://developer-docs.shipping.amazon.com/apis/docs/shipping-api-v2-reference) 购买货件标签，也可以使用 [Veeqo](https://www.veeqo.com/) 或[其他多渠道集成商](https://sellercentral.amazon.com/gp/help/external/GZZPMC9QLNBX48RP)作为您的首选渠道

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GPLTE4ZSMUJKCPWY
