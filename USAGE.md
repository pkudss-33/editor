# Editor Skill — Usage Guide

## What It Does

The **Editor** skill is a strategic pre-meeting editorial review system designed for recurring column writing workflows. It transforms a draft article and meeting context into a structured, three-part editorial diagnosis that both writing partners can read before their weekly meeting — so the discussion starts from shared context rather than raw first impressions.

Each review output has three pillars:

| Part | Method | Purpose |
|------|--------|---------|
| **Strategic Article Review** | McKinsey-style 7 questions | Test whether the article is strategically clear, not just well-written |
| **Virtual Expert Panel** | `ljg-roundtable` method with 3–5 expert lenses | Challenge assumptions and deepen the argument from multiple intellectual frameworks |
| **Editor's Checklist** | Mature editorial practice (15 criteria) | Catch blocking issues, risks, and high-value improvements before publication |

The skill is opinionated about **what good editing looks like**: it prioritizes the central claim, reader value, and publishability above surface-level wording polish. It distinguishes between "must fix", "would improve", and "future idea." It preserves the writer's voice.

---

## When to Use It

Invoke this skill whenever you are in or preparing for a **column editorial workflow**. The skill description triggers on mentions of:

- Editor / editing / editorial review
- Draft feedback / article review / pre-meeting pre-read
- Weekly column meeting / weekly review / co-writing session
- Economic commentary or opinion piece assessment
- Expert lenses / virtual expert panel / roundtable review
- McKinsey-style review / strategic article diagnosis
- Column planning / next-topic selection

**Concrete scenarios:**

- You have a draft and a weekly meeting coming up → get a pre-read to align both partners before the meeting
- You're unsure whether a piece is ready to publish → get a structured publishability diagnosis
- You want to pressure-test an argument from multiple expert angles → get a virtual roundtable that challenges assumptions
- You're planning the next column topic → get a structured topic evaluation and recommendation
- You received an unclear or emotional first reaction to a draft → get a calm, strategic diagnosis instead

---

## How to Invoke

### Direct invocation

```
/editor
```

Then provide the article draft and meeting context when asked. The skill will walk through its three-part review workflow.

### Natural-language trigger

Any phrase that matches the skill's trigger vocabulary will auto-load it:

> "帮我审阅一下这周的专栏草稿"
>
> "Run an editorial review on this draft before tomorrow's meeting"
>
> "用专家圆桌的方法压测这篇文章的论点"

### Combined with article text

Paste the article text directly with your request:

> "Here's this week's draft — give me a pre-meeting editorial review. Target audience is Caixin readers, meeting is tomorrow at 10am. We need to decide whether to publish or restructure."

---

## Required Inputs

The skill needs three pieces of information to produce a useful review. If any is missing, it will ask.

| Input | Example |
|-------|---------|
| **Article text or draft** | The full text, or a link/file path to it |
| **Target reader & publication context** | "Caixin opinion column", "FT Chinese", "internal strategy memo" |
| **Meeting decision needed** | Publish / revise / restructure / split / shelve / develop further |

Optional but helpful:

- **Author name or voice notes** — helps the skill preserve voice instead of normalizing it
- **Known editorial concerns** — "we're worried the evidence section is too thin" or "the editor-in-chief questioned the timeliness"
- **Previous reviews or feedback** — so the skill can track what's been addressed
- **Desired depth** — a quick strategic check vs. a full three-part review with detailed panel attachment

---

## What You Get

### Main review (always produced)

A structured pre-meeting document with:

1. **Header block** — thesis, reader payoff, recommended decision, one-line editorial judgment
2. **7-question strategic diagnosis** — answer-first, So what, MECE structure, issue tree, evidence hierarchy, problem-solving path, meeting synthesis
3. **Expert panel takeaway** — sharpest challenge, best deepening opportunity, missing perspective, demanded evidence, meeting question
4. **Editor's checklist** — must-fix, strengthen, watch-risk items
5. **Meeting questions** — questions designed to help authors decide direction, not just react
6. **Suggested agenda** — 3-item meeting structure

### Panel attachment (default: inline appendix; file mode: separate `.md`)

The full virtual expert roundtable with 3–5 expert lenses debating in rounds:

- Round 1: Definitions and first principles
- Round 2: Core disagreement with ASCII structure map
- Round 3: Implications for the article
- Knowledge network diagram
- Open questions for the authors

---

## Workflow Examples

### Example 1: Standard Weekly Review

**User:**
> /editor
> 这是本周的专栏草稿，目标读者是财新专栏的读者，明天上午10点开会，需要决定是发表还是需要大改。
> [pastes article text]

**Skill response:**
1. Confirms the review frame (article, audience, decision)
2. Runs the three-part review
3. Produces the main pre-meeting review document
4. Attaches the virtual expert panel as an appendix

**Expected time:** The review itself is generated in one response; the panel attachment may follow in a second turn if very detailed.

### Example 2: Quick Strategic Check

**User:**
> "Just give me the 7-question strategic review for this draft — skip the full panel. We're short on time."

**Skill response:**
Produces only Part 1 (strategic article review) and Part 3 (editor's checklist), with a brief expert takeaway but no detailed panel attachment.

### Example 3: Column Planning

**User:**
> "We need to pick next week's topic. Here are three candidates: [topic A], [topic B], [topic C]."

**Skill response:**
Uses the **Planning Template** to evaluate each candidate on angle, timeliness, evidence needed, expert lenses, and risk — then recommends the strongest option with a working title, core claim, structure, and inputs needed.

### Example 4: Expert Panel Only

**User:**
> "I'm confident in the structure but want to pressure-test the core argument. Just run the virtual expert panel on this draft."

**Skill response:**
Focuses on Part 2, selecting 3–5 expert lenses for the article's topic, running the roundtable, and producing both the main-review takeaway and the detailed panel attachment.

### Example 5: File-Based Workflow

**User:**
> "The draft is at `articles/2026-06-25-trade-war.md`. Run the full review and save the panel as a separate attachment file."

**Skill response:**
Reads the draft from the file, produces the main review, and creates `virtual-expert-panel-trade-war.md` as a separate Markdown file in the same directory.

---

## Common Use Cases & Prompts

### Before a weekly meeting

> "我们明天下午开周会，讨论这篇稿子 [paste draft]。帮我做一份会前编辑审阅，包含完整的战略审阅和专家圆桌。这篇文章的目标是财新专栏，读者是关注宏观经济的专业人士。"

### When stuck on structure

> "This piece feels repetitive and I can't figure out why. Run the MECE structure diagnosis and issue tree analysis. Don't worry about wording — just tell me if the argument pillars hold up."

### When the argument feels weak

> "我觉得这篇论证不够强，但说不清哪里弱。请用证据层级（evidence hierarchy）帮我校准，并让专家圆桌告诉我还需要什么数据或分析才能让论证立得住。"

### When preparing a rewrite

> "主编觉得这篇缺乏原创性。帮我做一轮完整的编辑审阅，重点放在：读者收益（reader payoff）、原创性和缺失视角上。专家圆桌至少选一位非经济领域的意外视角。"

### When planning the pipeline

> "接下来三周的选题还没定。我有四个可能的题目： [list topics]。帮我用选题规划模板做评估，推荐下周写哪篇。"

### When there's disagreement between co-authors

> "我和合作作者在这篇文章的论点上有分歧——我认为应该更强调风险，她觉得应该强调机会。帮我审阅草稿，把分歧定义为会议需要解决的编辑取舍，不要站队。"

---

## Tips & Best Practices

### 1. Give it the full draft, not a summary
The skill diagnoses structure, evidence, and argumentation — it needs the actual text to do that. A summary only lets it give generic feedback.

### 2. Name the publication context
"Economic media column" is too broad. "Caixin opinion column with a professional macroeconomic audience" produces much sharper feedback. The publication context determines the bar for evidence, originality, and risk tolerance.

### 3. State the meeting decision explicitly
"Is this ready to publish?" vs. "Should we restructure or split this into two pieces?" produce different kinds of reviews. The decision frames what the skill prioritizes.

### 4. Use "skip the panel" for fast turnaround
If you only have 5 minutes before the meeting, ask for just the 7-question strategic review and the editor's checklist. You can always run the panel later.

### 5. Treat the expert panel as a discussion starter, not a verdict
The panel is designed to surface tensions and deepen the meeting conversation. The "sharpest challenge" is meant to be debated, not accepted uncritically.

### 6. Let the skill ask clarifying questions
If you give it a draft without context, it will ask: target reader, publication, meeting goal, desired depth. Answering these produces a much better review.

### 7. Use the planning template between articles
The skill isn't only for reviewing finished drafts. Use the **Planning Template** to evaluate candidate topics before you write. It saves time and prevents weak starts.

### 8. Save panel attachments for reference
The virtual expert panel attachment contains frameworks, tensions, and open questions that are useful beyond one meeting. Save them alongside your article files — they become a reusable intellectual inventory for future pieces on similar topics.

---

## Relationship with Other Skills

| Skill | How it relates |
|-------|---------------|
| **ljg-roundtable** | The editor skill's Part 2 (Virtual Expert Panel) adopts the `ljg-roundtable` method for structuring expert debate. The roundtable skill provides the general debate framework; the editor skill applies it specifically to article review. |
| **huangwei-report-builder** | Complements the editor skill: use the report builder to turn messy research inputs into a polished draft, then use the editor skill to review that draft before publication. |
| **management-report-builder** | Similar complementary relationship — build the report, then review it with the editor skill. |

---

## Output Language

The skill produces reviews in the same language as the draft article and user request. Chinese drafts get Chinese reviews; English drafts get English reviews. The expert panel's frameworks and terminology stay in their original language (e.g., "MECE", "nut graf", "evidence hierarchy") regardless of the review language.
