# OPC 功能模块清单

> 公开版说明：本仓库只保留项目经历证明需要的脱敏材料。原始本机路径、聊天原文、日志、音频、模型、API 返回和凭证均不入库。

# OPC 功能模块清单（2026-03以来）

生成时间：2026-06-16  
口径：从 `OPC项目地图_分层版_20260616.md`、`opc_project_candidates.tsv`、`macmini_opc_session_evidence.tsv`、macmini output 目录与 OPC 文件系统证据归纳。  
说明：旧证据库里的 `package_function_index.json` / `function_package_index.json` 文件存在且大小正常，但本轮从原路径读取内容时文件系统会等待，因此本清单暂不声称完全复刻索引 JSON，只做基于已稳定证据的功能模块归档。

## 1. 平台配置 / 上架配置中心

证据强度：高  
对应项目：`上架配置中心/上架配置迁移`、`平台配置 / 平台配置 Copy 工作区与前端包`

已扒到的模块：

- 上架配置中心整体架构
- 待配置商品
- 组合套餐
- 组合产品门槛配置
- 招商授权 Tab
- 我的上级商品池
- 我的在售/可经营商品
- 开放给下级
- 下级可见结果
- 商品卡黑黄视觉体系
- 待发布卡 / P5 按钮条
- 上架配置中心五 Tab 修正版规划
- Copy 进货侧上架配置弹层
- 不展示供应商信息修正口径
- 平台配置 Copy 上架配置迁移

核心证据：

- `output/上架配置中心_v7整体业务架构逻辑.md`
- `output/上架配置中心_架构文档.md`
- `output/上架配置逻辑文档_vs_v3页面差异清单.md`
- `output/上架配置组合产品门槛配置对比.md`
- `output/figma-make-migration/平台配置Copy上架配置迁移到平台配置_差异清单与Make指令.md`
- macmini session `上架配置`：2026-06-03 针对 `平台配置 6.3` 招商授权 Tab 输出 Figma Make 修复指令。

## 2. 招商授权 / 渠道代理 / 经销商审核

证据强度：高  
对应项目：`招商授权/代理审核/平台代理授权`、`OPC PC 后台`

已扒到的模块：

- 平台代理授权
- 品牌方授权平台方
- 平台授权代理商
- 招商授权设置
- 代理管理
- 代理审核
- D1-D5 渠道代理体系
- 经销商审核
- 生态管理 / SAAS 节点管理
- `/eco/dealers`
- `/eco/supply-chain/dealers`
- 邀请码 / 注册链接 / 绑定关系
- 上下级关系
- 渠道可见范围

核心证据：

- `output/招商授权设置方案_建议版.md`
- `output/招商授权设置方案_业务逻辑版.md`
- `output/品牌方授权平台方_平台代理授权代理商_业务逻辑与调整方案.md`
- `output/代理管理代理审核一条龙规划与RP图.md`
- `output/figma-upload-docs/D1-D5渠道代理体系说明_Figma上传版.md`
- macmini session `OPC PC 后台`：判断 `/eco/dealers` 不是经销商审核主页面，真正相关的是 `/eco/supply-chain/dealers`。

## 3. 供应商管理 / 商品招商链路

证据强度：高  
对应项目：`供应商管理/供应商分润/商品招商链路`

已扒到的模块：

- 供应商管理
- 供应商体系完整架构
- 供应商模块精简重构
- 供应商分润
- 商品招商链路
- 商品中心
- 商品上下架
- 商品卡列表
- 活动申报
- 供应商、招商角色、经销商、达人、推客的角色链路
- 商品归属与项目归属
- 商品经营权限

核心证据：

- `[opc-evidence-path-redacted]`
- `OPC 快照/5.13/平台配置/供应商体系完整架构规划.md`
- `OPC 快照/5.13/平台配置/供应商模块精简重构方案.md`
- `OPC 快照/5.13/平台配置/PLAN_方案B_平台模式与分润配置统一设计方案.md`
- 2026-03-30 session：供应商管理三版本功能差异与逻辑缺口。

## 4. 分润配置 / 收益规则

证据强度：高  
对应项目：`代理商/招商人员分润配置`

已扒到的模块：

- 分润模板管理
- 招商分润配置
- 代理商分润配置
- 招商人员分润
- 商品分润比例
- 特殊商品分润
- 非默认商品逻辑
- 层级分润系数
- 平台 / 招商 / 销售分润口径
- 7 列分润矩阵
- 企微共享文档版
- 参数注解与案例说明

核心证据：

- `output/代理商分润配置文档/01_代理商分润配置_业务逻辑与需求文档.md`
- `output/代理商分润配置文档/02_代理商分润配置_页面设计与业务逻辑方案.md`
- `output/代理商分润配置文档/03_代理商分润配置_参数注解与案例说明.md`
- `OPC_平台配置_分润配置逻辑_企微共享文档版.docx`
- macmini session `分润配置逻辑导出`：已转为可上传/可编辑 Word，含 19 张表和 7 列矩阵。
- macmini session `特殊商品分润`：定位特殊商品逻辑在招商分润配置等文档内。

## 5. 营销推广 / 推客系统

证据强度：高  
对应项目：`营销推广/推客系统`

已扒到的模块：

- 推客系统 V1
- 知识付费专区
- 视频号推客中心
- 小程序查看器
- 推客配置
- 项目切换
- 登录页
- 入驻页
- 个人中心
- 导航重构
- 任务大厅
- 素材中心
- 商业模式相关文档
- 商品分发 / 内容分发

核心证据：

- `[opc-evidence-path-redacted]`
- `[opc-evidence-path-redacted]`
- `[opc-evidence-path-redacted]`
- `OPC 快照/5.13/营销推广/*`
- 2026-05-18 session：比对 5.13 与 5.16 营销推广文档，抽出 `_商业模式相关文档`。

## 6. 收单 / 订单 / CPS 履约

证据强度：中  
对应项目：`收单逻辑/订单履约/CPS 履约`

已扒到的模块：

- 收单渠道
- 收单渠道重构
- 订单履约
- CPS 链路
- 知识付费与微信 CPS
- 货品上架
- 云仓提货
- 物流
- 财务收益闭环
- 可测试状态节点
- 验收口径

核心证据：

- `output/收单逻辑架构文档.md`
- `OPC 快照/5.13/平台配置（copy）/收单渠道重构完成.md`
- `_10_当前工作区/文档/CPS 链路.md`
- `_90_收件箱/Downloads_20260429/OPC 总览规划表_知识付费与微信CPS_高亮版.xlsx`
- 2026-03-30 session：重写货品上架、云仓提货、物流、财务收益闭环的状态流和验收。

## 7. OPC 租户 / 五条流 / 总体业务架构

证据强度：高  
对应项目：`OPC 租户关系/商品招商链路可视化`、`OPC 全量图/五条流业务逻辑/业务架构`

已扒到的模块：

- OPC 租户
- 商品招商链路
- 人流
- 物流
- 单流
- 财流 / 收益流
- 信息流 / 任务流
- 角色进入系统
- 角色归属和上下级关系
- 企微 / SCRM 执行建群、拉群、触达
- 注册成功 / 绑定成功 / 入群成功 / 异常回流
- 全量图
- 四包最佳页面汇总
- 已完成前端页面路径筛选

核心证据：

- `_10_当前工作区/文档/OPC 租户 @商品招商链路.md`
- `_10_当前工作区/导图/OPC 租户_四包最佳页面汇总.xmind`
- `_10_当前工作区/导图/OPC 租户_已完成前端页面路径_筛选版.xmind`
- `output/opc_tenant_ecosystem_h5_20260516.html`
- `output/opc_tenant_radial_graph_h5_20260516.html`
- `output/opc_tenant_relation_graph_h5_20260516.html`
- `output/opc_graphify_logic_h5_20260516.html`

## 8. Figma Make 工作区 / 前端包协同

证据强度：高  
对应项目：`Figma Make 六个工作区规则/OPC 全局规则`、`Figma 前端包/五包规划对比`

已扒到的模块：

- OPC 全局规则
- 平台配置工作区规则
- 平台配置 Copy 工作区规则
- 营销推广工作区规则
- 日常运营工作区规则
- 供应商管理工作区规则
- C 系统版本工作区规则
- 五包对比总览
- 包级规划对比清单
- FigmaMake 喂数规则
- 前端包原始 MD
- Figma 上传文档

核心证据：

- `output/figma-make-skills/00_OPC全局规则.md`
- `output/figma-make-skills/01_平台配置工作区规则.md`
- `output/figma-make-skills/02_平台配置_Copy工作区规则.md`
- `output/figma-make-skills/03_营销推广工作区规则.md`
- `output/figma-make-skills/04_日常运营工作区规则.md`
- `output/figma-make-skills/05_供应商管理工作区规则.md`
- `output/figma-make-skills/06_C系统版本工作区规则.md`
- `output/figma-package-comparison/00_五包对比总览.md`
- `output/figma-package-comparison/01_平台配置_规划对比清单.md` 等。

## 9. Figma 设计链路协同 / PM 判断看板

证据强度：中高  
对应项目：`Figma设计链路协同试用表/包级变更总控`

已扒到的模块：

- 包级修改总览
- 每包改了哪些页面
- 页面节点
- 修改内容摘要
- 变更类型
- PM 判断
- PM 判断理由
- 回退/改进动作
- 关联版本号
- 是否当前版本
- 04 Figma 新旧对比与 PM 确认
- 05 版本变更沉淀
- 待 PM 判断清单
- 需回退改进清单
- 可分发清单
- 已分发清单
- PM 判断分布图

核心证据：

- macmini session `看板Figma设计链路协同试用表`：2026-06-04。
- macmini session `figma 设计链路协同`：2026-06-03。

## 10. 每日增量抓取 / 证据库自动化

证据强度：高  
对应项目：`Figma Make 每日增量聊天快照/版本归档`、`OPC 证据库自动化/董事长诊断端`

已扒到的模块：

- `run_daily_opc_sync`
- `collect_figma_chats`
- Figma 聊天记录自动扒取
- 页面截图与 OCR
- 版本 checkpoint
- `chat.txt`
- `raw_messages.json`
- `ocr.txt`
- `screenshot.png`
- `meta.json`
- `capture_manifest_versions.csv`
- `_index/packages.csv`
- `_index/failures.csv`
- `_index/update_log.md`
- `_runs/.../scrape_summary.md`
- codeSnapshotKey 去重与 makeVersionId 归属
- 原始完整包短期保留
- 精简前端包

核心证据：

- `macmini_opc_session_evidence.tsv` 里 2026-05-19 到 2026-05-29 的每日增量 run。
- 成功数线索：3、0、6、13、13、11、39、25、49 等。
- `[opc-evidence-path-redacted] 快照/FigmaMake聊天记录/_runs/...`
- `OPC证据库_旧位置备份_20260517_164930/09_自动化运行日志/*`

## 11. 飞书同步 / 证据落档

证据强度：中高  
对应项目：`飞书 Base 02/04 自动同步`

已扒到的模块：

- `02 当日信息自动采集`
- `04 当日页面功能点基于 02 的变化`
- Figma 前端包附件字段
- 现版本文件附件字段
- `sync_feishu_base_02_04.ts`
- `analyze_daily_evidence.ts`
- `run_daily.sh`
- 飞书云空间存文件
- 飞书多维表格存索引/状态/链接/董事长确认
- 同步日志
- 失败项下次补跑

核心证据：

- macmini session `OPC 每日抓取落档对比`：2026-06-04。
- `github_access_checks_20260616.tsv` 和 `macmini_opc_session_evidence.tsv` 里的同步脚本路径。

## 12. 董事长诊断端 / 确认口径

证据强度：高  
对应项目：`OPC 董事长诊断端/工作流优化`

已扒到的模块：

- 董事长 Codex OPC 诊断端
- 离线最小包
- 离线一键包
- 干净环境安装
- 主动诊断 skill
- `md_conflict_pool`
- 董事长确认记录
- 确认版 MD
- 按包诊断
- 按功能诊断
- 做到哪了
- 下一步调什么
- 能不能做
- 要不要本期做

核心证据：

- `opc-evidence-automation/OPC董事长诊断端_离线最小包_干净环境版_v2_20260517.zip`
- `opc-evidence-automation/OPC董事长诊断端_离线一键包_20260517.zip`
- `PROMPT_发给董事长Codex执行.md`
- `README_董事长电脑干净环境安装.md`
- `skills/chairman-opc-diagnosis/`

## 13. 可视化 / 知识库 / 工作台

证据强度：中高  
对应项目：`OPC 知识库/Graphify/工作台 H5`

已扒到的模块：

- OPC 工作台 H5
- Graphify OPC 知识库
- 租户生态 H5
- 放射关系图
- 拖拽聚焦截图
- 移动端/桌面端截图
- 方法论 summary

核心证据：

- `output/知识库与OPC工作台_H5_20260516.html`
- `output/graphify-opc-knowledge-v0/01_knowledge_v0_no_jiangziya.md`
- `output/graphify-opc-knowledge-v0/02_opc_workbench_methodology_summary.md`
- `output/h5-screenshots/*`

## 14. 合规 / 会议 / 项目沟通

证据强度：中  
对应项目：`OPC 合规法规梳理`、`OPC 业务梳理与排期/开发对齐`

已扒到的模块：

- OPC 法律法规合规合法化
- 青岛团队开发节奏对接
- 当前已做页面/模块梳理
- 卡点收集
- 问题绑定页面/模块/负责人
- 产品未定 / 技术问题 / 设计问题 / 资料问题区分
- 飞书知识库总规划页
- 功能索引多维表
- 功能业务逻辑文档库
- 高层沟通方法论

核心证据：

- 2026-04-30 到 2026-05-08 合规相关 Codex session。
- macmini session `OPC 对比`：飞书总规划与功能 MD 串联方案。
- `output/董事长工作流优化方案_20260519.md`

## 仍需补证的模块

这些方向已经出现，但证据还不如上面模块厚：

- `日常运营` 工作区具体功能拆解：目前有工作区规则和五包对比，但业务模块细节还可继续扒。
- `C 系统版本` 具体业务模块：目前有工作区规则和规划对比清单，仍需单独展开。
- `合规法规梳理` 的实体产物路径：session 明确，但文件路径还需继续定位。
- 私有 GitHub 仓库里的真实项目列表：当前缺 GitHub 权限，不能证明全量。

## 备注

`package_function_index.json` / `function_package_index.json` 是最理想的功能索引源，但本轮读取内容时卡在文件系统层；已确认文件存在：

- `package_function_index.json`：51483 bytes
- `function_package_index.json`：52187 bytes
- `current_status_rows.json`：40756 bytes

后续如果能稳定读取这三个 JSON，可以把本清单进一步升级成“索引原始字段版”。
