# OPC 项目案例库

公开工程证据库：OPC 项目经历、业务拆解、Figma Make 协同、证据库自动化、H5 Demo、成就素材库、迭代失败复盘和时间戳证明。

## 项目一句话

这个仓库把 2026-03 到 2026-06 的 OPC 项目工作，从分散的 Figma Make 包、H5、Excel、XMind、项目盘点和本地证据，整理成一个可公开检查的 GitHub 作品集。

## 为什么这个项目不只是“整理文件”

- 原始工作区约 3.7GB，混有临时目录、录音、模型、日志、截图包和私有证据，不能直接公开。
- OPC 主证据不在一个干净 GitHub 仓库里，而是分散在本地文件、Figma Make 包、证据库、H5、Excel 和 Codex session 派生材料里。
- 公开版既要证明项目经历，又不能泄露本机路径、私有仓库、原始聊天、API 结果、字段 ID 和大文件。
- 过程中出现过真实失败：宽扫卡顿、GitHub 私有证据不可验证、Excel 源路径泄露风险、Pages 构建 404、提交作者信息暴露本机身份等。这些都记录在失败复盘里。

## 三个入口

- [GitHub Pages 展示页](https://zixuouoscaroliver.github.io/opc-project-casebook/)
- [OPC 项目地图](casebook/01-project-map.md)
- [成就素材库公开版](resume-assets/achievement-library.md)
- [OPC 直接利益测算](resume-assets/opc-business-impact.md)
- [失败复盘与迭代过程](docs/failure-review.md)
- [时间戳证明](evidence/timestamped-proof.md)

## 我在这个项目里做了什么

- 把 OPC 复杂业务拆成租户、渠道、商品、供应商、分润、履约、证据链和诊断工作流。
- 把会议、XMind、Figma Make 前端包、截图 OCR、Excel、Codex session 里的材料整理为可追踪的项目资产。
- 输出业务模块、页面规划、Figma Make 喂数规则、每日增量同步、诊断端、Skill 工作流和 H5 展示。
- 把可公开部分整理成作品集，移除原始聊天、音频、日志、凭证、本机路径和大文件。

## 仓库结构

| 目录 | 内容 |
|---|---|
| `casebook/` | 项目总览、项目地图、功能模块、代码/GitHub 关系、个人贡献映射 |
| `docs/` | GitHub Pages、PRD、架构、数据模型、工程原则、实现说明、运行手册、失败复盘、简历证明 |
| `evidence/` | 时间线、时间戳证明、指标快照、发布验证 |
| `evidence-index/` | 第一版脱敏证据索引与公开边界说明 |
| `resume-assets/` | 成就素材库公开版，含 `.xlsx`、Markdown、CSV 和收益测算说明 |
| `src/` | 公开源代码边界说明；真实私有运行源不直接公开 |
| `config/` | 公开发布边界和校验策略 |

## 建议阅读顺序

1. 先看 [GitHub Pages 展示页](https://zixuouoscaroliver.github.io/opc-project-casebook/)。
2. 再看 [项目地图](casebook/01-project-map.md) 和 [功能模块清单](casebook/02-function-modules.md)。
3. 如果想看工程判断，看 [架构](docs/architecture.md)、[实现说明](docs/implementation-notes.md)、[失败复盘](docs/failure-review.md)。
4. 如果想验证真实性，看 [时间戳证明](evidence/timestamped-proof.md)、[指标快照](evidence/metrics-snapshot.json)、[发布验证](evidence/publication-validation.md)。
5. 如果要写简历，看 [成就素材库公开版](resume-assets/achievement-library.md)、[OPC 直接利益测算](resume-assets/opc-business-impact.md) 和 [简历证明叙事](docs/resume-proof.md)。

## 公开边界

这个仓库不是 OPC 原始资料全量备份。以下内容不会进入公开仓库：

- `transcripts/`、`tmp/`、音频、模型、日志、临时文件。
- 原始 Feishu/API JSON、字段 ID、聊天原文、会议转录。
- 私有仓库地址、本机绝对路径、凭证、手机、邮箱。
- 大 zip 原包和完整证据库镜像。

## 代表产物

- 20 项 OPC 项目/产物组整理。
- 14 个业务域功能模块清单。
- 多个可浏览 H5 Demo。
- 34 条公开版成就素材，可直接服务简历、面试和作品集表达。
- 公开收益口径：把证据检索、session 盘点、商品 AI 优化和 Figma Make 上下文治理转成可解释的时间/成本节约测算，同时标明不能硬写的收入和客户增长边界。
- 13 条真实迭代失败与经验复盘。
- 发布验证记录：公开仓库、Pages 状态 `built`、首页与 Demo HTTP 200、敏感信息扫描、Excel XML 扫描。
