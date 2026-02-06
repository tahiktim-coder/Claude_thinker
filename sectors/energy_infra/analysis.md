# Energy Infrastructure for AI Data Centers

**Updated:** February 2026
**Context:** Analysis for a retail investor deploying ~$1K via Interactive Brokers.

---

## The Thesis

AI requires enormous and growing amounts of electricity. U.S. data centers currently draw ~15 GW of power. By 2030, that number hits 100-134 GW (BloombergNEF, Goldman Sachs, S&P Global all converge on this range). Hyperscalers (Microsoft, Amazon, Google, Meta) are spending ~$400-430B in capex in 2025-2026, and the physical constraint on AI deployment is no longer algorithms -- it is power, cooling, and grid connections.

The investment logic: you do not need to pick the AI model winner. You buy the electricity, the uranium, the switchgear, and the cooling systems that every model needs.

---

## The Numbers (as of early 2026)

| Metric | Figure | Source |
|---|---|---|
| Current U.S. data center power draw | ~15 GW | Goldman Sachs |
| Projected U.S. data center power (2026) | ~76 GW (IT + cooling) | S&P Global |
| Projected U.S. data center power (2030) | ~134 GW | S&P Global |
| Data center share of U.S. electricity (2026) | ~6% (~260 TWh) | IEA / Pew |
| Data center share of U.S. electricity (2030) | ~9% | DOE |
| Hyperscaler capex 2025 | ~$414B | Analyst consensus |
| Single AI training cluster power (2028 est.) | Up to 1 GW | RAND |
| Global data center critical power (2026) | ~96 GW | Industry estimates |

These forecasts keep getting revised *upward*. BNEF's latest U.S. forecast (106 GW by 2035) was a 36% jump from their estimate just seven months prior. Of ~150 new data center projects tracked by BNEF in the past year, nearly 25% exceed 500 MW -- double last year's share.

**Grid impact is already real:** In the PJM electricity market (Illinois to North Carolina), data centers caused a $9.3B price increase in the 2025-26 capacity market. Average residential bills are rising $16-18/month in affected regions.

---

## Sub-Sectors

### 1. Nuclear Power (Baseload Clean Energy)

**Why it matters:** Nuclear provides 24/7 carbon-free baseload power. Tech companies need carbon-free energy for ESG commitments and regulatory compliance. Meta signed a 20-year, 1.1 GW deal with Constellation Energy. Amazon locked in 1,920 MW from Talen Energy through 2042. Trump administration aims to grow U.S. nuclear from 100 GW to 400 GW by 2050 via executive order.

**Key stocks:**

**Constellation Energy (CEG)** -- $287, ~32x forward P/E
- The dominant player: 21 reactors, largest U.S. carbon-free generator (31,676 MWh capacity, 69.7% nuclear).
- Stock has run 525% since 2022 IPO. 52-week range: $161-$413.
- Earnings growth: +8.3% in 2025, +18.8% in 2026. Capex: $3B (2025), $3.5B (2026).
- All 13 analysts rate Buy, average target ~$408 (+32% upside). Zacks Rank #2 (Buy).
- *Honest take:* Highest-quality name in the space. The premium valuation (~32x forward) is justified by long-dated PPAs with Big Tech, but you are paying up. At $287 it is well below the $413 peak -- that is the good news. The bad news is you are still paying a big multiple for a utility. For $1K, this works but you are buying quality at a fair-to-full price, not a bargain.

**Vistra Corp (VST)** -- $163, ~18x forward P/E
- Larger total generation capacity (40,657 MWh) but only 16% nuclear. Rest is gas + solar + battery.
- Guiding 2026 EBITDA to $6.8-7.6B, up from $5.7-5.9B in 2025. ROE of 72%.
- $1B buyback authorized through 2027. Zacks Rank #3 (Hold).
- *Honest take:* Cheapest quality name at ~18x forward. The diversified fuel mix is both a feature (more earnings levers, less single-source risk) and a bug (less pure-play appeal). For a $1K position, VST may offer more upside per dollar than CEG. The buyback provides a floor. This is the value play in the space.

**Cameco (CCJ)** -- Uranium miner, not a power generator
- Projected +100% EPS growth in FY25, +55% in FY26. Stock up 800% in 5 years.
- *Honest take:* You are betting on uranium prices staying elevated. Structural supply deficit supports this, but the stock has already moved enormously. Any uranium price dip hits CCJ hard. Best as a complement to a generator position, not standalone.

**Talen Energy (TLN)** -- Amazon's nuclear partner
- Providing Amazon 1,920 MW through 2042. Revenue growth expected 67.4%, earnings growth 100%+.
- *Honest take:* Less discussed than CEG, which means potentially less priced in. The Amazon anchor contract is powerful. Worth researching as a CEG alternative with more upside potential.

**NuScale Power (SMR)** -- ~$19, pre-revenue
- Only NRC-certified SMR design in the U.S. Market cap ~$4.6B on $37M revenue (2024).
- Expected to lose $0.62/share in 2026. No deployed reactors. Cancelled Utah project is a red flag.
- Revenue could 8x by 2027 ($293M target) but first plant not expected until ~2030.
- Zacks Rank #5 (Strong Sell). Price target $36.56 avg from 9 analysts (+81%).
- *Honest take:* This is a lottery ticket, not an investment. At $4.6B market cap with no deployed product and a Strong Sell rating, you are paying for a story. Could it 10x? Possibly. Could it go to zero? Also possible. Limit to 5-10% of your $1K if you must.

**Oklo (OKLO)** -- Even more speculative than NuScale
- Pre-revenue, no approved reactor design, stock down ~50% from peak. Could lose another 50% and still be expensive.
- *Honest take:* Avoid unless you are explicitly gambling.

### 2. Natural Gas (The Bridge Fuel)

Gas plants can be built in 2-3 years vs 10+ for nuclear. They are filling the gap while nuclear and renewables scale.

**GE Vernova (GEV)** -- Gas turbines + grid equipment
- EPS growth: +34% in FY25, +71% in FY26. $150B+ backlog.
- $2B+ in direct data center orders in 2025, tripling prior year.
- Pulled back ~20% from highs in early 2026.
- *Honest take:* Quality industrial compounder. The pullback creates a better entry than 3 months ago. Benefits from both gas-to-power and grid modernization. Not a moonshot -- a reliable grower.

### 3. Grid Infrastructure (Picks and Shovels)

The grid is the bottleneck. New data centers need high-voltage connections, transformers, and switchgear. There is a global transformer shortage creating pricing power.

**Eaton Corp (ETN)** -- The "grid-to-chip" leader
- Makes switchgear, transformers, busbar systems. Collaborated with Nvidia on 800V DC power architecture.
- Completing $1.2B capacity expansion. Acquired Boyd for $9.5B (liquid cooling scale).
- Analyst targets: $414-$495 for 2026. Ranked 47th out of 5,000+ stocks on financial health (overall grade: A).
- *Honest take:* The most boring name on this list -- and possibly the best risk-adjusted pick. Eaton benefits no matter which energy source wins. Every data center needs Eaton's products. Premium valuation but backed by real earnings and pricing power from the transformer shortage. If you want one stock for $1K, this is the safest choice.

**Quanta Services (PWR)** -- Grid modernization contractor
- Builds transmission lines, substations, grid connections. Raised 2025 outlook on data center-related contracts.
- *Honest take:* Captures spending that happens years before the first GPU gets racked. Less sexy, more reliable. Under-the-radar picks-and-shovels.

**EMCOR Group (EME)** -- Largest U.S. specialty contractor
- Handles critical electrical and mechanical systems for data centers: switchgear, backup generators, high-voltage distribution.
- *Honest take:* Another under-followed name. Real revenue, real contracts, less hype premium.

### 4. Cooling (The Physics Problem)

AI racks run at 20-100+ kW per rack vs 5-15 kW for traditional servers. Air cooling is physically impossible above ~40 kW. By early 2026, AI clusters push 120-150 kW per rack. Liquid cooling is now mandatory for frontier AI. Water holds heat 3,000x more effectively than air.

**Vertiv Holdings (VRT)** -- ~$163, the pure-play leader
- $9.5B backlog, 28% organic revenue growth. Co-developing cooling for Nvidia Blackwell/Rubin platforms ("Titan" partnership: 7MW reference architecture for GB200 NVL72).
- 2025E EPS: $4.08. 2026E EPS: ~$5.14 (+25% YoY). Analysts target ~$200-210.
- Barclays and Goldman reiterate Buy. Evercore target $210.
- *Honest take:* Best positioned cooling company. The Nvidia partnership is a genuine moat -- Vertiv's technology is embedded in the blueprints for the world's most advanced AI servers. At ~46x trailing / ~32x 2026E earnings, you pay a premium. Tariff risk on Chinese cooling components (145% tariffs) is real but manageable. If you believe AI buildout continues, Vertiv is a core holding.

**Modine Manufacturing (MOD)** -- Smaller, less known
- Climate Solutions segment grew 42% in data center revenue. $2B+ DC revenue target by FY28.
- *Honest take:* Interesting small-cap alternative to Vertiv with more room to run and less analyst coverage.

**Schneider Electric** -- Global competitor to Vertiv
- In a dead heat with Vertiv for global data center power infrastructure market share as of 2026. Broader industrial footprint but less AI-specialized.
- *Honest take:* Paris-listed, harder to access on IBKR for some. Good diversified industrial but less pure-play.

**nVent Electric (NVT)** -- ~30% data center exposure, growing Nvidia partnership. Solid but less pure-play than Vertiv.

---

## ETF Options for a $1K Portfolio

| ETF | Ticker | Focus | Expense Ratio | Key Holdings | Note |
|---|---|---|---|---|---|
| Global X Uranium | URA | Uranium miners + nuclear | 0.69% | CCJ (21%), OKLO (14%), SMR (5%) | Most liquid nuclear ETF. OKLO drag is a concern. |
| VanEck Uranium & Nuclear | NLR | Uranium + nuclear utilities | 0.56% | Broader, more conservative mix | Less speculative than URA |
| Range Nuclear Renaissance | NUKZ | Pure nuclear theme | Varies | Nuclear-focused basket | Newer, less established |
| Global X Data Center Infra | DTCR | Data center REITs + operators | 0.50% | Equinix, Digital Realty | Captures REIT/operator side, not energy side |
| iShares U.S. Digital Infra | IDGT | Digital infrastructure | Varies | Broad digital infra | Newer BlackRock offering |

**Honest take on ETFs:** URA is the most popular nuclear ETF but 14% in OKLO (pre-revenue) is dead weight. NLR is more conservative. DTCR captures REITs and operators, not the energy producers. There is no single ETF that perfectly captures the "power for AI" thesis across nuclear + grid + cooling. You may be better off with 1-2 individual stocks than a mediocre ETF.

---

## Consensus Check: Is This Trade Crowded?

**Yes, it is crowded.** Evidence:

1. Every major financial publication has run "nuclear stocks for AI" articles throughout 2025-26 (Motley Fool, Yahoo Finance, Nasdaq, Seeking Alpha, Benzinga -- all appeared in my searches).
2. CEG is up 525% since 2022. CCJ is up 800% in 5 years. VRT gained 190% in 2024 alone.
3. Pre-revenue companies (OKLO, SMR) reached multi-billion dollar valuations.
4. Nuclear ETFs (URA) saw massive inflows throughout 2025.
5. The early-2026 pullback (CEG and GEV both ~20% off highs) suggests froth is coming out.

**But "crowded" does not mean "wrong."** The underlying demand is real and accelerating. Forecasts keep being revised upward. The question is not *whether* AI needs power -- it does -- but whether current stock prices already discount 3-5 years of growth.

**The key nuance:** High-quality names (CEG, ETN, VRT) are crowded but fundamentally supported by real earnings and long-dated contracts. Speculative names (SMR, OKLO) are crowded AND fundamentally unsupported. Value/infrastructure plays (VST, Quanta, EMCOR, Modine) are less crowded and offer more edge.

---

## Contrarian Risk: The DeepSeek Efficiency Scenario

**The bear case:** DeepSeek demonstrated AI models can be trained with 10-40x less energy. Their servers reportedly consume 50-75% less energy than Nvidia's latest GPUs. A cluster of H800 chips uses ~75 MW vs ~150 MW for equivalent H100 chips. If efficiency gains continue, projected power demand could be dramatically lower.

**Why the bear case is probably wrong (but not certainly wrong):**

1. **Jevons Paradox** -- the strongest counter-argument. Every efficiency gain in computing history has led to *more* total energy consumption. Cheaper AI = more companies deploy it = more applications = more inference queries. Moody's VP: "What that does is it lowers the cost of computing and potentially increases the number of new companies and new applications that can be created."

2. **Training vs. inference** -- DeepSeek was cheap to *train* (~$5.5M). But inference (running the model for users) still consumes similar energy to competitors. Training is one-time; inference is ongoing and scales with users.

3. **Unverified claims** -- DeepSeek's 50-75% energy reduction figures come from their own papers. Third-party validation is pending.

4. **The math still works for bulls** -- Even if each query is 50% more efficient, a 10x increase in total queries still means 5x more power. The demand curve is exponential.

5. **Expert consensus holds** -- S&P Global, IEA, DOE, and BNEF all project rising data center power demand *after* accounting for efficiency improvements.

**But take the risk seriously.** If a true breakthrough makes AI 100x more efficient and demand does not scale proportionally, the power thesis weakens. This is a tail risk, not a base case.

**Monitor these signals:**
- Inference cost per query trends (declining = Jevons risk)
- Actual data center power consumption vs forecasts (tracking? lagging?)
- Hyperscaler capex guidance revisions (any slowdown = sector selloff)
- Total U.S. electricity generation growth rate

---

## Honest Verdict for $1K on Interactive Brokers

### The good news
- The underlying demand is real, accelerating, and being revised upward by every major forecaster.
- You do not need to pick the AI model winner -- every model needs power and cooling.
- The early-2026 pullback (CEG, GEV, VRT all 15-20% off highs) creates better entries.
- Government policy (Trump nuclear executive orders) is a tailwind.
- Long-dated PPAs (Meta-CEG 20yr, Amazon-TLN 18yr) provide revenue visibility rare in energy.

### The bad news
- This is one of the most crowded thematic trades on Wall Street right now.
- The best companies (CEG, VRT, ETN) trade at premium multiples.
- The cheap-looking companies (SMR, OKLO) are cheap for a reason (no revenue, no product).
- A $1K position limits your ability to diversify across sub-sectors.
- If hyperscaler capex guidance slows even slightly, the entire sector sells off hard.

### What to actually do with $1K

**Option A -- Single stock, highest conviction:**
Pick ONE based on risk tolerance:
- **Lower risk:** Eaton (ETN) -- benefits regardless of energy source, real earnings, transformer shortage = pricing power, top-tier financial health rating.
- **Moderate risk / best value:** Vistra (VST) -- cheapest quality name at ~18x forward, big EBITDA ramp, $1B buyback support.
- **Higher risk / pure-play:** Vertiv (VRT) -- pure cooling play, Nvidia partnership moat, but premium valuation.

**Option B -- Split approach:**
- $500 in VST or ETN (established, profitable, reasonable valuation)
- $500 in URA or NLR ETF (diversified nuclear/uranium exposure)

**Option C -- ETF only (simplest):**
- $1K in NLR (if you want conservative nuclear exposure)
- or $500 URA / $500 DTCR (nuclear + data center REITs)

### What to avoid
- **NuScale (SMR) and Oklo (OKLO)** at current valuations. Pre-revenue + multi-billion market caps + Strong Sell rating. The risk/reward is poor for a $1K portfolio.
- **Going all-in on CEG at 32x forward.** It is the best company but the price reflects that. You need it to keep compounding at premium multiples to make money.
- **Allocating more than 10-15% of total portfolio** to this single theme, no matter how compelling.

### Key catalysts to watch
1. Hyperscaler earnings calls -- any capex guidance change moves the entire sector
2. Actual data center power consumption vs projections (Q2-Q3 2026 data)
3. Uranium spot prices and long-term contracting activity
4. NRC regulatory decisions on new reactor designs
5. PJM and other grid operator capacity auction results
6. Nvidia Rubin platform launch and associated infrastructure requirements
7. DeepSeek follow-on efficiency claims and third-party validation

**Conviction: 8/10** -- strongest infrastructure thesis available, but stock selection and entry price matter enormously given how crowded the trade has become.

---

## Sources

- [Goldman Sachs: AI to drive 165% increase in data center power demand by 2030](https://www.goldmansachs.com/insights/articles/ai-to-drive-165-increase-in-data-center-power-demand-by-2030)
- [S&P Global: Data center grid-power demand to rise 22% in 2025, nearly triple by 2030](https://www.spglobal.com/energy/en/news-research/latest-news/electric-power/101425-data-center-grid-power-demand-to-rise-22-in-2025-nearly-triple-by-2030)
- [Pew Research: What we know about energy use at U.S. data centers](https://www.pewresearch.org/short-reads/2025/10/24/what-we-know-about-energy-use-at-us-data-centers-amid-the-ai-boom/)
- [BloombergNEF: AI and the Power Grid](https://about.bnef.com/insights/clean-energy/ai-and-the-power-grid-where-the-rubber-meets-the-road/)
- [RAND: AI Data Center Power Demand](https://www.rand.org/pubs/research_reports/RRA3572-1.html)
- [IEA: Energy demand from AI](https://www.iea.org/reports/energy-and-ai/energy-demand-from-ai)
- [Axios: Power, energy demand for AI data centers is surging](https://www.axios.com/2025/12/01/data-centers-ai-power-energy-demand-future)
- [S&P Global: Potential impacts of DeepSeek on datacenters and energy demand](https://www.spglobal.com/market-intelligence/en/news-insights/research/potential-impacts-of-deepseek-on-datacenters-and-energy-demand)
- [Heatmap News: What DeepSeek Means for AI Energy Demand](https://heatmap.news/energy/deepseek-ai-energy-demand)
- [Nasdaq: Constellation Energy vs. Vistra](https://www.nasdaq.com/articles/constellation-energy-vs-vistra-which-utility-stock-stronger-bet)
- [Motley Fool: Nuclear Energy ETFs for 2026](https://www.fool.com/investing/stock-market/market-sectors/energy/nuclear/nuclear-etfs/)
- [Motley Fool: Should You Buy Nuclear Energy Stocks in 2026?](https://www.fool.com/investing/2025/12/17/should-you-buy-nuclear-energy-stocks-in-2026/)
- [Sprott: Uranium Outlook 2026](https://sprottetfs.com/insights/uranium-outlook-2026/)
- [Benzinga: Top AI Infrastructure Stocks For 2026](https://www.benzinga.com/trading-ideas/long-ideas/25/12/49572927/top-ai-infrastructure-stocks-for-2026-industrial-super-cycle)
- [Seeking Alpha: NuScale Power -- Powerful But Risky Potential](https://seekingalpha.com/article/4856769-nuscale-power-powerful-but-risky-potential)
- [Global X: Data Center & Digital Infrastructure ETF (DTCR)](https://www.globalxetfs.com/funds/dtcr/)
- [Global X: Uranium ETF (URA)](https://www.globalxetfs.com/funds/ura)
- [Bismarck Analysis: AI 2026 -- Data Centers Restart Growth](https://brief.bismarckanalysis.com/p/ai-2026-data-centers-restart-growth)

---

*Disclaimer: This is research and analysis, not financial advice. All prices and valuations as of early February 2026. Do your own due diligence.*
