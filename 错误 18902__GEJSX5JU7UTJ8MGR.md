---
title: 错误 18902
doc_id: GEJSX5JU7UTJ8MGR
source: https://sellercentral.amazon.com/help/hub/reference/external/GEJSX5JU7UTJ8MGR
language: zh-CN
fetched_at: 2026-10-30 13:31:33
---

# 错误 18902

## 错误消息
此报价因发票被拒而被冻结，原因是 GTIN (cEAN) 与 NCM 或 CEST 代码不兼容。更新上述属性之一。更新完毕后，请点击此处了解如何解锁您的商品。${url}

## 导致错误 18902 的原因
出现此错误的原因如下：
- 商品信息中提交的全球贸易项目代码 (GTIN) 或欧洲商品编码 (EAN) 与巴西商城合规性所要求的 Nomenclatura Comum do Mercosul (NCM) 税务分类代码不一致，导致发票验证系统拒绝该报价。（例如，为手机使用 GTIN“7891234567890”分类为 NCM 代码“8517.12.31”的商品，但该 GTIN 在制造商数据库中注册为归属于 NCM 代码“8544.42.00”下的电子产品配件等不同商品分类。）
- 用于标识巴西需要进行税务替代的商品的 Código Especificador da Substituição Tributária (CEST) 代码与 GTIN 或 EAN 指示的商品类型不匹配，导致在财务验证过程中发票被拒。
- 商品信息中完全缺少有效的 NCM 代码，包含已弃用的 NCM 代码，格式错误（少于 8 位数），或者与根据巴西税务机构数据库中的 GTIN 验证的实际商品分类不符。
- 通过库存文件或 API 集成上传的多个商品包含系统错误，其中 GTIN、NCM 代码或 CEST 代码映射不正确，从模板中复制了错误的值，或者自动填充了与实际商品规格不符的默认代码。

## 解决错误 18902
要解决此错误，请按照以下步骤操作：
1. 导航至卖家平台，然后依次选择库存和管理所有库存，找到冻结的商品，点击编辑，访问合规性或税务信息部分，根据巴西联邦税务局 (Receita Federal) 网站上提供的官方 NCM 分类表验证当前 NCM 代码，使用准确代表商品分类的正确 8 位代码更新 NCM 字段，保存更改，并等待 24~48 小时，以便系统根据发票要求重新验证报价。
2. 通过交叉引用 [gs1.org](http://gs1.org) 或 [gs1br.org](http://gs1br.org) 上的 GS1 数据库验证您商品信息中输入的 GTIN 或 EAN 是否与商品包装上实际打印的条形码匹配，确保 GTIN 与正确的商品变体（包括尺寸、颜色和包装规格）对应，如果发现差异，请更新 GTIN 字段。
3. 查看商品分类的 CEST 代码要求，以确定您的商品是否需要进行税务替代 (Substituição Tributária) 以及是否需要提供 CEST 代码。
4. 更新所有必填属性（GTIN、NCM 和 CEST 代码）后，点击错误消息中提供的 URL 链接 (${url}) 以访问报价取消冻结请求页面，按照说明提交取消冻结请求，并提供显示更正后的商品信息的文件。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GEJSX5JU7UTJ8MGR
