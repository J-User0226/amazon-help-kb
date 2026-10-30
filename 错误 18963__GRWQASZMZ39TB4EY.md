---
title: 错误 18963
doc_id: GRWQASZMZ39TB4EY
source: https://sellercentral.amazon.com/help/hub/reference/external/GRWQASZMZ39TB4EY
language: zh-CN
fetched_at: 2026-10-30 13:50:02
---

# 错误 18963

## 错误消息
匹配已找到的候选 ASIN，但无法进一步缩小其范围：${candidateAsins}。原因：{reason}。

## 导致错误 18963 的原因
导致此错误的原因如下：
- 在尝试创建新的商品信息时，系统会找到多个具有类似商品属性（商品名称、品牌、制造商和款式编号等）的现有 ASIN。
- 在批量上传操作中，提供的商品编码不够具体，无法确切指向某一个 ASIN。
- 由于商品信息不完整或含糊不清，提交的商品数据与亚马逊目录中的多个 ASIN 匹配。
- 在目录匹配过程中，算法无法根据提供的商品详情准确选中某一个 ASIN 而非其他 ASIN。

## 解决错误 18963
要解决此错误，请按照以下步骤操作：
1. 查看错误 ASIN 的上传数据处理汇总报告。
2. 为您的商品添加唯一商品编码，如 UPC、EAN、ISBN 或制造商部件编号，以帮助系统识别您的特定商品。
3. 使用更详细和独特的信息更新您的商品信息，例如有助于区分您的商品与类似商品的特定型号、独特商品特性、准确尺寸、重量或制造商部件编号。
4. 如果您可以确定哪些候选的 ASIN 正确表示您的商品，则您可能需要在提交商品信息时手动选择或指定该 ASIN，而不是依靠自动匹配。
5. 重新提交上传数据文件。

---

原文出处：https://sellercentral.amazon.com/help/hub/reference/external/GRWQASZMZ39TB4EY
