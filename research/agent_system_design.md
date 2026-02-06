# Agent System Design: Ongoing Research Pipeline

*Each agent has a specific role, runs on a schedule, and writes to a specific file.*

---

## The 8 Agents

### Agent 1: INSIDER TRACKER
**Role:** Track what politicians, hedge funds, and company executives are buying/selling in our watchlist names.
**Frequency:** Weekly
**Data Sources:**
- Capitol Trades (politician trades)
- Quiver Quantitative (congress + hedge funds)
- Unusual Whales (options flow + congress)
- SEC Form 4 filings (company insider buys/sells)
- 13F filings (quarterly hedge fund positions)
**Output:** `research/weekly/insider_trades_YYYY-MM-DD.md`
**Key Questions:**
- Did any politician buy/sell our stocks this week?
- Did any company executive buy their own stock? (Strongest bullish signal)
- Did any major hedge fund file a new position in our names?
- Are 13F filings due? What did they show?
**Why we missed this:** We tracked Pelosi and Sen. King but never checked what the COMPANY INSIDERS at SDGR, VST, VRT, etc. are doing with their own shares.

---

### Agent 2: CATALYST CALENDAR
**Role:** Track every upcoming event that could move our stocks.
**Frequency:** Weekly update, daily scan during earnings season
**Data Sources:**
- Earnings calendars (Yahoo Finance, Nasdaq)
- FDA calendar (ClinicalTrials.gov, FDA.gov)
- Conference schedules (JPM Healthcare, CES, etc.)
- Company IR pages for investor day dates
**Output:** `research/catalysts.md` (running document)
**Key Dates We Already Know:**
- Feb 26, 2026: DUOL earnings
- H1 2026: SDGR SGR-3515 data
- H2 2026: ABSI ABS-202 interim data
- 2026: RLAY RLY-2608 Phase 3 completion
- Q2 2026: FDA final guidance on AI in drug development
- Mid-Feb 2026: Q4 2025 13F filings drop
- Quarterly: VST, VRT, ETN earnings
**Why we missed this:** We had scattered dates but no single calendar. DUOL earnings in 3 weeks and we almost didn't flag it.

---

### Agent 3: TECHNICAL SCANNER
**Role:** Check price action, support/resistance levels, RSI, moving averages for our portfolio.
**Frequency:** Weekly (daily during volatile periods)
**Data Sources:**
- TradingView or Finviz for charts
- Key moving averages (50-day, 200-day)
- RSI (overbought >70, oversold <30)
- Volume analysis (unusual volume = something happening)
**Output:** `research/weekly/technicals_YYYY-MM-DD.md`
**Key Questions:**
- Is any of our stocks oversold (RSI <30)? Could be a buy signal.
- Is any approaching a key support/resistance level?
- Any unusual volume spikes? (Institutions moving)
- Are we buying into a downtrend or an uptrend?
**Why we missed this:** We looked at fundamentals only. Price action tells you WHEN to buy, not just WHAT.

---

### Agent 4: MACRO MONITOR
**Role:** Track the big picture that affects EVERYTHING in our portfolio.
**Frequency:** Weekly
**Data Sources:**
- Federal Reserve announcements, FOMC minutes
- US Treasury yields (10-year)
- EUR/USD exchange rate (critical for Estonian investor!)
- Recession indicators (yield curve, unemployment, PMI)
- VIX (fear index)
- Hyperscaler CapEx guidance (any slowdown = energy thesis at risk)
**Output:** `research/weekly/macro_YYYY-MM-DD.md`
**Key Questions:**
- Where are interest rates heading? (Pre-revenue stocks like RLAY get crushed by high rates)
- EUR/USD: should I wait for a stronger euro before converting?
- Any recession signals? Defensive positioning needed?
- Did any hyperscaler cut CapEx guidance? (Kills VST, VRT, ETN thesis)
- VIX elevated? Broad market fear = buying opportunity or warning?
**Why we missed this:** We analyzed stocks in isolation. A rate hike or recession changes EVERYTHING regardless of how good our picks are. Also: the user lives in Estonia and invests in euros — EUR/USD moves directly affect returns.

---

### Agent 5: SENTIMENT SCANNER
**Role:** Track what retail and institutional investors are saying about our stocks.
**Frequency:** Weekly
**Data Sources:**
- Reddit (r/WallStreetBets, r/stocks) via SwaggyStocks or AltIndex
- Analyst upgrades/downgrades (MarketBeat, Benzinga)
- Short interest changes (Finviz, ORTEX)
- Social media mention volume
**Output:** `research/weekly/sentiment_YYYY-MM-DD.md`
**Key Questions:**
- Is any of our stocks suddenly trending on Reddit? (Could mean incoming volatility)
- Any analyst upgrades/downgrades this week?
- Short interest increasing or decreasing? (DUOL at 13.9% — if it drops, shorts are covering = bullish)
- Is consensus shifting on any of our names?
**Why we missed this:** We checked consensus once. Consensus CHANGES. An analyst downgrade or Reddit pump can move these stocks 10-20% in a day.

---

### Agent 6: COMPETITOR WATCHDOG
**Role:** Monitor what competitors are doing to our portfolio companies.
**Frequency:** Bi-weekly
**Data Sources:**
- Industry news, earnings calls of competitors
- Patent filings
- Partnership announcements
- New market entrants
**Output:** `research/competitive/competitor_updates.md`
**Key Questions:**
- Is anyone challenging Vertiv's cooling dominance? (Schneider Electric, Eaton's Boyd acquisition)
- Is Schrödinger's software moat defensible? Any new computational chemistry platforms?
- Are big pharma companies building AI labs that make SDGR/RLAY obsolete?
- New robotics IPOs coming that change the BOTZ landscape?
- Duolingo: is ChatGPT actually stealing users or not? What do the app store rankings show?
**Why we missed this:** We analyzed our companies in a vacuum. Eaton just acquired Boyd for $9.5B — that directly competes with Vertiv on cooling. We barely noted it.

---

### Agent 7: SECOND-ORDER EFFECTS SCOUT
**Role:** Find non-obvious AI beneficiaries that nobody is talking about yet.
**Frequency:** Monthly
**Data Sources:**
- Morgan Stanley research on AI second-order effects
- Academic papers on AI economic impact
- Industry reports on AI adoption rates by sector
- Job market data (which industries are hiring/firing due to AI?)
**Output:** `research/second_order/monthly_scan_YYYY-MM.md`
**Key Questions:**
- Which industries are ADOPTING AI fastest? (The adopters beat the builders historically)
- Any "boring" companies quietly using AI to cut costs 30%+ that the market doesn't know about?
- Water infrastructure for data center cooling — real investable thesis or too niche?
- Entertainment/leisure boom from AI productivity gains — any data supporting this?
- Insurance companies using AI to cut claims processing — could be massive margin expansion
**Why we missed this:** The devil's advocate flagged this as potentially the BEST approach. Morgan Stanley's research says AI adopters outperform AI builders. Netflix > Cisco. We identified the principle but never actually researched specific second-order stocks.

---

### Agent 8: PORTFOLIO DOCTOR
**Role:** Weekly health check on the actual portfolio. This is the "so what" agent.
**Frequency:** Weekly (runs AFTER all other agents)
**Inputs:** Output from all 7 other agents
**Output:** `research/weekly/portfolio_review_YYYY-MM-DD.md`
**Key Questions:**
- Given what all agents found this week, should we change anything?
- Any position >20% of portfolio? Rebalance signal.
- Any thesis broken? (E.g., SDGR software revenue declines, VRT loses Nvidia partnership)
- Any new opportunity that's better than a current holding? Swap candidate?
- Net portfolio performance vs benchmarks (S&P 500, QQQ)
- Action items for this week: BUY / SELL / HOLD / RESEARCH MORE
**Why we need this:** Without a synthesis agent, the other 7 produce information but no ACTION. This agent is the decision-maker.

---

## Agent Execution Order

```
Every Week:
  Monday:    Agent 4 (Macro) → Agent 1 (Insiders) → Agent 5 (Sentiment)
  Wednesday: Agent 2 (Catalysts) → Agent 3 (Technicals)
  Friday:    Agent 8 (Portfolio Doctor) — synthesizes everything

Every 2 Weeks:
  Agent 6 (Competitor Watchdog)

Every Month:
  Agent 7 (Second-Order Effects Scout)
```

## What This Catches That We Missed

| Blind Spot | Which Agent Fixes It |
|---|---|
| EUR/USD currency risk | Agent 4 (Macro) |
| Company executive insider buying | Agent 1 (Insider Tracker) |
| Earnings surprise risk | Agent 2 (Catalyst Calendar) |
| Buying into a downtrend | Agent 3 (Technical Scanner) |
| Recession kills everything | Agent 4 (Macro) |
| Analyst downgrade we didn't see | Agent 5 (Sentiment) |
| Competitor eating our company's lunch | Agent 6 (Competitor) |
| Better opportunities we're not seeing | Agent 7 (Second-Order) |
| No action from all this research | Agent 8 (Portfolio Doctor) |

---

## Implementation Notes

### For Claude Code Sessions
Each agent can be launched as a parallel sub-agent using the Task tool. In a single session:
1. Launch Agents 1-5 in parallel (independent research)
2. Wait for results
3. Launch Agent 6 if bi-weekly
4. Launch Agent 8 last (needs all other outputs)

### For IBKR
- Set price alerts on IBKR for key levels identified by Agent 3
- Set earnings alerts for dates from Agent 2
- Use IBKR's news feed to supplement Agent 5

### Data Storage
All agent outputs go to `/research/weekly/` or `/research/monthly/`
Over time, this builds a searchable history of what changed and when.

---

*The goal: never be surprised by something we should have known.*
