# Work Productivity Agent Skills

<p align="center">
  Reusable AI agent skills for everyday work productivity.
</p>

<p align="center">
  <a href="#english">English</a> ·
  <a href="#简体中文">简体中文</a>
</p>

---

<a id="english"></a>

## English

This repository provides reusable AI agent skills for operations, user research, knowledge organization, and visual communication.

Two skills are currently available:

| Skill | Description | Best for |
| --- | --- | --- |
| [`campaign-retrospective-en`](#campaign--survey-retrospective) | Generates a structured campaign or survey retrospective and cleans raw survey feedback. | Campaign reviews, survey analysis, promotion reviews, and user-feedback synthesis |
| [`lark-whiteboard-gen`](#lark-whiteboard-generator) | Turns natural-language prompts or documents into editable Lark whiteboards. | Architecture diagrams, process maps, roadmaps, operating models, and knowledge maps |

## Installation

Install a skill directly from this repository:

### ✍️Campaign & Survey Retrospective

```bash
npx skills add nuochen-rice/work-productivity-agent-skills \
  --skill campaign-retrospective-en
```

### 🎨Lark Whiteboard Generator

```bash
npx skills add nuochen-rice/work-productivity-agent-skills \
  --skill lark-whiteboard-gen
```

You can also install both skills:

```bash
npx skills add nuochen-rice/work-productivity-agent-skills \
  --skill campaign-retrospective-en \
  --skill lark-whiteboard-gen
```

> Your agent environment must support the `skills` installer. Lark publishing also requires the corresponding document, spreadsheet, Wiki, and whiteboard integrations.

## ✍️Campaign & Survey Retrospective

[`campaign-retrospective-en`](campaign-retrospective-en/) turns campaign materials, performance metrics, survey results, and raw user feedback into two standardized deliverables:

1. A cleaned survey workbook containing `Valid Feedback` and `Low-score Feedback` sheets.
2. A structured Lark Wiki retrospective covering key conclusions, campaign performance, user feedback, and follow-up actions.

Use this skill when you need to:

- review a campaign or promotion;
- analyze survey results;
- organize scattered user feedback;
- identify low-score or strongly negative feedback;
- produce an evidence-based retrospective without inventing missing data.

## 🎨Lark Whiteboard Generator

[`lark-whiteboard-gen`](lark-whiteboard-gen/) turns natural-language prompts, documents, or structured information into editable Lark whiteboards.

It automatically follows the language of the prompt and supports Chinese, English, and explicitly requested bilingual boards.

Use this skill when you need to create:

- product or technical architecture diagrams;
- processes and user journeys;
- timelines and roadmaps;
- role and collaboration maps;
- operating models and feedback loops;
- comparisons, funnels, pyramids, or knowledge maps.

The skill uses a structured, hand-drawn infographic style while keeping text, shapes, and connectors editable.

<p align="right"><a href="#work-productivity-agent-skills">Back to top ↑</a></p>

---

<a id="简体中文"></a>

## 简体中文

这个仓库提供面向日常工作提效的 AI Agent Skills，适用于运营复盘、用户调研、知识整理和可视化表达等场景。

目前提供两个 Skill：

| Skill | 能力说明 | 适用场景 |
| --- | --- | --- |
| [`campaign-retrospective-en`](#宣发与调研复盘) | 生成结构化活动或调研复盘，并清洗原始问卷反馈。 | 活动复盘、调研分析、宣发复盘、用户反馈分析 |
| [`lark-whiteboard-gen`](#飞书画板生成器) | 将自然语言或文档转换成可编辑的飞书画板。 | 产品架构、流程图、路线图、运营模型、知识地图 |

## 安装方式

可以通过以下命令直接从本仓库安装 Skill。

### ✍️安装宣发与调研复盘 Skill

```bash
npx skills add nuochen-rice/work-productivity-agent-skills \
  --skill campaign-retrospective-en
```

### 🎨安装飞书画板生成 Skill

```bash
npx skills add nuochen-rice/work-productivity-agent-skills \
  --skill lark-whiteboard-gen
```

也可以一次安装两个 Skill：

```bash
npx skills add nuochen-rice/work-productivity-agent-skills \
  --skill campaign-retrospective-en \
  --skill lark-whiteboard-gen
```

> 使用环境需要支持 `skills` 安装工具。若需要将结果写入飞书文档、电子表格、知识库或画板，还需要宿主环境提供相应的飞书集成能力和权限。

## ✍️宣发与调研复盘

[`campaign-retrospective-en`](campaign-retrospective-en/) 可以把活动素材、效果数据、问卷结果和用户原声整理成两项标准化交付物：

1. 一份包含 `Valid Feedback`（有效反馈）和 `Low-score Feedback`（低分反馈）的问卷清洗表格。
2. 一篇包含重点结论、活动效果、用户反馈和后续行动的飞书 Wiki 复盘文档。

适合以下场景：

- 复盘一场活动或宣传推广；
- 分析用户调研和问卷结果；
- 整理零散的用户反馈；
- 识别低评分和强烈负面反馈；
- 在不编造缺失数据的前提下生成结构化复盘。

## 🎨飞书画板生成器

[`lark-whiteboard-gen`](lark-whiteboard-gen/) 可以将自然语言、文档或结构化信息转换成可编辑的飞书画板。

它会自动跟随用户输入的语言，并支持中文、英文以及用户明确要求的双语画板。

适合生成：

- 产品或技术架构图；
- 流程图和用户旅程；
- 时间线和路线图；
- 角色关系与协作机制；
- 运营模型和反馈闭环；
- 对比图、漏斗、金字塔和知识地图。

画板采用“严谨网格 + 手绘信息图”的视觉风格，同时保留可编辑的文本、形状和连接线。

<p align="right"><a href="#work-productivity-agent-skills">返回顶部 ↑</a></p>

---

## License / 许可证

This repository is released under the [MIT License](LICENSE).

本仓库基于 [MIT License](LICENSE) 发布。
