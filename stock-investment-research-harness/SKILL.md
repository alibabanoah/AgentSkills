---
name: stock-investment-research-harness
description: Orchestrate a public-market stock investment research and portfolio risk-monitoring workflow using authoritative public sources, causal macro/geopolitical reasoning, and the user's preference for large established companies, buy-low-sell-high discipline, and exceptional high-growth leaders. Use when the user asks for stocks worth researching or investing in, recent investable opportunities, ticker-by-ticker equity analysis, portfolio holding reviews, recurring risk checks, risk alerts, watchlists, valuation/thesis memos, or deep analysis of how policies, geopolitics, macro data, news, and market reactions affect stocks.
---

# Stock Investment Research Harness

Use this skill as the controller for equity research and holding-risk surveillance. Produce research, not personalized financial advice or trade execution instructions. Treat every output as dated, evidence-based, and uncertain.

## User Investment Preferences

Apply these as the default investor mandate unless the user says otherwise:

- Prefer "buy low, sell high" opportunities where a strong company has a temporary valuation reset, market overreaction, or fixable near-term pressure.
- Prefer large, established companies with an existing business base, proven demand, liquidity, durable competitive position, and enough public disclosure to analyze.
- De-prioritize small companies, thinly traded stocks, penny stocks, concept-only businesses, or companies whose thesis depends mainly on distant optionality.
- Allow an exception for high-growth industry leaders when the sector has a strong structural tailwind and the company has clear leadership, execution evidence, and expanding fundamentals. In these cases, buying near highs can still be researchable, as with Nvidia-like AI infrastructure leadership, but only after testing growth durability, valuation scenarios, market expectations, and downside risk.
- When ranking candidates, favor mature quality companies at reasonable or temporarily depressed valuations first, then high-growth leaders with exceptional evidence, then speculative or smaller names only if explicitly requested.
- State when a candidate conflicts with these preferences and why it is still worth monitoring, if applicable.

## Core References

- Read `references/source-standards.md` before any task that uses recent facts, financial data, filings, macro data, or news.
- Read `references/research-methodology.md` when explaining how a new-stock thesis is produced, when building or auditing the research method, or when the user asks why a stock made the list.
- Read `references/macro-geopolitical-analysis.md` when the task requires current international news, geopolitical events, macro policy, war/conflict, sanctions, tariffs, elections, supply-chain disruption, commodity shocks, FX/rates moves, cross-asset risk analysis, or deep reasoning about how policies and events interact.
- Read `references/a-share-market-strategy.md` when the task involves Mainland China A-shares, Chinese domestic policy, A-share sector rotation, China industry-chain analysis, or adapting strategy away from US-style value investing.
- Read `references/research-pipeline.md` when screening for new stock ideas, building a watchlist, or writing a deep stock thesis.
- Read `references/portfolio-monitoring.md` when the user gives held tickers, positions, cost basis, allocation, or asks for ongoing/periodic risk checks.
- Read `references/report-templates.md` when producing the final output, alert, memo, or recurring update format.

## Harness Pipeline

1. Intake: identify market, tickers, objective, horizon, risk tolerance, constraints, and whether the task is new-idea research or existing-holding monitoring.
2. Source: gather current public information from authoritative public sources first: company filings, investor relations materials, exchange disclosures, regulators, official macro/statistical agencies, and reputable named reporting. Use weaker sources only as leads or sentiment, never as thesis proof.
3. Normalize: separate verified facts, estimates, market expectations, and analyst interpretation.
4. Map macro and geopolitical context when relevant: build a causal logic chain across policies, geopolitics, news, macro variables, sectors, companies, market reaction, second-order effects, and scenario risks. Do not stop at information aggregation.
5. Form thesis: convert facts into a falsifiable investment thesis with explicit value drivers.
6. Analyze: evaluate business quality, financials, valuation, catalysts, risks, market structure, and portfolio fit.
7. Decide: classify as research candidate, watchlist, avoid, hold-review, trim-review, or urgent-risk-review. Avoid direct instructions like "buy now" or "sell now."
8. Communicate: use a concise memo with evidence, confidence level, key assumptions, and what would change the view.
9. Monitor: define triggers, update cadence, and alert thresholds for holdings or watchlist names.
10. Iterate: when new data arrives, update the thesis instead of repeating old conclusions.

## Routing Rules

- If the user asks in Chinese or English for recent stocks worth investing in, stock opportunities, or help finding stocks, run new-idea research through `research-pipeline.md`.
- If the user gives tickers they already own, a portfolio list, cost basis, or asks in Chinese or English about risk, warnings, or periodic analysis, run holding monitoring through `portfolio-monitoring.md`.
- If the user asks for both new opportunities and current holdings, do holding monitoring first, then new-idea research. Protect existing capital before expanding risk.
- If the user asks for a single ticker, produce a deep equity memo and include whether it belongs in watchlist, existing-holding review, or avoid/research-later.
- If the user asks for urgent alerts, prioritize material events: earnings surprises, guidance cuts, regulatory/legal events, liquidity stress, credit downgrades, accounting issues, executive departures, major product failures, geopolitical exposure, or extreme price/volume moves.
- If the user asks to connect international events, policies, news, stock prices, and risk points, run `macro-geopolitical-analysis.md` before final stock-level conclusions and produce a causal explanation, not a news digest.
- If the user asks about A-shares, do not directly apply US-style value investing. Use `a-share-market-strategy.md` to analyze policy cycle, industry-chain position, market style, liquidity, governance/disclosure risk, and whether a value, dividend, cycle, policy leader, or strategic-substitution strategy fits better.

## Source And Freshness Discipline

- Always state the "as of" date for market-sensitive conclusions.
- Browse for current prices, market cap, earnings dates, filings, guidance, news, analyst consensus, macro rates, commodity prices, or sector data.
- Prefer primary sources: company filings, exchange disclosures, investor presentations, earnings releases, transcripts, regulator documents, and official macro/statistical agencies.
- Use secondary sources to triangulate, not to replace primary evidence.
- Reject or label rumor, anonymous social-media claims, promotional content, unsourced screenshots, and single-source claims that lack primary or reputable confirmation.
- Cite or name sources in the answer when making factual claims.
- Mark unsupported, stale, or unavailable information as unknown. Do not invent financial metrics, dates, management quotes, or catalysts.

## Output Discipline

Use clear labels:

```text
Research stage: source intake -> quality review -> valuation and catalysts -> risk check -> conclusion tier -> monitoring triggers
```

For investment opportunity research, return:

- candidate list with ranking logic
- thesis summary
- key evidence
- valuation view
- catalysts
- risks
- what would falsify the thesis
- next monitoring date or trigger

For existing holdings, return:

- ticker-by-ticker risk level
- what changed recently
- position-specific risk if allocation/cost basis is known
- alert triggers
- action framing as review categories, not trade commands

## Guardrails

- Do not present analysis as guaranteed return, insider information, or individualized financial advice.
- Do not recommend leveraged, options, short-selling, penny-stock, or highly speculative actions unless the user explicitly asks and risks are made prominent.
- Do not rely only on price movement or social-media attention as an investment thesis.
- Do not hide uncertainty. Use confidence levels and list missing data.
- When the user asks for "best stocks", translate that into "best candidates for further research under stated assumptions."
