# OPC 项目总览

> 公开版说明：本仓库只保留项目经历证明需要的脱敏材料。原始本机路径、聊天原文、日志、音频、模型、API 返回和凭证均不入库。

# OPC 项目阶段性总览（2026-03 以来）

生成时间：2026-06-16  
口径：先不给简历表/素材表写入，只把从 macmini、本机、Codex session、OPC 文件系统和 GitHub 侧能扒到的项目线索列出来。

## 当前结论

1. OPC 相关项目主证据不在 GitHub 仓库里，而是在本机/mini 的文件包、Figma Make 前端包、证据库、XMind、H5、Excel、docx、Codex session 里。
2. macmini 可通过 `ssh codex-mini` 持久访问，实际主机是 `OscardeMac-mini.local`；`mini` 这个 mDNS alias 不稳定。
3. macmini 上高相关目录里只有 4 个本地 Git 仓库，其中属于你 GitHub remote 的只有 `Jiangziya`；OPC 目录没有发现独立 `.git` 仓库。
4. GitHub 公共 API 查到 `zixuouoscaroliver` 账号公开仓库 4 个，更新时间都在 2026-02，不属于 2026-03 以来 OPC 项目。
5. 私有 GitHub 目前没法全量扒：GitHub connector 读 `private-repo-redacted` 返回 404；macmini 的 HTTPS 会要求用户名；macmini 的 `[email-redacted]` 返回 `Permission denied (publickey)`。

## 已整理出的 OPC 项目组（20项）

1. OPC 证据库索引/状态表
2. OPC 系统需求总包
3. 平台配置 / 平台配置 Copy 工作区与前端包
4. 招商授权 / 代理审核 / 平台代理授权
5. 供应商管理 / 供应商分润 / 商品招商链路
6. 营销推广 / 推客系统
7. 上架配置中心 / 上架配置迁移
8. 代理商 / 招商人员分润配置
9. OPC 租户关系 / 商品招商链路可视化
10. OPC 全量图 / 五条流业务逻辑 / 业务架构
11. 收单逻辑 / 订单履约 / CPS 履约
12. OPC 合规法规梳理
13. Figma 前端包 / 五包规划对比
14. 彬彬姐 FigmaMake 前端包拆解工作流模板
15. OPC 知识库 / Graphify / 工作台 H5
16. OPC 董事长诊断端 / 工作流优化
17. Figma Make 每日增量聊天快照 / 版本归档
18. OPC 证据库自动化 / 董事长诊断端
19. Figma Make 六个工作区规则 / OPC 全局规则
20. 彬彬姐上线功能 / 开发进度判断

详细证据见：`OPC项目组视图_20项_20260616.md`

另有一版更适合人工快速浏览的分层地图：`OPC项目地图_分层版_20260616.md`。这一版把项目拆成业务产品、Figma/前端包、证据库自动化、可视化/知识库、沟通研究、GitHub 六层。

## GitHub / Git 仓库侧

### macmini 高相关目录本地 Git 仓库

| 路径 | 分支 | remote | 判断 |
|---|---:|---|---|
| `[local-path-redacted]` | `main` | `https://github.com/private-repo-redacted.git` | 你的 GitHub 项目，但当前无远程读取权限 |
| `[local-path-redacted]` | `main` | 空 | 本地 git，无 GitHub remote |
| `[local-path-redacted]` | `main` | 空 | 本地 git，无 GitHub remote |
| `[local-path-redacted]` | `master` | `https://github.com/ggerganov/whisper.cpp.git` | 第三方依赖仓库 |

### `zixuouoscaroliver` 公开仓库

| 仓库 | 最近更新时间 | 语言 | 判断 |
|---|---:|---|---|
| `Oscar-Oliver` | 2026-02-20 | TypeScript | 早于 2026-03，非 OPC |
| `tailscale-link-viewer` | 2026-02-20 | TypeScript | 早于 2026-03，非 OPC |
| `gaokao-index-pages` | 2026-02-15 | JavaScript | 早于 2026-03，非 OPC |
| `Oscar-Oliver-beta` | 2026-02-15/20 | Python | 早于 2026-03，非 OPC |

## 输出文件

- `OPC项目组视图_20项_20260616.md`：20 个项目组的详细证据样例。
- `OPC项目候选清单_初扒_20260616.md`：更宽松的 104 个候选线索。
- `macmini_current_opc_sessions.tsv`：macmini 当前 Codex session 里 74 条 OPC 相关记录。
- `opc_relevant_codex_sessions.tsv`：本机/导入 session 索引里 165 条 OPC 相关记录。
- `opc_relevant_files.tsv`：文件系统证据采样 2000 条。
- `macmini_opc_session_evidence.tsv`：从 macmini Codex session 原文抽出的 116 条证据，包含用户请求、最后结论、产物路径。
- `OPC项目地图_分层版_20260616.md`：按业务/自动化/交付物重新分层后的人工阅读版。
- `OPC功能模块清单_20260616.md`：按业务域拆开的功能模块清单，包含平台配置、招商代理、供应商、分润、营销推广、CPS履约、自动化、飞书同步等模块。
- `GitHub与代码项目清单_20260616.md`：公开 GitHub 仓库、本地 git 项目、私有 remote 可访问性与 OPC 关系判断。
- `macmini_documents_git_remotes.tsv`：macmini 高相关目录 Git 仓库 remote 表。
- `github_public_repos_zixuouoscaroliver.tsv`：GitHub 官方公开 API 返回的公开仓库。
- `github_access_checks_20260616.tsv`：GitHub/SSH/本地 clone 访问检查记录。
- `目标完成度审计_20260616.md`：逐项说明哪些要求已证明完成、哪些仍被 GitHub 私有认证阻塞。

## 仍未完成

私有 GitHub 全量仓库没有被证明完成。要继续往下扒，需要至少一种可用路径：

- 在 macmini 配好 GitHub SSH key，确保 `ssh -T [email-redacted]` 能显示已认证；
- 或在 macmini / 本机安装并登录 `gh`，确保 `gh repo list zixuouoscaroliver --limit 200` 可用；
- 或把 GitHub connector 授权到包含私有仓库的账号/组织。

在这个权限补齐前，OPC 主线已经能从本地和 macmini 文件证据继续整理，但不能声称“GitHub 私有库已全量扒完”。
