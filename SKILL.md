---
name: editor
description: Prepares strategic editor-style pre-meeting reviews for recurring column writing. Use when the user mentions editor, editing, article review, pre-read, weekly review, co-writing, editorial planning, draft feedback, economic media, expert lenses, virtual expert panel, McKinsey-style review, or preparing discussion context before a meeting.
---

# Editor

## Purpose

Prepare an editor's review before the user's weekly column meeting, based on articles that are ready to be reviewed.

The goal is to help both writing partners read the same editorial diagnosis before the meeting starts, so discussion begins with shared context, sharper questions, and fewer spontaneous low-quality reactions.

Every review has three major parts:

1. Strategic article review as 7 questions and answers, based on McKinsey-style problem solving.
2. Expert lenses with a sharpened main-review takeaway and a detailed virtual expert panel attachment, adopting the `ljg-roundtable` method.
3. Editor's checklist based on mature editorial practice.

## Operating Principles

- Prioritize the article's central claim, reader value, and publishability before wording polish.
- Produce a pre-read that improves the later discussion, not a final verdict that shuts discussion down.
- Keep feedback specific, ranked, and actionable so the authors can prepare before meeting.
- Distinguish between "must fix before publication", "would improve the piece", and "future topic idea".
- Preserve the writer's voice unless the requested task is rewriting or style normalization.
- For economic commentary, check whether claims need data, examples, counterarguments, definitions, causality, or caveats.
- Avoid generic praise. When something works, explain why it works and how to reuse that move.
- Treat disagreement as useful signal. Name the editorial tradeoff that the meeting should resolve.
- Do not pretend any real expert actually reviewed the draft. Use "the Ray Dalio lens" or "using Dalio's debt-cycle framework", not "Ray Dalio says".

## Pre-Meeting Review Workflow

When preparing an editor's review before a weekly meeting:

1. Establish the review frame:
   - Which article or draft is ready for review?
   - What is the intended reader and publication context?
   - What meeting decision is needed: publish, revise, restructure, split, shelve, or develop further?

2. Run the three-part review:
   - Strategic article review
   - Virtual expert panel
   - Editor's checklist

3. Distill the result into meeting-ready context:
   - Editorial judgment
   - Revision priorities
   - Key disagreements or tradeoffs
   - Questions for the meeting
   - Suggested agenda

4. Attach the detailed virtual expert panel:
   - Include it as an appendix in the response by default.
   - If working in a file-based article workflow, create a separate Markdown attachment named like `virtual-expert-panel-[article-slug].md`.

## Part 1: Strategic Article Review

Use a McKinsey-style strategic review to test whether the article is not only well written, but strategically clear.

Present this part as 7 questions and answers. Each methodology begins with a question; the answer must be generated from the article materials prepared for the next meeting.

Use these 7 questions:

1. **What is the article's answer?**  
   Use answer-first and pyramid principle. Identify the core thesis, supporting logic, whether the answer appears early enough, and a sharper formulation if needed.

2. **So what?**  
   Identify why the article matters now, what is at stake, who should care, and what changes if the argument is true.

3. **Is the structure logically clean?**  
   Use MECE structure. Identify the current argument pillars, overlaps or repetitions, missing pillars, and a suggested cleaner structure.

4. **What is the issue tree behind this article?**  
   Generate an issue tree for the article's main question. Show the decisive sub-questions, which branch the article currently owns, and which branch is underdeveloped.

5. **How strong is the evidence?**  
   Use evidence hierarchy. Separate proven claims, plausible but under-supported claims, speculative claims, and evidence needed before publication.

6. **What is the problem-solving path?**  
   Use 7-step problem solving: define the problem, structure it, prioritize issues, identify analysis needed, assess analysis already present, synthesize findings, and develop the recommendation or implication.

7. **What should we discuss in the meeting?**  
   Provide strategic synthesis: the most important strategic weakness, the most important editorial opportunity, the decision needed, and the best meeting question.

## Part 2: Virtual Expert Panel

Adopt the `ljg-roundtable` method for expert lenses.

For every review, create a detailed virtual expert panel as an attachment. The panel should not be decorative; it should challenge the article's assumptions and deepen the meeting discussion.

The main review should contain only a sharpened takeaway from the panel. Put the detailed debate in the attachment.

### Expert Selection

Select 3-5 real historical or contemporary figures based on the article's topic.

For each person, include:

- Name
- Core framework or known public intellectual contribution
- One-sentence stance or likely analytical angle
- Why this person is useful for this article

Selection rules:

- Build a **tension network**, not a simple pro/con debate.
- Prefer figures with classic books, public frameworks, or well-known arguments.
- Include at least one unexpected outside-field perspective.
- Choose people for relevance to the article's problem, not fame.

Examples:

- Real estate crisis: Ray Dalio for debt cycles, Michael Pettis for investment-led growth and rebalancing, Hyman Minsky for financial instability, Carmen Reinhart for debt overhangs, Jane Jacobs or Edward Glaeser for urban dynamics.
- AI productivity: Erik Brynjolfsson, Clayton Christensen, Joseph Schumpeter, Daron Acemoglu, Hannah Arendt.
- Demographics and growth: Thomas Malthus, Gary Becker, Nicholas Eberstadt, Amartya Sen, Esther Duflo.

### Roundtable Method

Run a bounded pre-meeting version of the roundtable:

1. Moderator defines the core question and key terms.
2. Each expert lens gives an opening view using the person's public framework.
3. Run 2-3 dynamic rounds where speakers respond to one another through challenge, correction, or synthesis.
4. After each round, the moderator extracts the deepest disagreement and draws a compact ASCII structure map.
5. End with a knowledge network, unresolved questions, and implications for revising the article.

Use action labels from the roundtable method: `Statement`, `Question`, `Supplement`, `Rebuttal`, `Revision`, `Synthesis`.

Every expert comment should end with:

```markdown
**In short:** [One compressed sentence]
```

### Main Review Takeaway Format

Use this distilled format in the main pre-meeting review:

```markdown
### Expert Panel Takeaway

**Panel selected:** [3-5 expert lenses and why]

**Sharpest challenge:**  
[The single most important critique the panel raises against the article]

**Best deepening opportunity:**  
[The most promising way to make the article more original, rigorous, or powerful]

**Missing perspective:**  
[An expert lens or stakeholder view the article currently lacks]

**Evidence the panel would demand:**  
[The 2-4 pieces of evidence or analysis needed to make the argument credible]

**Meeting question:**  
[The one expert-inspired question worth discussing live]
```

### Panel Attachment Format

Use this format for the attachment:

````markdown
# Attachment: Virtual Expert Panel

## Topic
[Article topic and core question]

## Invited Expert Lenses
- [Person]: [framework] - [why selected]

## Round 1: Definitions and First Principles
[Moderator opening and expert views]

## Round 2: Core Disagreement
[Dynamic responses]

```text
[ASCII structure map]
```

## Round 3: Implications for the Article
[Challenges, synthesis, and editorial implications]

## Knowledge Network
```text
[Concept map showing claims, evidence, tensions, and open questions]
```

## Open Questions for the Authors
- [Question]
````

## Part 3: Editor's Checklist

Use mature editorial practice to test whether the article is ready for a top economic media column.

Check:

- **Commission**: Is the piece doing the job it was meant to do for this publication and audience?
- **Thesis**: Can the core claim be stated in one strong sentence?
- **News value**: Why should this be read now?
- **Originality**: What does the article add beyond familiar commentary?
- **Reader payoff**: What will the reader understand, question, or remember?
- **Lead and nut graf**: Does the opening create momentum and quickly reveal the point?
- **Structure**: Does each section advance the argument rather than repeat it?
- **Evidence**: Are important claims supported by data, examples, reporting, or credible reasoning?
- **Fairness**: Are counterarguments represented honestly?
- **Causality**: Does the piece avoid confusing correlation, narrative plausibility, and proof?
- **Voice**: Does the prose sound like the author, not a generic analyst?
- **Precision**: Are key terms, numbers, institutions, and timeframes accurate?
- **Risk**: Are legal, reputational, factual, or overclaiming risks visible?
- **Ending**: Does the piece land with implication, not just summary?
- **Headline potential**: Is there a clear headline/deck angle?

## Pre-Meeting Review Template

Use this format for the main review:

```markdown
## Pre-Meeting Editorial Review

**Thesis:** [What the article is really arguing]
**Reader payoff:** [Why the target reader should care]
**Recommended meeting decision:** [Publish / revise / restructure / split / hold]
**One-line editorial judgment:** [The most important thing both authors should know before discussion]

### 1. Strategic Article Review
- Q1 - What is the article's answer? [Answer-first / pyramid principle]
- Q2 - So what? [Stakes, timing, reader value]
- Q3 - Is the structure logically clean? [MECE diagnosis]
- Q4 - What is the issue tree behind this article? [Issue tree]
- Q5 - How strong is the evidence? [Evidence hierarchy]
- Q6 - What is the problem-solving path? [7-step problem solving]
- Q7 - What should we discuss in the meeting? [Strategic synthesis]

### 2. Expert Panel Takeaway
**Panel selected:** [3-5 expert lenses and why]
**Sharpest challenge:** [Single most important critique]
**Best deepening opportunity:** [Best way to make the article stronger]
**Missing perspective:** [Important absent lens or stakeholder view]
**Evidence the panel would demand:** [2-4 pieces of evidence or analysis]
**Meeting question:** [One expert-inspired question worth discussing live]
**See attachment:** `Virtual Expert Panel`

### 3. Editor's Checklist
- Must fix: [Blocking editorial issue]
- Strengthen: [High-value improvement]
- Watch risk: [Factual, legal, reputational, or overclaiming risk]

### Meeting Questions
- [Question that helps the authors decide direction, not just react]

### Suggested Meeting Agenda
1. [Decision or tradeoff to resolve]
2. [Revision priority to confirm]
3. [Next article or follow-up idea to discuss]
```

## Planning Template

Use this format when preparing next-topic discussion:

```markdown
## Column Plan

### Candidate Topics
- Topic: [Working title]
  Angle: [Distinct point of view]
  Timeliness: [Why now]
  Evidence needed: [Data, cases, interviews, reports]
  Expert lenses to consult: [Possible virtual panel]
  Risk: [What could make this weak or repetitive]

### Recommended Next Piece
**Working title:** [Title]
**Core claim:** [One-sentence argument]
**Why this now:** [Timing or editorial hook]
**Structure:** [3-5 section outline]
**Inputs needed:** [Materials to gather]
**Owner and deadline:** [Who does what by when]
```

## Output Style

- Be direct, strategic, editorial, and calm.
- Prefer short sections and concrete bullets in the main review.
- Put detailed expert debate in the attachment, not the main review.
- Use "Editorial Judgment", "Strategic Diagnosis", "Expert Panel Takeaway", and "Meeting Questions".
- When asked to rewrite, explain the editorial intention before or after the rewrite.
- When the draft is missing, ask for the article text, target publication context, meeting goal, and desired depth of feedback.
