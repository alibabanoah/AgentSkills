---
name: ai-tech-content-research-harness
description: Orchestrate an AI technology and frontier-trend content research workflow for self-media creators. Use when the user wants to discover AI/technology topics, track tech founders and investors, verify information sources, analyze AI education/career/creator trends, reverse-engineer viral tech content, generate topic angles, or transform authoritative AI tech information into compelling but fact-safe secondary content.
---

# AI Tech Content Research Harness

Use this skill as the controller for AI technology trend research and self-media topic production. The goal is to turn reliable frontier information into attractive, understandable, and platform-ready content without fabricating facts.

## Core References

- Read `references/source-map.md` when collecting AI tech, founder, investor, company, research, education, career, or creator-economy information.
- Read `references/influencer-and-investor-tracking.md` when tracking Elon Musk, Sam Altman, Jensen Huang, Mark Zuckerberg, AI investors, tech founders, labs, VCs, and public-market technology narratives.
- Read `references/topic-discovery.md` when finding topics, scoring whether a lead is worth writing, or building a topic calendar.
- Read `references/fact-verification.md` before using strong claims, statistics, quotes, controversy, company facts, research findings, or viral screenshots.
- Read `references/scheduled-topic-monitoring.md` when running daily or recurring topic monitoring across AI tech sources, media, founders, investors, papers, social platforms, education, jobs, and creator cases.
- Read `references/narrative-transformation.md` when turning source material into a strong self-media angle, story, script, article, or short-video structure.
- Read `references/secondary-creation-stylebook.md` when choosing the secondary-creation voice, expression type, intensity level, platform format, or rewrite style for AI tech content.
- Read `references/attention-and-platform-packaging.md` when writing titles, hooks, covers, short-video openings, Xiaohongshu notes, WeChat articles, or other platform-specific packaging.

## Harness Pipeline

1. Intake: identify target audience, platform, content format, topic domain, desired tone, risk tolerance, and whether the task is trend discovery, source research, topic selection, or final content creation.
2. Source: gather authoritative and timely sources first, then use social platforms and creator posts as leads rather than proof.
3. Verify: classify every important claim as confirmed fact, credible report, interpretation, speculation, or unsupported rumor.
4. Map signal: identify why the information matters for ordinary people, education, career, investment attention, creators, companies, or social change.
5. Build angle: convert raw information into a content thesis with conflict, stakes, audience relevance, and one clear takeaway.
6. Deepen: connect the topic to a broader mechanism such as AI replacing tasks, education changing, jobs restructuring, capital allocation, creative democratization, or tech-giant strategy.
7. Style: choose the secondary-creation style, expression intensity, and platform format.
8. Package: create an attractive hook, title, cover line, outline, and platform-specific expression while preserving factual boundaries.
9. Risk-check: remove false certainty, fake quotes, unsupported statistics, defamatory claims, and misleading exaggeration.
10. Output: deliver a topic memo, content outline, script, article, platform package, or source brief with citations or source names.
11. Iterate: update source lists, recurring topic buckets, and successful narrative patterns based on performance feedback.

## Routing Rules

- If the user asks where a tech creator gets information, run `source-map.md` and `topic-discovery.md`.
- If the user gives raw notes, links, titles, or transcripts and asks for analysis, identify the source type, narrative pattern, audience promise, and reusable content mechanism.
- If the user asks for AI frontier topics, track AI labs, founders, investors, funding, product launches, papers, benchmarks, regulations, job-market data, and viral creator cases.
- If the user asks for a daily plan, recurring monitoring task, or "today's topics", run `scheduled-topic-monitoring.md` first, then verify the strongest candidates with `source-map.md` and `fact-verification.md`.
- If the user asks about famous people such as Musk, Altman, Huang, Zuckerberg, or major VCs, run `influencer-and-investor-tracking.md` and verify quotes from original posts, interviews, filings, or full videos when possible.
- If the user asks to write, rewrite, polish, adapt, imitate a content style, or create a post/script, run source verification first, then `narrative-transformation.md`, `secondary-creation-stylebook.md`, and `attention-and-platform-packaging.md`.
- If the user asks for moderate attention-grabbing exaggeration, translate it into sharper framing, stronger contrast, vivid metaphors, and audience stakes. Do not exaggerate facts, numbers, quotes, causality, or certainty.

## Default Content Thesis Pattern

Use this pattern unless the user requests another structure:

```text
fresh signal -> hidden mechanism -> ordinary-person impact -> tension or controversy -> practical takeaway
```

Examples of valid mechanisms:

- AI lowers the cost of producing courses, videos, code, design, analysis, and simulations.
- AI shifts career value from execution to business understanding, taste, judgment, workflow design, and source verification.
- Tech capital prefers scalable systems over slow human training, creating education and job-market tension.
- Founder/investor narratives move public attention before facts are fully reflected in institutions or markets.
- Individual creators can use AI to bypass old production bottlenecks, but taste and originality become scarcer.

## Output Discipline

For topic research, return:

- source lead
- source reliability
- why it matters
- audience pain or curiosity
- possible angle
- verification gaps
- content risk
- recommended format

For content drafts, return:

- title options
- opening hook
- core thesis
- evidence chain
- story structure
- audience takeaway
- fact-risk notes
- platform packaging suggestions

## Guardrails

- Do not fabricate sources, statistics, quotes, companies, papers, or events.
- Do not convert social-media rumors into confirmed facts.
- Do not use "AI will definitely replace everyone" or similar certainty unless the source and scope support it.
- Do not defame named people or companies; describe claims as reported, alleged, disputed, or unverified when needed.
- Do not use fear-based packaging unless there is a concrete mechanism and practical takeaway.
- Use attention ethically: amplify relevance and contrast, not falsehood.
