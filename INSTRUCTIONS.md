# HOW TO USE CLAUDE THINKER
### Quick Guide (Phone-Friendly)

---

## WHAT IS THIS?

An AI-powered investment research system tracking your portfolio of AI-disruption stocks. It lives in a GitHub repo. Every session, you share your portfolio screenshot and I analyze it, compare to previous reviews, and give you specific actions.

---

## WHAT TO DO EACH SESSION

### 1. Screenshot your Lightyear portfolio
- Open the app
- Go to Investments tab
- Set filter to "All time"
- Screenshot it

### 2. Send the screenshot to me
- I'll read every position, value, and % change
- Compare to the last review automatically

### 3. Tell me what you need
Some examples:
- **"Review"** — Full portfolio analysis vs last time
- **"What should I buy?"** — Recommendations based on cash + allocation
- **"Research [TICKER]"** — Deep dive on a new stock
- **"Update"** — Quick check, no deep analysis
- **"Macro check"** — What's happening in the market that affects us

### 4. I'll give you
- Updated position table with grades
- What changed since last review
- Specific BUY / SELL / HOLD actions with dollar amounts
- A letter grade (A-F) for the portfolio
- Updated MASTER_TABLE.md committed to the repo

---

## WHAT I TRACK

### Your Portfolio (as of April 6, 2026)
| Ticker | What It Is | Status |
|--------|-----------|--------|
| INOD | AI data services | Hold (too concentrated) |
| CEVA | Edge AI semiconductor IP | Best pick, hold + add |
| RXRX | AI drug discovery | Trim (consensus, no edge) |
| RLAY | AI drug discovery | Star (+25%), hold |
| AMSC | Grid infrastructure | Winner (+18%), hold |
| SDGR | Computational chemistry | Hold for Q2 catalyst |
| VST | Power generation | Hold + add (underweight) |
| SOUN | Voice AI | SELL (4th warning) |

### Key Files in the Repo
| File | What It Is |
|------|-----------|
| `MASTER_TABLE.md` | Single source of truth — all positions, watchlist, signals |
| `METHODOLOGY.md` | Full playbook — scoring, rules, process |
| `INSTRUCTIONS.md` | This file |
| `research/weekly/` | Every weekly review, dated |
| `devils_advocate/` | The bear case for everything |
| `framework/` | How we score stocks |

---

## THE RULES I FOLLOW

### How I Pick Stocks
1. **Consensus test** — If every AI recommends it, be cautious
2. **Insider check** — CEOs buying own stock = strongest buy signal
3. **Politician check** — Pelosi, congress trades via Capitol Trades
4. **Devil's advocate** — Write the bear case before buying
5. **Sector fit** — Must fit AI disruption thesis

### When I Say SELL
- Insiders mass-selling (like SOUN March 20)
- Thesis broken (like DUOL)
- Consensus pick not performing (like RXRX)
- Position too large (>25%)

### When I Say BUY/ADD
- Insiders buying (like CEVA)
- Politician signal (like VST via Pelosi)
- Thesis confirmed by data (like RLAY post-ESMO)
- Sector underweight (like energy right now)

### Target Allocation
| Sector | Target | Current |
|--------|--------|---------|
| Energy / Grid | 25-30% | 17.5% (need more) |
| Edge AI / Semicon | 20-25% | 27.5% |
| Biotech / AI Drug | 20-25% | 31.5% (trim RXRX) |
| AI Data Services | 15-20% | 33.4% (way over) |
| Speculative | 0-5% | 5.6% (sell SOUN) |

---

## SIGNAL SOURCES I CHECK

### Best (Smart Money)
- **Capitol Trades** — politician stock trades
- **SEC Form 4** — company insider buys/sells
- **Unusual Whales** — options flow + congress
- **13F filings** — hedge fund quarterly positions

### Good (Analyst)
- **MarketBeat** — upgrades/downgrades
- **StockAnalysis** — consensus estimates
- **Yahoo Finance** — earnings, news

### Use with Caution
- Reddit, TikTok, Discord — idea generation ONLY, never a buy signal

---

## UPCOMING DATES TO WATCH

| When | What | Stock |
|------|------|-------|
| Q2 2026 | SGR-3515 Phase 1 data | SDGR (binary catalyst) |
| H1 2026 | Zovegalisib triplet data | RLAY |
| May 7 | SoundHound earnings | SOUN (sell before) |
| May 13 | CEVA earnings | CEVA |
| May 2026 | Fed Powell term expires | All stocks |
| Q4 2026 | OpenAI IPO expected | AI sentiment |

---

## YOUR WEEKLY CHECKLIST

- [ ] Check Capitol Trades for new politician filings
- [ ] Check Unusual Whales for unusual options activity
- [ ] Screenshot portfolio and run a review session
- [ ] Check if any earnings/catalysts are this week
- [ ] Execute any SELL recommendations (don't delay!)

---

## WHAT I NEED FROM YOU

1. **Portfolio screenshots** — So I can track real numbers
2. **Tell me when you buy/sell** — So I can update the records
3. **Tell me when you add capital** — So I can distinguish gains from deposits
4. **Act on SELL signals** — The longer you wait, the more it costs (SOUN lesson)
5. **Ask questions** — "Should I buy X?", "What about sector Y?", "Is Z still good?"

---

## HOW THE REPO WORKS

Everything is stored in a Git repository. Each session:
1. I read previous files to know where we left off
2. I create/update analysis files
3. I commit and push so nothing is lost
4. You can browse the repo anytime to read old reviews

The history is your research journal. Every decision, every recommendation, every mistake — all documented with dates.

---

## QUICK COMMANDS

Just tell me what you need in plain language:

| You Say | I Do |
|---------|------|
| "Review" or send screenshot | Full portfolio analysis |
| "Quick update" | Compare to last review, flag issues |
| "Research TICKER" | Deep dive on a specific stock |
| "What should I buy with €X?" | Allocation recommendation |
| "Macro check" | Market conditions affecting portfolio |
| "New opportunities" | Scan for stocks we're not tracking |
| "Update master table" | Refresh MASTER_TABLE.md |
| "Grade me" | Honest portfolio grade with reasoning |

---

*Last updated: April 6, 2026*
*Total portfolio: €1,284.68 | Grade: B-*
