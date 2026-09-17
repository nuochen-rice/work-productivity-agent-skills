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

Three skills are currently available:

| Skill | Description | Best for |
| --- | --- | --- |
| [`campaign-retrospective-en`](#campaign-survey-retrospective) | Generates a structured campaign or survey retrospective and cleans raw survey feedback. | Campaign reviews, survey analysis, promotion reviews, and user-feedback synthesis |
| [`lark-whiteboard-gen`](#lark-whiteboard-generator) | Turns natural-language prompts or documents into editable Lark whiteboards. | Architecture diagrams, process maps, roadmaps, operating models, and knowledge maps |
| [`report-web-glass`](#report-web-glass) | Turns raw materials into a glassmorphism narrative single-page HTML report (dark / light themes) and deploys it. | Background briefings, project kickoffs, research reports, and stakeholder alignment |

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

### 🪟Report Web Glass

```bash
npx skills add nuochen-rice/work-productivity-agent-skills \
  --skill report-web-glass
```

You can also install multiple skills at once:

```bash
npx skills add nuochen-rice/work-productivity-agent-skills \
  --skill campaign-retrospective-en \
  --skill lark-whiteboard-gen \
  --skill report-web-glass
```

> Your agent environment must support the `skills` installer. Lark publishing also requires the corresponding document, spreadsheet, Wiki, and whiteboard integrations.

<a id="campaign-survey-retrospective"></a>

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

<a id="lark-whiteboard-generator"></a>

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

<a id="report-web-glass"></a>

## 🪟Report Web Glass

[`report-web-glass`](report-web-glass/) turns raw materials — documents, research notes, data, interview quotes — into a single-page HTML report in a glassmorphism "narrative long-page" style, then deploys it to a shareable link.

It organizes content in an easy-to-follow narrative order (analogy → concept → structure → judgment → next steps), so readers without background knowledge can understand a complex topic. Every page ships with a scroll progress bar, sticky navigation, reveal-on-scroll animations, and a searchable glossary.

Key features:

- **Dark / light themes** — switch with a single `data-theme` attribute; both share the same tokens.
- **Content fidelity** — never fabricates data; missing fields are left as explicit placeholders, and inferences are marked distinctly from facts.
- **Source links** — material sources in the footer link back to the original documents.

Use this skill when you need to:

- explain a project's background to management or cross-team collaborators;
- write a research report or a project kickoff page;
- turn scattered materials into a polished, shareable web page.

Not for: full web apps requiring login / backend / multiple routes, or charts meant to be embedded inside a Lark document.

<p align="right"><a href="#work-productivity-agent-skills">Back to top ↑</a></p>

---

<a id="简体中文"></a>

## 简体中文

这个仓库提供面向日常工作提效的 AI Agent Skills，适用于运营复盘、用户调研、知识整理和可视化表达等场景。

目前提供三个 Skill：

| Skill | 能力说明 | 适用场景 |
| --- | --- | --- |
| [`campaign-retrospective-en`](#宣发与调研复盘) | 生成结构化活动或调研复盘，并清洗原始问卷反馈。 | 活动复盘、调研分析、宣发复盘、用户反馈分析 |
| [`lark-whiteboard-gen`](#飞书画板生成器) | 将自然语言或文档转换成可编辑的飞书画板。 | 产品架构、流程图、路线图、运营模型、知识地图 |
| [`report-web-glass`](#报告式玻璃拟态长页) | 将现有材料整理成玻璃拟态叙事长页 HTML 报告（深色 / 浅色主题），并部署成可访问链接。 | 背景说明、项目 kickoff、调研报告、方案对齐 |

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

### 🪟安装报告式玻璃拟态长页 Skill

```bash
npx skills add nuochen-rice/work-productivity-agent-skills \
  --skill report-web-glass
```

也可以一次安装多个 Skill：

```bash
npx skills add nuochen-rice/work-productivity-agent-skills \
  --skill campaign-retrospective-en \
  --skill lark-whiteboard-gen \
  --skill report-web-glass
```

> 使用环境需要支持 `skills` 安装工具。若需要将结果写入飞书文档、电子表格、知识库或画板，还需要宿主环境提供相应的飞书集成能力和权限。

<a id="宣发与调研复盘"></a>

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

<a id="飞书画板生成器"></a>

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

<a id="报告式玻璃拟态长页"></a>

## 🪟报告式玻璃拟态长页

[`report-web-glass`](report-web-glass/) 可以把现有材料——文档、调研笔记、数据、访谈原声——整理成一份「玻璃拟态 · 叙事长页」风格的单页 HTML 报告，并部署成可分享的链接。

它按「先类比 → 再概念 → 再结构 → 再判断 → 再下一步」的叙事顺序组织内容，让没有背景知识的读者也能读懂一件复杂的事。每个页面都自带滚动进度条、吸顶导航、渐显动画和可搜索的术语速查。

核心特性：

- **深色 / 浅色双主题**——只需一个 `data-theme` 属性即可切换，两套主题共用同一批设计 token；
- **内容忠实**——绝不编造数据，缺失字段以显式占位标注，推断与事实明确区分；
- **来源链接**——页脚的材料来源可点击回溯到原始文档。

适合以下场景：

- 向管理层或跨团队协作方讲清一个项目的背景；
- 撰写调研报告或项目 kickoff 页面；
- 把零散材料整理成一份好看、可分享的网页。

不适用于：需要登录 / 后端 / 多路由的完整 Web 应用，或要嵌进飞书文档的图表。

<p align="right"><a href="#work-productivity-agent-skills">返回顶部 ↑</a></p>

---

## License / 许可证

This repository is released under the [MIT License](LICENSE).

本仓库基于 [MIT License](LICENSE) 发布。
