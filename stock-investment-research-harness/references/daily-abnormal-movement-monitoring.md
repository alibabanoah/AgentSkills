# Daily Abnormal Movement Monitoring

Use this reference when the user asks to scan A-share or Hong Kong market daily movers, post-close abnormal stocks, limit-up/limit-down names, unusual volume, sector surges, sharp drawdowns, or event-driven opportunities.

## Principle

Abnormal movement is a research entry point, not an investment thesis. Start from the market move, then identify the cause, test whether it changes fundamentals or risk premium, and classify the stock.

Required chain:

```text
abnormal move -> source verification -> immediate catalyst -> policy/news/industry/company linkage -> market confirmation -> fundamental impact -> valuation/risk implication -> research classification
```

Do not treat a 10% rise or fall as meaningful by itself. Explain whether the movement reflects real information, liquidity, crowding, speculation, forced selling, or broad sector rotation.

## Daily scan scope

Default market scope when the user does not specify:

- A-shares: Shanghai, Shenzhen, Beijing exchanges, including main board, STAR, ChiNext, and BSE where data is available.
- Hong Kong: Main Board and major liquid small/mid caps; prioritize Hang Seng Composite, Hang Seng Tech, sector leaders, Southbound Connect names, and high-turnover movers.

For each market, run the scan after the local close or clearly state if using intraday/partial data.

## Abnormal movement triggers

Use a combination of triggers. Do not rely on only price change.

Price triggers:

- A-shares: limit-up, limit-down, close near limit, daily move >= 8%, or board-specific large move; for STAR/ChiNext/BSE, use larger board-appropriate thresholds where price limits differ.
- Hong Kong: daily move >= 8% for liquid large/mid caps, >= 12% for smaller names, or any sharp move with unusually high turnover.
- gap up/down, intraday reversal, multi-day consecutive rise/fall, or break of major 20/60/120-day range.

Volume and liquidity triggers:

- turnover value ranking near market top
- volume or turnover >= 2x-3x recent 20-day average
- abnormal turnover rate relative to float
- block trades, buybacks, insider/major-shareholder changes, Southbound/Northbound flow shock when relevant

Sector and market-structure triggers:

- stock moves with sector index or theme basket
- multiple upstream/downstream names move together
- leader moves first and second-tier names follow
- one stock diverges sharply from peers
- ETF/fund style rotation affects the group

Event triggers:

- earnings surprise, guidance revision, profit warning, dividend/buyback, restructuring, M&A, asset sale, spin-off
- regulatory inquiry, penalty, investigation, litigation, audit issue, resignation, trading halt/resumption
- policy document, subsidy, tender/procurement, industry rule, price change, export control, sanction, tariff
- product approval/failure, safety incident, order win/loss, capacity change, supply-chain disruption
- rumor-driven moves must be labeled and not used as thesis proof without confirmation

## Source priority for daily movers

Use `source-standards.md` first. For daily mover work, prioritize official market data, company announcements, exchange disclosures, regulator notices, official policy documents, credible named reporting, sector data, and price/volume/valuation sources.

For A-shares, verify with CNINFO, SSE/SZSE/BSE disclosures, exchange inquiry letters, CSRC/regulator notices, official policy releases, and company announcements. For Hong Kong, verify with HKEXnews, company announcements, SFC/HKMA/regulator releases, and Stock Connect/Southbound context where relevant.

## A-share daily mover logic

A-share abnormal moves often reflect policy, liquidity, theme rotation, or event-driven speculation before earnings confirmation. Analyze whether the move is a real policy/industry signal or only a theme label; whether local implementation, orders, tenders, subsidies, or official documents confirm the theme; whether the company is a leader or a weak peripheral concept stock; limit-up/limit-down quality; ST/delisting risk; inquiry letters; pledge pressure; shareholder reduction; lock-up expiry; weak disclosure; and whether fundamentals can catch up with valuation after the move.

Prefer A-share movers that combine policy/industry confirmation with company-level evidence and reasonable valuation. Treat pure limit-up themes without evidence as watchlist or avoid.

## Hong Kong daily mover logic

Hong Kong abnormal moves often reflect earnings, liquidity, Southbound flows, global rates, China macro expectations, short covering, sector repricing, or low-liquidity gaps. Analyze whether the stock is liquid enough for the move to be reliable; whether the move is driven by company news, sector beta, China macro, US rates, ADR spillover, or Southbound flow; whether valuation has reset enough relative to fundamentals; and whether the move is only a technical rebound from oversold levels.

For low-liquidity Hong Kong names, raise the evidence bar and avoid treating sharp percentage moves as investment signal by default.

## Classification workflow

For each abnormal mover, classify:

- `Event-confirmed opportunity`: move backed by official announcement, earnings, policy implementation, or operating data.
- `Policy/industry watchlist`: policy or sector logic is plausible, but company-level evidence is incomplete.
- `Valuation repair candidate`: sharp fall or long drawdown where risk is clearing and valuation becomes researchable.
- `Momentum/crowding risk`: move mostly driven by theme, liquidity, limit-up behavior, or short squeeze without fundamental confirmation.
- `Red-flag avoid`: accounting, governance, regulatory, liquidity, ST/delisting, pledge, or fraud-like risk dominates.
- `Needs more evidence`: source support is weak or contradictory.

## Required analysis for selected movers

For each selected stock, include market, ticker, name, abnormal trigger, verified cause, source quality, causal chain, sector/peer context, fundamental impact, investment classification, and what would confirm or falsify the signal.

## Daily report shape

Produce a shortlist rather than every mover. Default to top 5-10 A-share movers worth investigating, top 5-10 Hong Kong movers worth investigating, a separate high-risk/speculative group, one or two deeper cases when the causal chain is strong, and next-session triggers.
