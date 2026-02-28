# Debt Recycling

description: Model and implement a debt recycling strategy that converts non-deductible home loan debt into tax-deductible investment debt. Covers loan structuring, investment selection, tax deduction calculations, franking credit integration, risk assessment, and year-by-year projections. Triggers on "debt recycling", "convert mortgage to deductible", "deductible debt", "recycle mortgage", or "non-deductible to deductible".

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

Investments purchased with recycled debt must produce **assessable income** (to support the interest deduction):

| Vehicle | Income Type | Typical Yield | Franking | Suitability |
|---------|-----------|---------------|----------|-------------|
| Broad AU equity ETFs (VAS, IOZ, A200) | Dividends | 3.5-4.5% | ~80-100% franked | Excellent — diversified, income-producing, franked |
| Direct ASX blue chips (CBA, BHP, WES, WOW) | Dividends | 3.5-5.5% | Typically 100% franked | Good — but concentration risk |
| Listed Investment Companies (AFIC, Argo, Milton) | Dividends | 3.5-4.5% | 100% franked typically | Good — dividend smoothing, fully franked |
| International equity ETFs (VGS, IVV) | Dividends | 1-2% | Unfranked | Acceptable — lower yield but diversification benefit |
| Managed funds (AU equity) | Distributions | Varies | Varies | Acceptable — watch for CGT distributions |
| Growth-only / no-income assets | None | 0% | N/A | **Risky** — ATO may deny interest deduction if no income expectation |

**Recommended approach:**
- Core holding: diversified Australian equity ETF (VAS or IOZ) — income-producing, franked, low cost
- Satellite: international equity ETF (VGS) for diversification — lower yield but still income-producing
- Suggested split: 60-70% Australian equity, 30-40% international equity
- Avoid: speculative stocks, crypto, vacant land, or anything that doesn't produce regular assessable income

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
   → Purchase income-producing investments (e.g., VAS, IOZ)
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
| **Investment produces no income** | Choose established, income-producing investments (ETFs, blue chips). Avoid speculative assets. ATO may deny deduction if no reasonable expectation of income |
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

### Step 11: Output

- Suitability assessment summary
- Loan restructure instructions for the lender/broker
- Investment recommendation with rationale
- Year-by-year projection (debt composition, portfolio growth, tax savings)
- After-tax cost of carry analysis
- Stress test results
- Exit strategy options
- Record-keeping checklist
- Action plan with timeline

## Important Notes

- Debt recycling is **not a tax scheme** — it is the legitimate conversion of non-deductible debt to deductible debt. Interest deductibility on investment borrowings is well established in Australian tax law (ATO Taxation Ruling TR 2000/2)
- The strategy works because the ATO looks at the **purpose of the borrowed funds** (what the money was used to purchase), not the security for the loan (the home)
- Funds must flow DIRECTLY from the investment loan split to the investment purchase — any detour through personal accounts, offsets, or other splits breaks the deductibility nexus
- Do NOT mix deductible and non-deductible borrowings in the same loan split — ever
- Interest-only on the deductible split is acceptable and often preferable (keeps deductions higher)
- Franking credits are a powerful complement — fully franked dividends at 30% company tax almost fully offset tax at marginal rates up to 32%
- This is a **leveraged strategy** — investments can fall while debt remains. The client must understand and accept this risk
- Emergency fund and adequate insurance are prerequisites, not optional
- The strategy can be paused or stopped at any time — it does not require ongoing commitment to work (existing recycled amounts continue generating deductions)
- Consider the interaction with Centrelink: the investment portfolio will be an assessable asset for Age Pension purposes, but the deductible debt reduces the net assessable amount
- All advice must comply with Best Interest Duty and be documented in an SOA
- Recommend the client involves their accountant/tax agent for tax return preparation to ensure deductions are correctly claimed
