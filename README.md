# hand-on-openclaw

`hand-on-openclaw` 是一个面向零基础学习者的 OpenClaw 中文开源教程项目，目标是提供从安装到实战的完整参考手册。

## 项目目标

- 面向零基础用户的完整参考手册 / 百科全书式教程
- 模块化设计：可按需跳读，不必按固定学习节奏
- 图文并茂：关键步骤配截图，降低实操门槛
- 中国用户友好：优先覆盖国内常用模型与平台（DeepSeek / 智谱 / Moonshot、飞书 / 钉钉 / 企业微信）

## 项目亮点

- 端到端闭环：从 `Windows + WSL` 安装、`openclaw onboard`、飞书接入，到多 Agent 与 Skills 使用，形成完整落地链路。
- 零基础友好：按操作顺序拆分章节，保留截图驱动的步骤说明，强调“做完可验证”的实操路径。
- 中国场景优先：优先覆盖国内用户高频渠道与模型，降低网络、支付、可用性门槛。
- 结构化演进：README 明确区分“当前状态（已完成）”与“Roadmap（计划）”，便于协作和持续迭代。
- 可迁移到工程化文档站：已预留 MkDocs 站点化目录与示例工程结构，后续可平滑升级到文档网站。

## 同类项目调研（2026-03-01 快照）

### 调研口径

- 检索范围：官方文档 + GitHub 上 `openclaw` 相关 `tutorial/docs/awesome/skills` 项目。
- 评估维度：定位（官方/教程/导航/技能清单）、内容完整度、面向人群、可执行性。
- 数据来源：GitHub API（星标、更新时间、仓库描述）与官方文档页面。

### 已发现的主要类似项目

| 项目 | 类型/定位 | 已验证信号（2026-03-01） | 与本项目的主要差异 |
| --- | --- | --- | --- |
| [`openclaw/openclaw`](https://github.com/openclaw/openclaw) | 官方核心仓库（产品与代码） | 242,346 stars；持续更新 | 偏产品与开发实现，不是中文零基础图文教程。 |
| [`docs.openclaw.ai`](https://docs.openclaw.ai/start/getting-started) | 官方文档（Quickstart/CLI Wizard） | 官方站点；含 `Getting Started` 与 `Onboarding Wizard` | 权威但更偏通用说明，国内平台和本土化实战覆盖有限。 |
| [`SamurAIGPT/awesome-openclaw`](https://github.com/SamurAIGPT/awesome-openclaw) | 生态导航/资源聚合 | 713 stars；持续更新 | 更像“索引目录”，不提供从 0 到 1 的连续实操手册。 |
| [`VoltAgent/awesome-openclaw-skills`](https://github.com/VoltAgent/awesome-openclaw-skills) | Skills 清单与分类 | 23,835 stars；强调 5,400+ skills | 强在技能发现，不负责安装部署与渠道接入全流程教学。 |
| [`sundial-org/awesome-openclaw-skills`](https://github.com/sundial-org/awesome-openclaw-skills) | Skills 热门清单 | 307 stars；持续更新 | 同样偏“技能推荐”，不是系统化入门教程。 |
| [`yeuxuan/openclaw-docs`](https://github.com/yeuxuan/openclaw-docs) | 社区中文教程/拆解文档 | 447 stars；近期活跃 | 与本项目同属教程方向，但本项目更强调“按步骤可复现 + 飞书多智能体落地链路”。 |
| [`mengjian-github/openclaw101`](https://github.com/mengjian-github/openclaw101) | 中文学习站/资源聚合 | 595 stars；`OpenClaw 101` 定位 | 偏资源平台与课程化组织，本项目更聚焦开源文档手册与可复制操作细节。 |

### 本项目的差异化定位

1. 相比官方文档：本项目更聚焦中文用户实操路径，补充国内模型/平台和踩坑经验。
2. 相比 awesome 清单：本项目不是“链接集合”，而是“可一步步照做的流程文档”。
3. 相比 Skills 清单项目：本项目覆盖安装、配置、渠道、Agent、Skills 的全链路，不只讲技能选择。
4. 相比部分社区教程：本项目将“当前状态 + 计划路线”写入 README，强调长期维护与工程化演进。
5. 相比一次性教程帖：本项目采用模块化拆分，支持按需跳读，同时保留完整阅读顺序索引。

## 当前状态（截至 2026-03-01）

### 已完成

- 已将原始单文件教程拆分为 `doc/` 多文件结构，按阅读顺序组织。
- 已补充文档入口索引：`doc/00-阅读顺序.md`。
- 已在 README 说明项目定位、内容范围与迭代方向。

### 当前仓库结构（实际）

```text
hand-on-openclaw/
├── README.md
└── doc/
    ├── 00-阅读顺序.md
    ├── 01-介绍.md
    ├── 02-环境准备.md
    ├── 03-openclaw配置.md
    ├── 04-飞书配置.md
    ├── 05-飞书群聊多智能体配置.md
    ├── 06-workspace与agentdir.md
    ├── 07-skills与clawhub.md
    └── 08-心得.md
```

### 当前阅读入口

1. [阅读顺序索引](./doc/00-阅读顺序.md)
2. [01-介绍](./doc/01-介绍.md)
3. [02-环境准备](./doc/02-环境准备.md)
4. [03-openclaw配置](./doc/03-openclaw配置.md)
5. [04-飞书配置](./doc/04-飞书配置.md)
6. [05-飞书群聊多智能体配置](./doc/05-飞书群聊多智能体配置.md)
7. [06-workspace与agentdir](./doc/06-workspace与agentdir.md)
8. [07-skills与clawhub](./doc/07-skills与clawhub.md)
9. [08-心得](./doc/08-心得.md)

## 计划（Roadmap）

### P0：文档质量与一致性（近期）

- 统一章节标题规范（命名、大小写、编号格式）。
- 为每章补充模板：前置条件 / 操作步骤 / 验收结果 / 常见报错。
- 增加“命令速查表”和“飞书最小权限清单”。
- 清理重复段落，缩短超长章节并提高可检索性。

### P1：站点化发布（中期）

- 引入 `MkDocs + Material for MkDocs`。
- 新增 `mkdocs.yml` 与 `docs/` 站点目录，迁移现有内容。
- 使用 GitHub Pages 自动部署文档站点。

### P2：示例与工程化（中期）

- 新增 `examples/skills`、`examples/configs`、`examples/workflows`。
- 提供可直接复制的 `openclaw.json`、`SOUL.md`、`USER.md` 示例。
- 增加端到端实战案例（个人助手 / 团队机器人 / 自动化流）。

### P3：进阶内容（后续）

- 增加源码解析、消息链路、从源码构建章节。
- 补齐自动化专题（cron / heartbeat / webhook）。
- 增加团队协作最佳实践（权限边界、日志与审计、命名规范）。

## 目标结构（规划版）

以下是计划中的标准化目录（用于站点化后版本）：

```text
openclaw-guide/
├── README.md                          # 项目介绍 + 贡献指南
├── LICENSE                            # Apache 2.0
├── mkdocs.yml                         # MkDocs 配置
├── requirements.txt                   # mkdocs-material 等依赖
├── docs/
│   ├── index.md                       # 首页：什么是 OpenClaw + 教程导航
│   ├── install/                       # 第一篇：安装部署
│   ├── basic/                         # 第二篇：基础使用
│   ├── skills/                        # 第三篇：插件/技能系统
│   ├── automation/                    # 第四篇：自动化工作流
│   ├── deep-dive/                     # 第五篇：源码解析与复现
│   └── projects/                      # 第六篇：实战项目
└── examples/
    ├── skills/
    ├── configs/
    └── workflows/
```

## 目标内容大纲（规划版）

### 第一篇：安装部署（docs/install/）

- 安装方式对比：一键脚本 / npm / 源码 / 云端
- 平台安装：macOS、Windows（WSL2）、Linux、云端
- 故障排查：权限、Node 版本、端口冲突

### 第二篇：基础使用（docs/basic/）

- `openclaw onboard` 全流程与 Web 面板使用
- 国内友好模型选择（DeepSeek、Ollama 等）
- 多渠道接入（Telegram、飞书、钉钉、企业微信、Discord）
- Workspace 与 Memory 实战

### 第三篇：Skills 插件开发（docs/skills/）

- Skills 基础认知与安装
- 自定义 Skill 编写（`SKILL.md`）
- 发布到 ClawHub（含 OAuth 授权）

### 第四篇：自动化工作流（docs/automation/）

- 晨报、邮件摘要、定时提醒等场景化模板

### 第五篇：源码解析（docs/deep-dive/）

- 模块架构图（Mermaid）
- 消息处理链路（用户输入 -> AI 回复）
- 从源码构建与本地调试

### 第六篇：实战项目（docs/projects/）

- 个人助手、团队机器人、自动化工作流 3 个端到端教程

## 贡献建议

- 优先提交可复现的步骤、报错和修复方案。
- 新增章节时遵循统一模板，避免重复描述。
- 示例配置请脱敏（API Key、Token、组织信息）。
