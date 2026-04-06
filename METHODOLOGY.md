# METHODOLOGY — How This Research System Works

*The complete playbook for Claude Thinker: what we do, how we do it, why we do it that way, and what every output should contain.*

---

## 1. MISSION

Find AI-disruption investment opportunities **before the market prices them in**, for a small retail portfolio (~€1,000-5,000) deployed from Estonia via Lightyear/IBKR.

**Time horizon:** 1-3 years
**Edge we're hunting:** Non-consensus ideas that require domain knowledge to see.

---

## 2. CORE PHILOSOPHY

### The Three Laws

1. **If every AI gives you the same stock pick, it's not an edge — it's consensus.**
   - Before buying any name, ask 3+ AI models. If they all say it, be cautious.
   - The best opportunities are ones that require nuance to find.

2. **Follow the insiders, not the analysts.**
   - When a CEO buys their own stock with personal money, that's conviction.
   - When a politician buys before legislation, that's signal.
   - When every C-suite exec sells on the same day, that's the exit.

3. **The devil's advocate is mandatory, not optional.**
   - Every thesis gets attacked before money goes in.
   - Read `/devils_advocate/contrarian_analysis.md` before every trade.
   - If the bear case doesn't make you uncomfortable, it's not honest enough.

### Investment Style

| Attribute | Our Approach |
|-----------|-------------|
| **Size** | Small-cap to mid-cap bias (under-covered = potential edge) |
| **Sectors** | AI infrastructure chain: biotech, energy/grid, semiconductors |
| **Geography** | US-listed stocks, bought in EUR from Estonia |
| **Holding period** | Months to years. Not day-trading. |
| **Position sizing** | No single stock >20-25% of portfolio (target, not always reality) |
| **Risk tolerance** | High for individual picks, managed through diversification |
| **Benchmark** | S&P 500 (VOO). We need to beat this or we're wasting time. |

---

## 3. RESEARCH PROCESS

### 3A. The 8-Agent System

We use 8 specialized research agents, each with a specific role. They run on a schedule and write to specific files. Full design: `/research/agent_system_design.md`

| Agent | Role | Frequency | Output |
|-------|------|-----------|--------|
| **1. Insider Tracker** | Politicians, hedge funds, executive trades | Weekly | Insider signals |
| **2. Catalyst Calendar** | Earnings, FDA dates, conferences, catalysts | Weekly | Event timeline |
| **3. Technical Scanner** | Price action, RSI, support/resistance, volume | Weekly | Entry/exit signals |
| **4. Macro Monitor** | Fed, rates, EUR/USD, recession risk, CapEx | Weekly | Market context |
| **5. Sentiment Scanner** | Reddit, analyst upgrades/downgrades, short interest | Weekly | Crowd positioning |
| **6. Competitor Watchdog** | What competitors are doing to our portfolio companies | Bi-weekly | Threat assessment |
| **7. Second-Order Scout** | Non-obvious AI beneficiaries nobody talks about | Monthly | New opportunities |
| **8. Portfolio Doctor** | Synthesize all agents into actionable decisions | Weekly (last) | BUY/SELL/HOLD |

**Execution order:**
```
Monday:    Macro → Insiders → Sentiment
Wednesday: Catalysts → Technicals
Friday:    Portfolio Doctor (synthesizes everything)
Bi-weekly: Competitor Watchdog
Monthly:   Second-Order Scout
```

### 3B. Signal Sources (Ranked by Reliability)

**Tier 1 — Smart Money (Most Reliable)**
- Capitol Trades — politician trades (45-day delay)
- Quiver Quantitative — congress + hedge funds + lobbying
- Unusual Whales — options flow + congressional trades
- SEC Form 4 — company insider buys/sells (strongest signal)
- 13F filings — quarterly hedge fund positions

**Tier 2 — Analyst & Institutional**
- MarketBeat — analyst upgrades/downgrades, price targets
- Seeking Alpha — deep-dive analysis (filter for quality)
- StockAnalysis — consensus estimates, financials
- Company IR pages — earnings calls, presentations

**Tier 3 — Crowd Sentiment (Fast but Noisy)**
- Reddit (r/WallStreetBets, r/stocks) — hype detection
- Finviz — screener, heat maps, short interest
- AltIndex — AI-scored stock sentiment

**Tier 4 — Avoid or Use with Extreme Caution**
- TikTok/FinTok — entertainment, not analysis
- Discord trading servers — potential pump-and-dump
- Random "top 10 AI stocks" articles — pure consensus

### 3C. How We Evaluate a New Stock

Every stock goes through this scoring framework (full version: `/framework/scoring_criteria.md`):

**Step 1: The Consensus Test**
- Ask 3+ AI models for their "best AI stock pick"
- If the stock appears on every list → be cautious (RXRX failed this)
- If nobody mentions it → dig deeper (CEVA passed this)

**Step 2: Sector Scoring (1-5 each)**

| Criteria | What We're Asking | Weight |
|----------|-------------------|--------|
| AI Leverage | How much does AI multiply this company's output? | High |
| Current Adoption | Low adoption = more room to run | High |
| Market Pricing | Has the AI narrative been priced in already? | High |
| Investability | Can we buy it on Lightyear/IBKR? | Medium |
| Time Horizon | Will impact show in 1-3 years? | Medium |
| Bottleneck Type | Compute constraint (good) or regulatory (bad)? | Medium |

**Step 3: Company Scoring**

| Criteria | What We're Asking |
|----------|-------------------|
| AI-Native | Built around AI, or bolting it on? |
| Moat | Data moat? Regulatory moat? Network effects? |
| Valuation | AI premium already, or still at legacy multiples? |
| Insider Activity | Are insiders buying or selling? |
| Catalysts | Upcoming events that could move the stock? |
| Risk | Binary outcomes? Cash burn? Dilution? |

**Step 4: Devil's Advocate**
- Write the bear case. Make it uncomfortable.
- If you can't find a strong bear case, you haven't researched enough.
- Check: would you still hold this if AI spending dropped 50%?

**Step 5: Position Sizing**
- Conviction level determines allocation (not equal-weight)
- Max 20-25% for highest conviction
- 5-10% for speculative/lottery tickets
- No position below $50 (not worth tracking)

---

## 4. OUTPUT FORMAT — What Every Report Must Contain

### 4A. Weekly Portfolio Review (the core output)

Every portfolio review follows this exact structure:

```markdown
# PORTFOLIO REVIEW — [Date]
## [One-liner editorial headline]

*Account stats: total value, cash, invested*
*Previous review date and value*
*Capital added since last review*

---

## WHAT CHANGED SINCE [LAST REVIEW DATE]
[Numbered list of actions taken and market moves]

## CURRENT HOLDINGS TABLE
| # | Ticker | Company | Value | Change | % of Portfolio | Action |

## PORTFOLIO SCORECARD (vs previous)
| Metric | Previous | Current | Change |

## WHAT'S WORKING / WHAT'S STRUGGLING
[Honest assessment of each position with specific data points]

## CONCENTRATION ANALYSIS
[Position sizes ranked, risk flags for anything >20%]

## SECTOR ALLOCATION TABLE
| Sector | Stocks | Value | % | Target % | Status |

## RECOMMENDED ACTIONS
[Numbered, specific: SELL X, TRIM Y, ADD Z with dollar amounts and reasoning]

## MACRO CONTEXT
[Only if significant changes from last review]

## INSIDER & POLITICIAN SIGNALS
[Any new trades or filings]

## UPCOMING CATALYSTS
| Date | Event | Stock | Action |

## GRADE
[Letter grade A-F with specific reasoning]

---
*Sources and disclaimer*
```

### 4B. Deep Research Reports

For new stock analysis or sector deep-dives:

```markdown
# [TICKER] DEEP DIVE — [Date]

## THE THESIS (2-3 sentences max)
## KEY NUMBERS
| Revenue | Growth | Margins | Valuation | Analyst PT |

## BULL CASE (why this works)
## BEAR CASE (why this fails)
## CONSENSUS CHECK (is this already priced in?)
## INSIDER ACTIVITY
## CATALYST TIMELINE
## VERDICT: BUY / WAIT / SKIP
## POSITION SIZE RECOMMENDATION
```

### 4C. Master Table (running document)

`MASTER_TABLE.md` is the single source of truth. Updated after every portfolio review:

- Current portfolio with all positions
- Watchlist with entry criteria
- Removed/skipped stocks with reasons
- Allocation targets vs actual
- Catalyst calendar
- Insider/politician signal tracker
- Macro dashboard

---

## 5. STRATEGY RULES

### Entry Rules
1. **Never buy on the same day you discover a stock.** Research first, sleep on it.
2. **Check insider activity before buying.** If insiders are selling, don't buy.
3. **Confirm the position is not consensus.** Run the 3-AI test.
4. **Define the thesis in one sentence.** If you can't, you don't understand it.
5. **Set a "thesis broken" trigger.** Know in advance what would make you sell.

### Exit Rules
1. **Sell when the thesis breaks.** Not when the price drops (that might be opportunity).
2. **Sell when insiders mass-sell.** CEO + CFO + COO selling same day = exit (SOUN).
3. **Sell consensus picks that aren't performing.** No edge + red = dead weight (RXRX).
4. **Trim when a position exceeds 25%.** Concentration kills portfolios.
5. **Never sell before a known catalyst** unless the thesis is broken (SDGR before SGR-3515 data).

### Allocation Rules
1. **No single stock >20-25% of portfolio** (aspirational — enforce this)
2. **Energy/grid: 25-30%** — highest conviction macro thesis
3. **Biotech/AI drug: 20-25%** — high risk, high reward, needs catalysts
4. **Edge AI/semicon: 20-25%** — CEVA is the core holding
5. **AI data/services: 15-20%** — INOD is the play
6. **Speculative/new: 5-10%** — lottery tickets only
7. **Cash reserve: 10-15%** — dry powder for catalysts and dips

### Risk Management
1. **Sector concentration cap:** No sector >35% of portfolio
2. **Biotech rule:** Never have >3 biotech names (binary risk compounds)
3. **EUR/USD awareness:** Dollar strength helps, euro strength hurts US positions
4. **Macro kill switch:** If recession odds >60% and Fed is raising rates, shift to defensive (energy, ETFs)
5. **Drawdown limit:** If total portfolio drops >30% from peak, reassess everything

---

## 6. WHAT WE'VE LEARNED (Lessons from Feb-April 2026)

| Lesson | Example | Action |
|--------|---------|--------|
| **Insider buying is the strongest signal** | CEVA insiders bought → stock recovering | Always check Form 4 before buying |
| **Insider selling is the strongest exit signal** | SOUN C-suite mass sold → stock collapsed further | Sell within 48 hours of mass insider sales |
| **Consensus picks underperform** | RXRX recommended by every AI → worst performer | Run the 3-AI test on every pick |
| **Follow the politicians** | Pelosi bought VST → outperformed | Check Capitol Trades weekly |
| **Energy/infrastructure is the safest AI bet** | AMSC only consistent green position | Maintain 25-30% energy allocation |
| **Clinical data confirmation matters** | RLAY post-ESMO → +25% | Buy biotech before catalysts, hold through data |
| **Don't fight the SELL signal** | We said sell SOUN 4 times, still holding = lost money | Execute sells within one session of recommendation |
| **Concentration is the silent killer** | INOD at 33% — one bad day = portfolio-level damage | Enforce the 20-25% cap |

---

## 7. FILE STRUCTURE

```
Claude_thinker/
├── METHODOLOGY.md              ← You are here. The playbook.
├── MASTER_TABLE.md             ← Single source of truth for all positions
├── FINAL_CALL.md               ← Original thesis document
├── README.md                   ← Project overview
├── summary.md                  ← Running conclusions
│
├── framework/
│   └── scoring_criteria.md     ← How we score sectors & companies
│
├── devils_advocate/
│   └── contrarian_analysis.md  ← The bear case for everything
│
├── research/
│   ├── agent_system_design.md  ← The 8-agent pipeline design
│   ├── signal_sources.md       ← Where we get data
│   ├── insider_tracking.md     ← Running insider activity log
│   │
│   └── weekly/
│       ├── portfolio_review_YYYY-MM-DD.md  ← Core weekly output
│       ├── full_update_YYYY-MM-DD.md       ← Deep weekly reports
│       └── [topic]_YYYY-MM-DD.md           ← Topical deep dives
│
├── sectors/
│   ├── biotech/analysis.md     ← Sector thesis + picks
│   ├── energy_infra/analysis.md
│   └── robotics/analysis.md
```

---

## 8. SESSION WORKFLOW

When starting a new research session, follow this order:

### Quick Review (5 min)
1. User provides portfolio screenshot or update
2. Compare to last review in `research/weekly/`
3. Flag any immediate actions (sell signals, broken theses)

### Full Analysis (when doing weekly review)
1. **Read last review** — what did we recommend?
2. **Compare positions** — what changed? Did user follow recommendations?
3. **Check macro** — any major shifts (rates, war, CapEx guidance)?
4. **Check insiders** — any new Form 4 filings or politician trades?
5. **Check catalysts** — anything coming up this week/month?
6. **Write review** — follow the template in Section 4A exactly
7. **Update MASTER_TABLE.md** — keep the single source of truth current
8. **Grade the portfolio** — honest letter grade with specific reasoning

### Deep Research (when exploring new opportunities)
1. **Source the idea** — where did this come from? (insider signal, screen, user request)
2. **Run consensus test** — is every AI model recommending this?
3. **Score using framework** — sector + company scoring from Section 3C
4. **Write devil's advocate** — the honest bear case
5. **Set position size** — based on conviction level
6. **Define thesis + exit trigger** — one sentence each

---

## 9. COMMUNICATION STYLE

### Tone
- Direct. No hedging with "might" and "could" when we have conviction.
- Honest. If a pick is failing, say so. Don't sugarcoat.
- Opinionated. Grade positions. Rank them. Say SELL when it's time.
- Self-aware. Acknowledge when we were wrong (we missed VRT, we were late on SOUN sell).

### What we always include
- Specific numbers (not "the stock went up" — "$367.96, +25.11%")
- Comparisons to previous review (was X, now Y)
- Action items with dollar amounts ("sell ~$61 of SOUN, add ~$65 to VST")
- A grade — letter grade with reasoning

### What we never do
- Say "this is not financial advice" as an excuse to be vague. Be specific, add the disclaimer at the bottom.
- Recommend a stock without the bear case.
- Ignore a sell signal because the user didn't act on it. Say it again. And again.
- Add positions to the portfolio without checking concentration first.

---

## 10. PERFORMANCE TRACKING

Every month, calculate:

| Metric | How to Calculate |
|--------|-----------------|
| **Total return** | (Current value - Total capital deployed) / Total capital deployed |
| **vs S&P 500** | Compare our return to VOO over same period |
| **Win rate** | Green positions / Total positions |
| **Best pick** | Highest % gainer |
| **Worst pick** | Highest % loser |
| **Thesis accuracy** | How many of our BUY/SELL calls were correct? |
| **Recommendation follow-through** | Did the user act on our recommendations? |

---

*This document is the operating manual. When in doubt about process, check here first. When starting a new session, skim Sections 3-4 and 8. When the user asks "what do you do" — point them here.*

*Last updated: April 6, 2026*
