# Amazon 卖家帮助 · 本地知识库

Amazon Seller Central 帮助中心文档的 Markdown 镜像，供 AI agent 检索使用。

## 内容来源

- 站点：`sellercentral.amazon.com`
- 抓取路径：仅 `/help/hub/reference/external/<ID>` 与 `/gp/help/external/<ID>`，即 `robots.txt` 中 `Allow` 的公开路径
- 抓取方式：本地 Chrome 无头模式渲染（页面正文由 JavaScript 生成，直接 HTTP 请求拿不到）
- 语言：简体中文（页面按浏览器语言返回）

## 目录结构

| 文件 | 说明 |
|---|---|
| `INDEX.md` | 总目录，列出全部文章的 ID、标题、字数、官方来源 |
| `CHANGELOG.md` | 每次刷新的结果记录：哪些更新了、哪些没变、哪些失败 |
| `文章标题__<ID>.md` | 单篇文章，文件名即文档 ID（如 `G181.md`） |

每篇文章头部带 front matter：

```yaml
---
title: 账户设置
doc_id: G181
source: https://sellercentral.amazon.com/help/hub/reference/external/G181
language: zh-CN
fetched_at: 2026-10-30 09:04:14
---
```

## 怎么用

- **让 agent 检索**：指向本目录即可。先读 `INDEX.md` 定位文章，再按索引中的文件链接打开正文。
- **核对原文**：每篇末尾都有官方来源链接，正文后附原文出处。
- **新增文章**：
  ```bash
  cd C:/Users/PC018/WorkBuddy/2026-10-28-14-55-46
  python sc_help_refresh.py G181 G200421970
  ```
  已存在则检查更新，不存在则抓取入库。

## 刷新机制

每天 07:30 自动运行 `sc_help_refresh.py`：

1. 逐篇重新抓取；
2. 与本地正文比对（链接中的会话参数不计入差异）；
3. 内容没变 → 文件不动；有变化 → 更新文件；
4. 结果追加到 `CHANGELOG.md`，并提交到本仓库。

抓取失败时保留旧文件，不会破坏已有内容。

## 已知边界

- **登录后才能看到的内容抓不到**（个性化提示、账户相关动态文案）；帮助正文绝大多数在公开版中。
- **页面内嵌视频不收录**，只有文字。
- **文章 ID 无法穷举**（无 sitemap，无效 ID 也返回 200 空壳）。新增文章需要提供具体 ID 或从已有文章的内链中发现。
- 若 Amazon 改版导致正文容器结构变化，抓取会批量失败，会在 `CHANGELOG.md` 中表现为大量 `failed`。

## 版权

文档内容版权归 Amazon 所有。本仓库仅作内部知识库与 agent 检索之用，**请勿对外公开发布或用于商业分发**。若要把仓库公开到互联网，请先评估这一点。

## 文件与覆盖范围

文章采用“标题__文章ID.md”命名；先读 INDEX.md 或 manifest.json。现阶段不代表全量，PENDING.md 列出从已收录文章发现但尚未采集的链接。

## 文件与覆盖范围

文章采用“标题__文章ID.md”命名；先读 INDEX.md 或 manifest.json。现阶段不代表全量，PENDING.md 列出从已收录文章发现但尚未采集的链接。
