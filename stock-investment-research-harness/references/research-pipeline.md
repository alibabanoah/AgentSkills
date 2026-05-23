# New-Idea Research Pipeline

Use this workflow when the user asks for stocks worth researching or investing in.

## 1. Define the mandate

Identify or infer:

- market: US, A-share, HK, global, or unspecified
- horizon: short term, 6-18 months, 3-5 years, income, special situation
- risk tolerance: conservative, balanced, aggressive, unknown
- exclusions: sectors, market cap, leverage, China/ADR exposure, ESG, liquidity

If missing, proceed with a balanced long-only public-equity assumption and state it. Apply the user's default preference for large, established companies and "buy low, sell high" value discipline unless the user gives a different mandate.

When the market is Mainland China A-shares, read `a-share-market-strategy.md` and apply the A-share source priority and risk checks from `source-standards.md` before ranking candidates. Do not directly apply US-style value investing. Pay special attention to policy cycle, industry-chain position, market style, liquidity, disclosure quality, ownership/control structure, ST/delisting risk, pledged shares, related-party transactions, regulatory inquiry letters, and cash-flow quality.

Default preference screen:

- First look for large, established companies with durable demand, strong disclosure, adequate liquidity, and a real operating base.
- Prefer temporary valuation resets, market overreactions, or cyclical pressure in otherwise high-quality companies.
- Avoid making small-cap, thinly traded, penny-stock, or concept-stage companies top candidates unless explicitly requested.
- Treat high-growth industry leaders as a separate exception bucket: they may be researchable even near highs only when structural demand, competitive leadership, execution evidence, and valuation scenario support are unusually strong.

## 2. Build candidate universe

Use multiple idea sources, not a single screen:

- quality compounders: durable revenue growth, high margins, strong returns on capital, clean balance sheet
- valuation resets: good business with temporary drawdown, multiple compression, or sector selloff
- catalyst-driven names: earnings inflection, product cycle, regulatory approval, restructuring, capital return, margin recovery
- macro/sector beneficiaries: rate cycle, AI/cloud, energy, healthcare, defense, financials, consumer recovery, commodities
- defensive/income names: stable cash flow, dividends, regulated or recurring revenue

Avoid making "recent popularity" the main reason.

For high-growth themes such as AI infrastructure, do not reject a leader only because price is near a high. Instead test whether the company resembles a true category leader with compounding fundamentals, not a short-lived narrative.

For Mainland China A-shares, build the candidate universe from A-share-specific strategy buckets:

- policy-supported quality leaders with implementation evidence
- valuation repair after risk clearing
- industry-cycle inflection
- high-dividend, central-SOE, or cash-return names
- technology self-reliance and strategic substitution
- consumption or domestic-demand recovery
- theme rotation or event-driven watchlist names, only when fundamentals or policy implementation can be verified

## 2A. Produce the research thesis

Before ranking a candidate, create a thesis chain:

```text
observable facts -> business interpretation -> value drivers -> valuation implication -> catalysts -> risk/falsification tests
```

Require each thesis to answer:

- What does the market appear to be underestimating or overestimating?
- Which value driver matters most: growth, margin, reinvestment runway, return on capital, balance-sheet risk, terminal durability, or capital return?
- Which macro or geopolitical event could change the value driver, if any?
- What evidence supports that driver?
- What time horizon is needed for the market to recognize it?
- What would prove the thesis wrong?

If this chain cannot be completed, classify the stock as watchlist or avoid-for-now rather than a high-priority research candidate.

## 3. First-pass filters

Reject or de-prioritize candidates with:

- unclear business model or poor disclosure
- severe liquidity or solvency risk
- valuation that only works under extreme growth assumptions
- major unresolved accounting, legal, or regulatory red flags
- single-customer or single-product dependency without compensation in valuation

## 4. Deep analysis framework

For each finalist, analyze:

- macro/geopolitical context: event chain, transmission channels, affected sectors, cross-asset signals, and scenario risks when relevant
- business model: what it sells, to whom, pricing power, moat, cyclicality
- financial quality: revenue growth, gross/operating margin, free cash flow, ROIC/ROE, leverage, dilution
- management/capital allocation: buybacks, dividends, M&A, stock compensation, guidance credibility
- valuation: historical multiples, peer comparison, DCF or scenario valuation when useful
- catalysts: upcoming earnings, product launches, regulatory decisions, macro shifts, cost cuts, balance-sheet events
- risk: downside case, thesis killers, crowded positioning, narrative risk
- fit: why this name is better than alternatives in the same theme

Tie every section back to the thesis chain. Do not allow valuation, catalyst, or risk sections to float independently from the original thesis.

When current international events may affect the stock, read `macro-geopolitical-analysis.md`. Do not force macro narratives onto companies with low exposure. State when the linkage is weak or speculative.

## 5. Ranking method

Rank candidates with transparent factors:

- evidence strength
- upside/downside asymmetry
- quality of business
- valuation reasonableness
- catalyst clarity
- risk severity
- confidence level

Use categories:

- `A: high-priority research candidate`
- `B: watchlist / wait for better price or evidence`
- `C: interesting but high risk`
- `D: avoid for now`

## 6. Required final shape

Produce a shortlist rather than a long undifferentiated list. Include:

- top candidates and why they made the list
- names rejected and why, when useful
- scenario table: base, upside, downside
- key dates to monitor
- missing information that would improve confidence

End with "what would change the view" instead of a blanket recommendation.
