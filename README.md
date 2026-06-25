# Editor

Strategic editorial review skill for **Claude Code** — McKinsey-style pre-meeting reviews with virtual expert panels and an editor's checklist, built for recurring column writing workflows.

为 **Claude Code** 打造的战略型编辑审阅技能 — 麦肯锡式会前审阅、虚拟专家圆桌和编辑检查清单，专为周期性专栏写作工作流设计。

## What It Does / 功能概述

The Editor skill transforms a draft article and meeting context into a structured, three-part editorial diagnosis that writing partners can read before their weekly meeting — so discussion starts from shared context rather than raw first impressions.

Editor 技能将一篇草稿和会议背景转化为结构化的三部分编辑诊断，让写作伙伴在周会前读到同一份审阅——讨论从共同背景出发，而非从原始的第一反应开始。

Every review has three pillars / 每次审阅包含三大支柱：

1. **Strategic Article Review** / **战略文章审阅** — 7 questions based on McKinsey-style problem solving (answer-first, MECE, issue tree, evidence hierarchy, 7-step problem solving) / 基于麦肯锡式问题解决的 7 个问题（答案先行、MECE、议题树、证据层级、7 步问题解决法）
2. **Virtual Expert Panel** / **虚拟专家圆桌** — 3–5 expert lenses debating the article's assumptions using the `ljg-roundtable` method / 3–5 位专家视角，采用 `ljg-roundtable` 方法辩论文章假设
3. **Editor's Checklist** / **编辑检查清单** — 15 criteria from mature editorial practice (thesis, originality, evidence, fairness, risk, voice, and more) / 基于成熟编辑实践的 15 项标准（论点、原创性、证据、公平性、风险、声音等）

## Quick Start / 快速开始

Invoke the skill in Claude Code / 在 Claude Code 中调用技能：

```
/editor
```

Or trigger with natural language / 或用自然语言触发：

> "帮我审阅一下这周的专栏草稿"
>
> "Run a pre-meeting editorial review on this draft"

## Documentation / 文档

| Document | Language | Description |
|----------|----------|-------------|
| [USAGE.md](USAGE.md) | English | Full usage guide with examples, prompts, and best practices |
| [USAGE.zh-CN.md](USAGE.zh-CN.md) | 中文 | 完整使用说明，含示例、提示语和最佳实践 |
| [SKILL.md](SKILL.md) | English | Skill definition — workflow, methodology, templates |
| [SKILL.zh-CN.md](SKILL.zh-CN.md) | 中文 | 技能定义 — 工作流、方法论、模板 |

## When to Use / 使用场景

- Before a weekly column meeting: get a pre-read that aligns both writing partners / 周会前：生成会前预读，让双方对齐
- When unsure about publishability: get a structured diagnosis / 不确定是否达到发表标准：获取结构化诊断
- When an argument feels weak: pressure-test with expert lenses / 论证力度不够：用专家视角压测
- When planning the pipeline: evaluate candidate topics / 规划选题：评估候选题目
- When co-authors disagree: name the editorial tradeoff without taking sides / 合作作者有分歧：把分歧定义为编辑取舍，不站队

## Installation / 安装

Copy the skill files to your Claude Code skills directory / 将技能文件复制到 Claude Code 技能目录：

```bash
cp SKILL.md ~/.claude/skills/editor/SKILL.md
cp SKILL.zh-CN.md ~/.claude/skills/editor/SKILL.zh-CN.md
```

Or symlink the entire directory / 或软链接整个目录：

```bash
ln -s $(pwd) ~/.claude/skills/editor
```

## Related Skills / 相关技能

- [ljg-roundtable](https://github.com/pkudss-33/ljg-skill-roundtable) — the general roundtable debate method used by the expert panel / 专家圆桌采用的通用圆桌辩论方法
- [huangwei-report-builder](https://github.com/Hatari130/huangwei-report-builder) — build polished report drafts, then review with Editor / 构建精致报告草稿，然后用 Editor 审阅

## License / 许可

This skill is part of the Claude Code skills ecosystem. / 本技能属于 Claude Code 技能生态系统。
