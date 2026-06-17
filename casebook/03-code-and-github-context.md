# 代码与 GitHub 关系说明

> 公开版说明：本仓库只保留项目经历证明需要的脱敏材料。原始本机路径、聊天原文、日志、音频、模型、API 返回和凭证均不入库。

# GitHub 与代码项目清单（阶段版）

生成时间：2026-06-16  
口径：根据 GitHub 公开 API、macmini 高相关目录 `.git` 扫描、本机/macmini 可见目录结构整理。私有 GitHub 远程未打通，因此本清单把“能读到什么”和“读不到什么”分开写。

## 结论

1. `zixuouoscaroliver` 公开 GitHub 仓库只有 4 个，最近更新时间都在 2026-02，不属于 2026-03 以来 OPC。
2. macmini/本机高相关目录里发现 4 个本地 git 项目，其中只有 `jiangziya-oem-work` 指向你的 GitHub remote `private-repo-redacted`。
3. OPC 没有发现独立 GitHub 主仓库或本地 `.git` 仓库；OPC 主证据仍是文件包、Figma Make、飞书、证据库和 Codex session。
4. `Jiangziya` 是本地结构最完整的私有代码项目，但当前远程不可读；从目录结构看，它是「姜子牙 OEM / 起名 Agent 平台」项目，不是 OPC 主项目。

## A. GitHub 公开仓库

| 仓库 | 更新时间 | 语言 | 地址 | 判断 |
|---|---:|---|---|---|
| `Oscar-Oliver` | 2026-02-20 | TypeScript | `https://github.com/zixuouoscaroliver/Oscar-Oliver` | 新闻自动发送相关，非 OPC |
| `tailscale-link-viewer` | 2026-02-20 | TypeScript | `https://github.com/zixuouoscaroliver/tailscale-link-viewer` | Tailscale 链接查看器，非 OPC |
| `gaokao-index-pages` | 2026-02-15 | JavaScript | `https://github.com/zixuouoscaroliver/gaokao-index-pages` | GitHub Pages index，非 OPC |
| `Oscar-Oliver-beta` | 2026-02-15/20 | Python | `https://github.com/zixuouoscaroliver/Oscar-Oliver-beta` | Telegram/news pusher beta，非 OPC |

证据文件：`github_public_repos_zixuouoscaroliver.tsv`、`github_public_repos_zixuouoscaroliver_raw.json`

## B. macmini / 本机本地 git 项目

### B1. `jiangziya-oem-work`

- 本地路径：`[local-path-redacted]`
- remote：`https://github.com/private-repo-redacted.git`
- 分支：`main`
- 当前远程访问：不可读
  - GitHub connector：404
  - HTTPS：要求 Username
  - SSH：`Permission denied (publickey)`
- 本地结构线索：
  - Go 后端：`go.mod`、`cmd/oem-server`、`internal/oem`、`internal/jiangziya`
  - Vite/前端：`frontend/package.json`、`frontend/src`、`frontend/vite.config.ts`
  - 管理后台/设计：`design/admin-dashboard`、`design/figma-make-kit`、`design/figma-skill-upload`
  - OEM/NAS 交付：`deploy/nas`、`dist/nas-partner-access*`、`README_OEM_H5.md`、`SEND_TO_PARTNER_README.md`
  - 起名 Agent V2：`docs/NAMING_AGENT_V2_PRD.md`、`frontend-variants/naming-v2-*`
  - QA/部署输出：`output/ui-qa-*`、`dist/deploy-*`
- 本地 Git 轻量历史线索：
  - `.git/logs/HEAD` 最近 30 条本地提交时间集中在 2026-05-13 到 2026-05-26。
  - 提交主题集中在 `shadow naming agent lab`、`Core naming lab`、`NAS deploy`、`lab naming fallback`、`Jiangziya agent manifests`、`v8.3 bazi verification flow`、`DeepSeek provider/backend`、`V10 frontend`、`Figma package` 等。
  - `git log --since=2026-03-01` 与最近 20 条 `git log` 在当前镜像目录上会超时，因此没有把它当作完整历史证明。
- OPC 关键词检查：
  - 对关键源码/文档路径用 `OPC|平台配置|供应商|分润|上架|招商|代理|营销|推客|CPS|收单|履约|租户|渠道|经销商` 搜索，稳定输出为 0 条。
  - 对项目自身关键词 `姜子牙|起名|命理|OEM|NAS|Figma` 搜索，命中文档集中在 Figma kit、NAS 部署、Naming Agent PRD、frontend variants。
- 初步判断：这是「姜子牙 OEM / 起名 Agent 平台 / NAS 交付 / Figma Make 设计包」项目。它和 OPC 的共同点是都用了 Figma Make / Codex / OEM 化交付方法，但不是 OPC 业务项目。

### B2. `SignalDesk`

- 本地路径：`[local-path-redacted]`
- remote：空
- 分支：`main`
- 判断：本地 git 项目，没有 GitHub remote；当前未发现 OPC 证据。

### B3. `WhisperScribe`

- 本地路径：`[local-path-redacted]`
- remote：空
- 分支：`main`
- 判断：本地 git 项目，没有 GitHub remote；从名称和目录看更像语音/转录工具项目，可辅助 OPC 会议转录，但不是 OPC 主项目。

### B4. `whisper.cpp`

- 本地路径：`[local-path-redacted]`
- remote：`https://github.com/ggerganov/whisper.cpp.git`
- 分支：`master`
- 判断：第三方依赖仓库，不计入你的项目。

证据文件：`macmini_documents_git_remotes.tsv`、`local_documents_git_remotes.tsv`、`jiangziya_key_files.txt`、`jiangziya_git_head_reflog_tail.txt`、`jiangziya_project_keyword_files.txt`、`jiangziya_opc_keyword_hits.tsv`

## C. 和 OPC 的关系判断

| 项目 | 与 OPC 的关系 | 可否放入 OPC 简历素材 |
|---|---|---|
| OPC 文件包/证据库/Figma Make 自动化 | 直接相关 | 可以，主线 |
| `Jiangziya` | 方法论/技术栈类似，但业务不同 | 可以作为 AI OEM/Agent 平台单独经历，不应混进 OPC |
| `WhisperScribe` | 可能辅助会议转录 | 可作为工具能力背景，不应写成 OPC 项目 |
| `SignalDesk` | 未发现 OPC 关系 | 暂不放 |
| 4 个公开 GitHub 仓库 | 早于 2026-03，非 OPC | 暂不放 |

## D. 仍需权限补齐的地方

要真正完成“GitHub 私有库全量扒取”，还需要至少一种可用认证方式：

- macmini 上 `gh auth login`，然后可跑 `gh repo list zixuouoscaroliver --limit 200 --json name,visibility,updatedAt,pushedAt,url,description`;
- 或 macmini 的 GitHub SSH key 加到账户，确保 `ssh -T [email-redacted]` 认证成功；
- 或 GitHub connector 授权到包含私有仓库的账号/组织。

在这些条件满足前，不能证明私有 GitHub 已全量覆盖。
