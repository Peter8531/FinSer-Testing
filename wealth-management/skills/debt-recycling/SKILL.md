# Debt Recycling

description: Produce an adviser working paper (paraplanning brief) for a debt recycling strategy. Models conversion of non-deductible home loan debt into tax-deductible investment debt with full calculation workings — loan structuring, investment selection, tax deduction calculations, franking credit integration, cost of carry analysis, risk assessment, stress testing, and year-by-year projections. Output goes to paraplanning for formal SOA/ROA drafting. Triggers on "debt recycling", "convert mortgage to deductible", "deductible debt", "recycle mortgage", or "non-deductible to deductible".

## Workflow

### Step 1: Suitability Assessment

Debt recycling is a leveraged strategy — not suitable for everyone. Assess:

| Factor | Requirement | Client Detail |
|--------|------------|---------------|
| Stable income | Reliable employment or business income to service debt | |
| Marginal tax rate | Higher rate = greater deduction value (30%+ is ideal) | |
| Time horizon | 7+ years minimum — need time for compounding and to ride out market cycles | |
| Home loan | Existing mortgage with capacity for extra repayments or offset/redraw | |
| Risk tolerance | Comfortable with leveraged investing — must accept that investments can fall while debt remains | |
| Emergency fund | 3-6 months expenses in cash BEFORE starting | |
| Insurance | Adequate life, TPD, and income protection — leveraged investors need stronger cover | |

**Do NOT proceed if:**
- Client is uncomfortable with investment risk or leveraged strategies
- Income is unstable or at risk
- No emergency fund
- Time horizon <5 years
- Already over-leveraged (total debt serviceability is tight)

### Step 2: Loan Structure

The home loan must be structured correctly **before** any recycling begins:

**Required structure:**
```
Home Loan Facility
├── Split A: Non-deductible (home loan) — variable or fixed
│   └── This is the split that receives extra repayments
│   └── Redraw facility enabled (or offset account linked)
│
├── Split B: Deductible (investment loan) — variable preferred
│   └── Interest-only is acceptable (keeps deduction maximised)
│   └── Borrowed funds go DIRECTLY to investment platform
│   └── Each reborrowing may create a new sub-split for clean tracking
│
└── (Optional) Offset account linked to Split A
    └── Salary and surplus cash sit here, reducing non-deductible interest
```

**Critical rules:**
- Borrowed funds from Split B must go **directly** to the investment platform/broker — not through a personal account, offset, or other loan split. The ATO traces the purpose of borrowed funds from the point of drawdown
- Do not mix deductible and non-deductible borrowings in the same split
- Each reborrowing tranche should be identifiable (some lenders create a sub-split per drawdown)
- Keep all records: loan statements, drawdown confirmations, investment purchase confirmations, showing the direct link between borrowing and investing
- Interest-only on the deductible split is acceptable (and often preferred — keeps deductions higher and directs cash flow to paying down the non-deductible split faster)

### Step 3: Investment Selection

Investments purchased with recycled debt must produce **assessable income** (to support the interest deduction). All investment is delivered through the First Financial Execution Framework via Akambo SMA.

| Vehicle | Income Type | Typical Yield | Franking | Suitability |
|---------|-----------|---------------|----------|-------------|
| Akambo SMA (MA) for income-focused debt recycling | Distributions from income-biased allocation | Higher yield from defensive allocation (Cash + Fixed Interest + equity distributions) | Varies by allocation. Higher Australian equity allocation increases franking | Primary choice where the recycled portfolio must produce income to service the investment loan. MA-A (75% income) or MA-B (55% income) in early stages when LVR is high. Transition to MA-C or MA-D as debt reduces and income obligation drops. See `sma-portfolio-mapping` skill for staged transition guidance |
| Akambo SMA (CA) for growth-focused debt recycling | Distributions | Target drawdown rate | Varies by allocation | Use where client services the investment loan from salary or other cashflow (not from the recycled portfolio). CA0 or CA2 for maximum growth. Portfolio income is a bonus, not a loan-servicing requirement. Designed to meet specified drawdown requirement. Delivered through the execution framework with dynamic management and tactical overlay |
| Akambo SMA (MA-D or MA-E) for growth-focused debt recycling | Distributions | Lower yield, growth focus | Varies by allocation | Use where client services the loan externally and wants maximum growth from the recycled portfolio. High equity allocation (75-90%) with long time horizon. Some income production supports deductibility |
| Akambo Collaborative Model | Distributions | Varies | Varies by allocation | Effectively SMA. Use where collaborative structure suits the client. Same execution framework applies |
| Growth-only / no-income assets | None | 0% | N/A | Do not use. ATO may deny interest deduction if no reasonable expectation of income |

**Recommended approach:**
- Akambo SMA is the default for debt recycled funds, both inside and outside super. This delivers the First Financial execution framework: dynamic portfolio management, quality asset selection, tactical overlay, and continuous risk management
- SMA type selection depends on how the investment loan is serviced:
  - **Income-focused debt recycling (MA range):** Where the recycled portfolio must produce income to service the investment loan, use the MA range. MA-A (25/75 growth/income) or MA-B (45/55) in early stages when LVR is high and income certainty is critical. Transition to MA-C (60/40) or MA-D (75/25) as debt reduces and the income servicing obligation drops. The income tilt ensures the portfolio generates sufficient distributions to cover loan repayments, making the strategy self-evident for ATO purposes
  - **Growth-focused debt recycling (CA range):** Where the client services the loan from salary or other cashflow, use CA0 or CA2 for maximum growth. The portfolio produces some income (distributions) but the primary focus is capital growth. Income is a bonus, not a loan-servicing requirement
- The SMA must produce assessable income (distributions) to support the interest deduction on the investment loan. Confirm income production with Akambo. Run a serviceability check: compare expected distribution yield against after-tax interest cost (see `sma-portfolio-mapping` skill)
- The SMA may hold direct assets, ETFs, or managed funds as building blocks within the portfolio. That is Akambo's implementation decision within the framework
- Avoid: speculative stocks, crypto, vacant land, standalone index funds/ETFs, or anything that does not produce regular assessable income
- See the `sma-portfolio-mapping` skill for the full debt recycling SMA selection decision tree, staged transition guidance, and serviceability check template

### Step 4: Franking Credit Integration

Franking credits are central to debt recycling economics. For a fully franked 4% cash yield:

| Marginal Rate | Cash Dividend | Franking Credit | Grossed-Up | Tax on Grossed-Up | Less Franking Offset | **Net Tax on Dividend** |
|---------------|-------------|-----------------|-----------|-------------------|---------------------|----------------------|
| 32% (30% + ML) | 4.00% | 1.71% | 5.71% | 1.83% | 1.71% | **0.12%** |
| 37% + ML | 4.00% | 1.71% | 5.71% | 2.23% | 1.71% | **0.52%** |
| 45% + ML | 4.00% | 1.71% | 5.71% | 2.69% | 1.71% | **0.98%** |

At a 32% marginal rate, fully franked dividends are almost tax-free (only the 2% Medicare Levy gap creates a tiny liability).

**After-tax cost of deductible debt vs dividend income:**

| Component | At 32% Marginal Rate |
|-----------|---------------------|
| Gross interest rate | 6.00% |
| Tax deduction value | -1.92% |
| **After-tax interest cost** | **4.08%** |
| Cash dividend yield | 4.00% |
| Net tax on dividends | 0.12% |
| **After-tax dividend income** | **3.88%** |
| **Net cost of carry** | **0.20%** |

The dividends almost entirely cover the after-tax interest cost. The remaining cost is trivial, and **capital growth is the bonus on top**.

### Step 5: Year-by-Year Projection

Build a projection showing the debt composition shift and portfolio growth:

| Year | Age | Non-Deductible Debt | Deductible Debt | Total Debt | Investment Portfolio | Deductible Interest | Tax Saving (@ marginal rate) | Cash Dividends | Franking Credits |
|------|-----|--------------------|-----------------|-----------|--------------------|--------------------|-----------------------------|---------------|-----------------|
| 0 | | [Mortgage balance] | $0 | | $0 | $0 | $0 | $0 | $0 |
| 1 | | | | | | | | | |
| 5 | | | | | | | | | |
| 10 | | | | | | | | | |
| 15 | | | | | | | | | |

**Key milestones to highlight:**
- Year when non-deductible debt reaches $0 (all remaining debt is deductible)
- Cumulative tax savings over the strategy period
- Portfolio value at retirement
- Net wealth impact (portfolio value minus deductible debt = net benefit)

### Step 6: How the Recycling Cycle Works (Annual Process)

Each year (or more frequently if desired):

```
1. EXTRA REPAYMENT
   → Client pays $X extra into the home loan (Split A — non-deductible)
   → Non-deductible balance reduces by $X

2. REBORROW
   → Client redraws $X from a new investment split (Split B — deductible)
   → Funds transferred DIRECTLY to investment platform

3. INVEST
   → Purchase via Akambo SMA (CA or MA per client circumstances)
   → Keep purchase confirmation for records

4. RECEIVE DIVIDENDS
   → Dividends paid into home loan offset or directly onto Split A
   → Further reduces non-deductible balance
   → (Or dividends reborrowed and reinvested — turbocharges the strategy)

5. CLAIM DEDUCTIONS
   → Interest on Split B is tax-deductible
   → Claim in tax return → refund or reduced tax payable
   → Direct tax refund into home loan offset or Split A

6. REPEAT
   → Next year, make another extra repayment and reborrow
```

### Step 7: Acceleration Techniques

| Technique | How It Works | Impact |
|-----------|-------------|--------|
| Recycle dividends | Dividends paid into home loan, then reborrowed and reinvested | Increases recycled amount beyond the annual cash contribution |
| Recycle tax refunds | Tax refund from interest deductions paid into home loan, then reborrowed | Further accelerates the non-deductible paydown |
| Salary into offset | All salary sits in offset account linked to non-deductible split, reducing interest | More of each scheduled payment goes to principal → more available to redraw |
| Lump sum recycling | Bonus, inheritance, or asset sale → large extra repayment → large reborrowing | Jumps the strategy forward significantly |
| Increasing contributions | As salary grows, increase the annual recycling amount | Accelerates debt conversion |

### Step 8: Risk Management

| Risk | Mitigation |
|------|-----------|
| **Market downturn** | Long time horizon (7+ years). Diversified portfolio. Don't panic-sell — the debt recycling benefit persists through market cycles. Margin call risk does NOT apply (this is a standard home loan, not a margin loan) |
| **Interest rate rise** | Model a stress test at current rate + 2-3%. Ensure debt remains serviceable. Variable rate on deductible split means deduction increases with rates (partial natural hedge) |
| **Job loss** | Emergency fund covers 6 months. Income protection insurance. Dividends from portfolio provide partial income. Can pause recycling at any time without unwinding |
| **Investment produces no income** | Akambo SMA produces distributions by design. For income-focused debt recycling, the MA range (MA-A or MA-B) has a high income allocation (55-75%) specifically to ensure income production. Confirm income production for the selected SMA type with Akambo. ATO may deny deduction if no reasonable expectation of income |
| **Loan structure error** | Get it right from the start — work with a mortgage broker who understands debt recycling. Do not commingle splits |
| **ATO challenge** | Maintain meticulous records. Each borrowing → investment link must be documented. Interest deductibility is well-established in tax law (TR 2000/2) — the risk is in execution, not the concept |

**Stress test table:**

| Scenario | Impact on Strategy |
|----------|--------------------|
| Interest rates rise to 8% | After-tax cost rises to 5.44%. Dividends (4%) still partially offset. Tax deduction value increases. Strategy still works but net carry cost rises |
| 30% market crash in Year 1 | Portfolio value drops but dividends continue. Debt unchanged. Recovery over remaining years. No margin calls. Do not sell |
| Job loss for 6 months | Emergency fund covers expenses. Pause extra repayments. Continue holding investments. Resume when income restored |
| Dividends cut by 50% | Net carry cost increases. Deductions still apply. Strategy still works but less efficiently |
| ATO denies deduction | Low risk if structured correctly. Risk is in execution (commingling funds, no-income assets), not in the concept |

### Step 9: Exit Strategy at Retirement

At retirement, the client will have:
1. **Home**: fully owned (non-deductible debt cleared, possibly years earlier)
2. **Investment portfolio**: built over the strategy period
3. **Deductible debt**: remaining balance on the investment split

**Options at retirement:**

| Option | Outcome | Tax Implication |
|--------|---------|-----------------|
| **Keep the investments and debt** | Interest remains deductible against investment income (dividends). In pension phase with low/nil marginal rate, the deduction has less value but the debt cost is also lower | Interest deduction reduces assessable income |
| **Sell investments, clear debt** | Crystallise CGT (50% discount if held >12 months). Use proceeds to pay off deductible debt. Remainder is additional retirement capital | CGT on gains, but net proceeds add to retirement pool |
| **Sell investments, contribute to super** | Sell, pay CGT, contribute net proceeds as non-concessional super (if under cap and balance <$1.9M) | Moves wealth into tax-free pension environment |
| **Partial sell-down** | Sell enough to clear the debt, keep the rest for income and flexibility | Manage CGT by staging sales across financial years |

**Recommended approach:** Depends on the client's tax position at retirement. If entering pension phase with low income, selling and moving to super (if cap space allows) is often optimal. If income is higher, keep the investments and deductions.

### Step 10: Record-Keeping Requirements

Maintain a complete debt recycling file:

- **Loan facility letter** showing split structure
- **Each drawdown confirmation** from Split B (deductible)
- **Corresponding investment purchase confirmation** showing same amount on same/next day
- **Interest statements** for Split B (annual — for tax return)
- **Dividend statements** (for income and franking credit reporting)
- **Annual portfolio valuation** (tracking growth)
- **Tax returns** showing interest deductions claimed

Keep for **5 years after the last relevant tax return** (standard ATO record-keeping requirement). In practice, keep for the life of the strategy plus 5 years.

### Step 11: Output — SOA Summary Request Input

This skill produces the **analytical working papers** that feed into the SOA Summary Request (assembled by the `strategy-request` skill). See [CONVENTIONS.md](../../CONVENTIONS.md) for house style rules.

**Feeds into Summary of Advice:**
- Debt recycling action items (loan restructure, extra repayments, reborrow, invest, claim deductions)
- Each item as a short, directive sentence (e.g., "Restructure home loan into Split A (non-deductible) and Split B (deductible investment loan). Redirect $20,000 p.a. ($1,667/month) surplus to debt recycling.")

**Feeds into Projection Parameters:**
- Mortgage balance, rate, term, repayment schedule
- Surplus cashflow available for recycling (show derivation)
- Marginal tax rate (current and projected)
- Interest rate, investment return, dividend yield, franking percentage, inflation
- +3.0% interest rate stress test results
- Source-of-Truth for each input

**Feeds into Alternatives:**
- Full debt paydown before investing (dismiss: opportunity cost over time horizon)
- Non-super investing without leverage (dismiss: loses deductible interest benefit)
- Direct shares vs SMA for recycled portfolio

**Feeds into Product Considerations:**
- Platform for investment portfolio (paraplanning to determine lowest total cost)
- SMA type selection rationale (CA vs MA)

**Feeds into Notes to AA or Paraplanning:**
- Loan restructure: confirm lender supports split facility with redraw
- Investment platform: confirm APL compliance for recommended SMA
- Risk profile: confirm leveraged strategy aligns with documented risk profile
- Accountant/tax agent involvement for tax return preparation
- Record-keeping checklist for client (drawdown to investment purchase trail)
- Mortgage broker referral if loan restructure required
- Gap items to request from client

**Calculation Workings (appendix):**
- Suitability assessment with all factors documented
- After-tax cost of carry analysis with full workings (gross interest, deduction value, net cost vs dividend income)
- Year-by-year projection (debt composition shift, portfolio growth, tax savings), every row calculable from stated assumptions
- Amortisation schedule (non-deductible paydown)
- Deductible interest and tax saving by year
- Portfolio accumulation (FV of annual contributions at assumed return)
- Franking credit and dividend tax calculation at client's marginal rate
- Crossover year (when non-deductible debt reaches $0)
- Stress test results (rate rise, market crash, job loss, dividend cut)
- Exit strategy options at retirement with CGT and NCC modelling
- Comparison: recommended position vs do-nothing (quantified difference)
- Legislative references: TR 2000/2, s8-1 ITAA 1997, s961B

## Important Notes

- **This output is an adviser working paper. It is not a client-facing document.** The `strategy-request` skill assembles the final SOA Summary Request for paraplanning.
- All calculations must show full workings. Paraplanning needs the basis for advice, not just conclusions.
- All tables must follow house style: no bullets in cells, no em dashes, short directive sentences.
- Debt recycling is not a tax scheme. Interest deductibility on investment borrowings is established in Australian tax law (TR 2000/2).
- Funds must flow directly from the investment loan split to the investment purchase. Any detour breaks the deductibility nexus.
- Do not mix deductible and non-deductible borrowings in the same loan split.
- This is a leveraged strategy. The adviser must document that the client understands and accepts the risk.
- Emergency fund and adequate insurance are prerequisites. Document in the brief.
- The adviser and paraplanner ensure the final SOA/ROA meets Best Interest Duty (s961B) and FASEA Code of Ethics.
