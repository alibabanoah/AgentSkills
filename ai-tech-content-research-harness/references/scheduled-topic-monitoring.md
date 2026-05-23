# Scheduled Topic Monitoring

Use this reference when running a daily or recurring task to discover AI technology self-media topics from many information sources.

## Principle

Do not try to deeply read the whole internet. Use a layered signal system:

```text
wide signal collection -> rule-based filtering -> scoring -> verification -> topic classification -> content recommendation
```

The goal is to compress many daily signals into a small set of reliable, high-potential topics.

## Daily signal collection

Collect from these buckets:

- AI company official releases: OpenAI, Anthropic, Google DeepMind, Meta AI, xAI, Nvidia, Microsoft, Apple, Amazon, DeepSeek, MiniMax, Alibaba Qwen, ByteDance, Baidu, Huawei, Tencent, Zhipu, Moonshot.
- Founder and investor signals: Elon Musk, Sam Altman, Jensen Huang, Mark Zuckerberg, Satya Nadella, Sundar Pichai, Demis Hassabis, Dario Amodei, a16z, Sequoia, YC, Khosla, Founders Fund, major AI investors.
- Papers, open source, and benchmarks: arXiv, GitHub Trending, Hugging Face, Papers With Code, LMSYS/Chatbot Arena, SWE-bench, MLPerf, major conference papers.
- Technology and business media: The Information, Bloomberg, Reuters, FT, WSJ, The Verge, Wired, TechCrunch, MIT Technology Review, 36Kr, LatePost, Caixin, QbitAI, Machine Heart, InfoQ, GeekPark.
- Social and community signals: X/Twitter, YouTube, Bilibili, Xiaohongshu, Douyin, Product Hunt, Hacker News, Reddit, Discord, Substack, WeChat public accounts.
- Education, career, and capital signals: labor data, hiring/layoff signals, education AI tools, AI creator cases, funding rounds, investor memos, consulting reports.

Use social platforms for early signals and audience language. Use primary or authoritative sources for proof.

## First-pass filter

A signal enters the candidate pool only if it satisfies at least two or three of these conditions:

- Fresh: appeared within 24-72 hours, or an older event suddenly regained attention.
- Authoritative: comes from official source, paper, founder/investor original statement, reputable media, or institution.
- Counterintuitive: challenges common belief or reveals a hidden reversal.
- Broad impact: affects education, jobs, creation, business, investment attention, parenting, learning, or ordinary people.
- Famous person or institution: involves major founders, investors, labs, universities, regulators, or influential companies.
- Concrete case: includes a named company, tool, creator, school, job role, product, research result, or policy.
- Tension: contains conflict such as technology efficiency vs human value, capital efficiency vs education fairness, tool adoption vs skill devaluation.
- Translatable: can be explained clearly to non-experts.
- Actionable: gives the audience something to watch, learn, avoid, rethink, or try.

Reject or delay if the signal is only a vague hot word, pure opinion, unverified rumor, copied quote, or technical detail with no audience relevance.

## Scoring model

Score each candidate from 1-5:

- Freshness
- Authority
- Conflict
- Ordinary-person relevance
- Mechanism depth
- Spread potential
- Fact risk

Interpretation:

- `>=24`: priority topic for today.
- `20-23`: watchlist or secondary topic.
- `<20`: do not write today.
- High fact risk: downgrade unless primary verification is available.

Fact risk is not a positive factor. If scoring numerically, subtract or flag it separately. A high-risk topic can be exciting but should not be published until verified.

## Verification gate

Before recommending publication, check:

- Can the core fact be verified?
- Is the original source available?
- Is the quote exact or paraphrased?
- Are numbers scoped by geography, time, sample, and method?
- Is causality supported, or only inferred?
- Is the content legally or reputationally risky?

If verification fails, output a research task rather than a publishable topic.

## Topic classification

Classify daily candidates:

- `Today's priority`: strong source, strong angle, strong audience relevance.
- `Short-video candidate`: one case, one conflict, one clear takeaway.
- `Deep article candidate`: complex mechanism, multiple sources, structural impact.
- `Observation pool`: interesting but needs more proof or timing.
- `High-risk/unverified`: attractive but not publishable yet.

Default daily output:

- 1-2 priority topics
- 2-3 short-video candidates
- 1-2 deep article candidates
- several observation items
- high-risk/unverified list

## Topic worthiness chain

A topic is worth publishing when it can form this chain:

```text
new event -> verifiable fact -> hidden mechanism -> ordinary-person impact -> strong framing -> safety boundary
```

Do not write if:

- there is heat but no mechanism
- there is emotion but no fact
- there is a technical detail but no audience relevance
- there is a famous person but no new signal
- there is a strong claim but no verification

## Daily report template

Use this shape:

```text
As of: YYYY-MM-DD
Monitoring scope:

Executive summary
- strongest signal:
- strongest ordinary-person impact:
- main risk:

Priority topics
| Rank | Topic | Source | Score | Angle | Format | Verification status | Risk |

Short-video candidates
- Topic:
- Hook:
- One-sentence mechanism:
- Source:

Deep article candidates
- Topic:
- Source chain:
- Mechanism:
- Audience impact:

Observation pool
- Item:
- Why monitor:
- What would upgrade it:

High-risk / unverified
- Claim:
- Why risky:
- Verification needed:

Recommended next action
- write now:
- verify first:
- monitor:
```
