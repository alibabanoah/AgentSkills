# Portfolio Monitoring Workflow

Use this workflow when the user provides held tickers or asks for regular risk analysis.

## Intake fields

Ask only when necessary; otherwise analyze what is available.

- ticker and exchange
- position size or portfolio weight
- cost basis
- holding period and intended horizon
- reason for owning it
- tax or liquidity constraints
- alert preference: urgent only, weekly, monthly, earnings-driven

If position size and cost basis are missing, provide company-level risk and say position-level risk cannot be assessed.

## Monitoring cadence

Default cadence:

- urgent alert: material event or severe price/volume move
- weekly: news, price action, estimate changes, sector developments
- quarterly: earnings, guidance, balance sheet, cash flow, valuation reset
- annual: long-term thesis, competitive position, capital allocation, governance

## Risk levels

Classify each holding:

- `Green`: thesis intact; no material new risk found
- `Yellow`: monitor closely; new risk or valuation pressure exists
- `Orange`: active review; thesis impairment possible
- `Red`: urgent review; material adverse change, liquidity/accounting/regulatory shock, or severe downside scenario

Do not translate colors into automatic buy/sell commands.

## Risk dimensions

Check:

- macro/geopolitical: war, sanctions, tariffs, elections, policy shocks, supply-chain disruption, commodity shock, FX/rates shock, cross-border capital controls
- fundamental: revenue, margins, cash flow, leverage, guidance, customer demand
- valuation: multiple expansion/compression, peer gap, rate sensitivity
- event: earnings, litigation, regulatory decisions, product launches, M&A
- financial health: debt maturity, interest burden, covenants, liquidity, dilution
- market behavior: drawdown, volatility, volume spike, correlation with sector
- portfolio concentration: oversized single name, theme crowding, factor exposure
- narrative: expectations too high, thesis dependent on one catalyst, sentiment reversal

## Alert triggers

Issue an alert-style update when any condition appears:

- international event creates a direct revenue, cost, supply-chain, financing, sanctions, commodity, or FX channel for the holding
- company cuts guidance, misses key metric, or withdraws forecast
- auditor resigns, filing delayed, restatement, material weakness
- CEO/CFO departure without clear succession
- regulator investigation, major lawsuit, product ban, safety issue
- credit downgrade, refinancing risk, covenant breach, liquidity stress
- position falls materially more than sector/market with company-specific cause
- valuation becomes disconnected from fundamentals or original thesis
- concentration risk exceeds user-stated limits

## Holding review output

For each ticker, include:

- current risk level
- recent changes
- thesis status: intact, weakened, broken, unclear
- main risks ranked by severity
- next evidence to watch
- review category: keep monitoring, reassess thesis, reduce-risk review, urgent-risk review

For portfolio-level review, add:

- concentration map
- sector/theme exposure
- correlated downside scenario
- missing data
- suggested monitoring calendar
