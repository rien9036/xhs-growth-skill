# XHS Growth Skill

面向小红书获客、内容增长、线索转化与规模化运营的一体化 AI Skill。

**这是一个单一 Skill。** 安装后只需要调用根目录 `SKILL.md`；所有专业能力都由它在内部自动选择，不需要分别安装或调用多个 Skills。

## Core Workflow

**业务目标 → 方向假设 → 小规模测试 → 定位收敛 → 需求关键词 → 内容 SOP → 自然分发 → 意向识别 → 合规线索承接 → 成交 → 付费放大 → 规模复制 → 数据复盘**

## Capabilities

- `account-launch-positioning`：方向测试、定位收敛、主页表达与视觉基线
- `audience-keyword-intelligence`：目标用户、需求信号、关键词与长尾需求
- `content-production-sop`：选题、标题、封面、正文与内容生产 SOP
- `organic-distribution-seo`：搜索、推荐、点击、互动与自然流量诊断
- `lead-conversion-funnel`：意向识别、线索承接与成交漏斗
- `paid-growth`：素材测试、预算、CAC/ROI 与付费放大
- `matrix-scaling`：已验证模型的多账号与规模复制
- `analytics-experimentation`：数据诊断、A/B 测试与增长实验
- `team-growth-ops`：角色分工、SOP、培训、知识库与绩效

以上名称只是内部能力模块。详细方法放在 `references/methods/`，用于按需加载，不是独立 Skills。

## Structure

```text
.
├── README.md
├── SKILL.md
└── references/
    ├── capability-map.md
    ├── case-patterns.md
    ├── checklists.md
    ├── frameworks.md
    ├── metrics-and-diagnostics.md
    ├── versioning-and-compliance.md
    └── methods/
        ├── account-launch-positioning.md
        ├── audience-keyword-intelligence.md
        ├── content-production-sop.md
        ├── organic-distribution-seo.md
        ├── lead-conversion-funnel.md
        ├── paid-growth.md
        ├── matrix-scaling.md
        ├── analytics-experimentation.md
        └── team-growth-ops.md
```

- `SKILL.md`：唯一 Skill 入口，负责理解任务、选择内部方法和组合完整工作流。
- `references/methods/`：详细方法库，仅供本 Skill 内部按需读取。
- 其他 `references/`：框架、检查清单、指标、案例模式与平台时效性资料。

# Installation

## Codex — Skill Installer

在 Codex 中可以让内置的 `$skill-installer` 安装该 GitHub 仓库根目录的 Skill：

```text
$skill-installer install the skill at the repository root from https://github.com/rien9036/xhs-growth-skill
```

安装完成后，重新启动 Codex 或开启新的会话。

## Codex — Manual Install

macOS / Linux：

```bash
git clone https://github.com/rien9036/xhs-growth-skill.git ~/.codex/skills/xhs-growth-skill
```

安装后的核心结构：

```text
~/.codex/skills/xhs-growth-skill/
├── SKILL.md
└── references/
```

## ChatGPT

如果你的 ChatGPT 账号或工作区支持 Skills：

1. 点击本仓库右上角 **Code → Download ZIP**。
2. 在 ChatGPT 的 Skills 页面选择 **Create → Upload from your computer**。
3. 上传下载的 Skill 包。

> Skills 的具体可用范围取决于当前账号、工作区权限和管理员设置。

## Other Agent Skills Clients

如果其他 Agent 支持以 `SKILL.md` 为入口的 Agent Skills，可以克隆整个仓库，并把根目录 `SKILL.md` 作为唯一入口：

```bash
git clone https://github.com/rien9036/xhs-growth-skill.git
```

# Quick Start

安装后直接描述任务即可，不需要记忆内部方法名称。

```text
我有一个服务型业务，帮我从 0 到 1 建立小红书获客系统。
```

```text
帮我找目标客户最可能搜索的关键词，并建立长尾选题库。
```

```text
我的笔记有曝光但没有有效客户，帮我诊断获客漏斗。
```

```text
哪些内容值得付费放大？帮我设计小预算测试和止损规则。
```

```text
单账号已经跑通，帮我设计矩阵扩张和团队分工。
```

# How It Works

`SKILL.md` 会先判断当前问题属于哪个环节，只读取必要的内部方法。例如：

- 定位未明确时，不会直接跳到投流或规模化。
- 流量异常时，会先区分需求、包装、内容、分发还是承接问题。
- 有流量但商业结果弱时，会进入转化/交易诊断，而不是继续只追求曝光。
- 从 0 到 1 的复杂任务会按端到端工作流组合多个内部方法。

# Platform Freshness

小红书的平台规则、账号权限、广告产品、店铺能力、认证条件、私信/留资方式、费用和流量产品可能随时间变化。稳定的方法论可以直接执行；涉及当前平台功能、门槛、费用和限制时，应先核验当前官方规则。历史经验、案例数据和经验阈值不能包装成当前平台算法。

# Compliance

本 Skill 不建议或鼓励刷量、刷粉、伪造互动、虚构身份、内容搬运、规避平台风控或绕过平台规则的引流方式。优先使用真实内容、真实用户反馈、合规商业表达、官方商业工具以及可持续的交易模型。

# Contributing

欢迎通过 Issue 或 Pull Request 改进工作流、判断规则、Prompt、输出模板、数据诊断框架、平台时效性与合规说明。

# Disclaimer

本项目提供内容运营、商业分析和 AI 工作流辅助，不构成收益保证。涉及平台规则、广告、店铺、认证、线索工具和其他平台功能时，请以当前官方规则为准。
