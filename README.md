# Editor

Strategic editorial review skill for **Claude Code** — McKinsey-style pre-meeting reviews with virtual expert panels and an editor's checklist, built for recurring column writing workflows.

## What It Does

The Editor skill transforms a draft article and meeting context into a structured, three-part editorial diagnosis that writing partners can read before their weekly meeting — so discussion starts from shared context rather than raw first impressions.

Every review has three pillars:

1. **Strategic Article Review** — 7 questions based on McKinsey-style problem solving (answer-first, MECE, issue tree, evidence hierarchy, 7-step problem solving)
2. **Virtual Expert Panel** — 3–5 expert lenses debating the article's assumptions using the `ljg-roundtable` method
3. **Editor's Checklist** — 15 criteria from mature editorial practice (thesis, originality, evidence, fairness, risk, voice, and more)

## Quick Start

Invoke the skill in Claude Code:

```
/editor
```

Or trigger with natural language:

> "帮我审阅一下这周的专栏草稿"
>
> "Run a pre-meeting editorial review on this draft"

## Documentation

| Document | Language | Description |
|----------|----------|-------------|
| [USAGE.md](USAGE.md) | English | Full usage guide with examples, prompts, and best practices |
| [USAGE.zh-CN.md](USAGE.zh-CN.md) | 中文 | 完整使用说明，含示例、提示语和最佳实践 |
| [SKILL.md](SKILL.md) | English | Skill definition — workflow, methodology, templates |
| [SKILL.zh-CN.md](SKILL.zh-CN.md) | 中文 | 技能定义 — 工作流、方法论、模板 |

## When to Use

- Before a weekly column meeting: get a pre-read that aligns both writing partners
- When unsure about publishability: get a structured diagnosis
- When an argument feels weak: pressure-test with expert lenses
- When planning the pipeline: evaluate candidate topics
- When co-authors disagree: name the editorial tradeoff without taking sides

## Installation

Copy the skill files to your Claude Code skills directory:

```bash
cp SKILL.md ~/.claude/skills/editor/SKILL.md
cp SKILL.zh-CN.md ~/.claude/skills/editor/SKILL.zh-CN.md
```

Or symlink the entire directory:

```bash
ln -s $(pwd) ~/.claude/skills/editor
```

## Related Skills

- [ljg-roundtable](https://github.com/pkudss-33/ljg-skill-roundtable) — the general roundtable debate method used by the expert panel
- [huangwei-report-builder](https://github.com/Hatari130/huangwei-report-builder) — build polished report drafts, then review with Editor

## License

This skill is part of the Claude Code skills ecosystem.
