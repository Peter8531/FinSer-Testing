# Client Review Prep

description: Produce an adviser working paper (paraplanning brief) for client review meetings with portfolio performance summary, allocation analysis, talking points, and action items. Pulls together account data into a concise meeting-ready format. Use before annual reviews, ongoing fee arrangement renewals, or ad-hoc client meetings. Output goes to paraplanning for formal SOA/ROA drafting. Triggers on "client review", "meeting prep for [client]", "annual review", "prep for [client name]", or "client meeting".

## Workflow

### Step 1: Client Context

Gather or look up:
- **Client name** and household members
- **Account types**: Personal (individual/joint), super (accumulation), super (pension phase), SMSF, family trust, company
- **Total assets** across all accounts (including super, property, cash)
- **Investment Policy / SOA**: Target allocation, risk profile, constraints
- **Life stage**: Accumulation, pre-retirement, transition to retirement, retirement (pension phase), aged care
- **Last review date** and any outstanding action items
- **Ongoing Fee Arrangement (OFA)**: Renewal date — must renew annually with client opt-in

### Step 2: Portfolio Performance

For each account and the household aggregate:

| Metric | QTD | YTD (FY) | 1-Year | 3-Year | Since Inception |
|--------|-----|----------|--------|--------|----------------|
| Portfolio return | | | | | |
| Benchmark return | | | | | |
| Alpha | | | | | |

**Benchmarks**: S&P/ASX 200 (Australian equities), MSCI World ex-AU (international), Bloomberg AusBond Composite (fixed income), or blended benchmark matching the client's target allocation.

**Performance Attribution:**
- Which asset classes / positions drove returns?
- Top 3 contributors and top 3 detractors
- Any outsized single-position impact?
- Franking credits received and their after-tax value

### Step 3: Allocation Review

Current vs. target allocation:

| Asset Class | Target | Current | Drift | Action |
|------------|--------|---------|-------|--------|
| Australian Equities | | | | |
| Australian Small/Mid Cap | | | | |
| International Developed | | | | |
| Emerging Markets | | | | |
| Australian Fixed Income | | | | |
| International Fixed Income | | | | |
| Property (A-REITs / direct) | | | | |
| Alternatives | | | | |
| Cash / Term Deposits | | | | |

Flag any drift exceeding the rebalancing threshold (typically 3-5%).

### Step 4: Talking Points

Generate a meeting agenda:

1. **Market overview** (2-3 min): Brief macro context — RBA interest rate outlook, ASX performance, global markets, AUD movements
2. **Portfolio performance** (5 min): How did we do? Why? Franking credits received
3. **Allocation review** (5 min): Any rebalancing needed?
4. **Superannuation review** (5-10 min):
   - Contribution strategy — are we maximising concessional cap? Carry-forward available?
   - Insurance inside super — adequate? Eroding balance?
   - Pension drawdown on track (if in pension phase)?
   - BDBN current? (Check lapsing nomination expiry)
5. **Planning updates** (5-10 min):
   - Life changes? (job, health, family, property, business)
   - Income needs changing?
   - Tax position — FY tax planning opportunities before 30 June
   - Centrelink / Age Pension review (if approaching or past 67)
   - Estate planning — will, BDBN, power of attorney current?
6. **Action items** (5 min): What are we doing before next review?

### Step 5: Proactive Recommendations

Based on the review, suggest:
- Rebalancing trades (if drift exceeds thresholds)
- Super contribution strategy changes (salary sacrifice, non-concessional, spouse contributions, carry-forward)
- Capital loss harvesting opportunities (particularly approaching 30 June)
- Franking credit optimisation (portfolio tilts, timing of sales relative to ex-dividend dates)
- Transition to Retirement strategy review (if nearing preservation age)
- Centrelink optimisation (if approaching or in retirement — means testing, deeming rates)
- Insurance review: life, TPD, income protection — inside vs outside super, adequacy, own occupation TPD
- BDBN renewal (if lapsing nomination approaching 3-year expiry)
- Estate planning updates (will, testamentary trust, power of attorney)
- Aged care planning (if relevant — RAD, DAP, means-tested fees)
- Ongoing Fee Arrangement renewal (if due)

### Step 6: Output — SOA Summary Request Input

This skill produces the **analytical working papers** that feed into the SOA Summary Request (assembled by the `strategy-request` skill). See [CONVENTIONS.md](../../CONVENTIONS.md) for house style rules.

**Feeds into Summary of Advice:**
- Recommended action items with responsible party and dates (rebalancing trades, contribution strategy changes, insurance review items)
- Each item as a short, directive sentence

**Feeds into Projection Parameters:**
- Performance table with benchmarks (YTD aligned to financial year July-June)
- Allocation chart (current vs. target) with drift analysis
- Source-of-Truth table for each input (document name, date, section)

**Feeds into Alternatives:**
- Strategies considered and dismissed with rationale (e.g., alternative rebalancing approaches, different contribution strategies)

**Feeds into Notes to AA or Paraplanning:**
- Gap items to request from client
- Risk profile, life stage, last review date, outstanding action items
- OFA renewal date, BDBN expiry, next review date
- Flag any areas requiring further research or compliance review

**Calculation Workings (appendix):**
- Performance attribution (top contributors/detractors, franking credits)
- Allocation drift analysis with current vs. target percentages
- Rationale linking each recommendation to client goals, risk profile, and current circumstances
- ROA vs SOA determination (ROA if client circumstances have not significantly changed, otherwise full SOA required)
- Meeting agenda and talking points

## Important Notes

- **This output is an adviser working paper. It is not a client-facing document.** The `strategy-request` skill assembles the final SOA Summary Request for paraplanning.
- All tables must follow house style: no bullets in cells, no em dashes, short directive sentences.
- Know your client before the meeting. Review notes from last meeting and any life changes.
- Lead with what the client cares about, not what you want to talk about.
- If performance was poor, address it directly. Do not hide or spin.
- Always end with clear action items and next steps with dates.
- Document the meeting notes and any changes to the investment strategy.
- If advice is provided, document via SOA or ROA as required under the Corporations Act.
- Compliance: ensure all materials comply with AFSL obligations and ASIC regulatory guidance.
- Best Interest Duty (s961B): every recommendation must demonstrably be in the client's best interests.
- Ongoing Fee Arrangement must be renewed annually with client consent. Flag if renewal is due.
