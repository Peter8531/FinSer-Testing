# Wealth Management Plugin — Guide for Australian Financial Planners

This guide reviews the wealth-management plugin through the lens of an Australian financial planner (financial adviser) and maps each workflow to Australian rules, terminology, and practice.

## Quick Compatibility Summary

| Workflow | Works in AU? | Effort to Adapt |
|----------|-------------|-----------------|
| `/client-review` | Yes, mostly | Low — swap terminology |
| `/client-report` | Yes, mostly | Low — swap account types and benchmarks |
| `/proposal` | Yes | Low — swap terminology and fee disclosure format |
| `/financial-plan` | Partially | High — super, Age Pension, CGT discount, franking |
| `/rebalance` | Partially | Medium — different account types, no wash sale rule |
| `/tlh` | Partially | Medium — different tax rules, no wash sale rule, Part IVA |

---

## Terminology: US to AU Translation

Swap these terms throughout all outputs:

| US Term | Australian Equivalent |
|---------|----------------------|
| Financial advisor | Financial adviser |
| 401(k) | Superannuation (accumulation phase) |
| IRA / Traditional IRA | Superannuation (accumulation phase) |
| Roth IRA | Non-concessional super contributions (loosely) |
| Social Security | Age Pension (Centrelink) |
| IRS | ATO (Australian Taxation Office) |
| SEC | ASIC (Australian Securities and Investments Commission) |
| Brokerage / taxable account | Personal investment account |
| 529 Plan | No equivalent (education savings are not tax-advantaged) |
| CD (Certificate of Deposit) | Term deposit |
| REIT | A-REIT (ASX-listed) |
| Mutual fund | Managed fund |
| Closed-end fund | LIC (Listed Investment Company) |
| Estate tax | No equivalent (abolished 1979) |
| Gift tax | No equivalent |
| RMD (Required Minimum Distribution) | Minimum pension drawdown |
| Fiduciary standard | Best Interest Duty (s961B Corporations Act) |
| Suitability | Appropriate advice obligation |
| Fiscal year (Jan-Dec) | Financial year (1 July - 30 June) |
| Dollar ($) | AUD ($) |
| W-2 | Income Statement (via Single Touch Payroll) |
| 1099-DIV | AMMA Statement / Distribution Statement |
| Check / checking account | Transaction account |

---

## Workflow-by-Workflow Review

### 1. Client Review (`/client-review`) — Low Adaptation

**What works as-is:**
- Meeting agenda structure (market overview, performance, allocation, planning, action items)
- Performance attribution (contributors / detractors)
- Drift analysis against target allocation
- "Lead with what the client cares about" philosophy
- Action item tracking

**What to change:**

Account types — replace:
- `Taxable, IRA, Roth, 401(k), trust` → `Personal, Super (accumulation), Super (pension), SMSF, Family Trust, Company, Joint`

Asset classes — replace:
- `US Large Cap` → `Australian Equities (ASX 200)`
- `US Mid/Small` → `Australian Small/Mid Cap`
- Keep `International Developed`, `Emerging Markets`
- Add `Australian Fixed Income` (distinct from global)
- Add `Australian Property (direct / A-REITs)`
- Add `Cash / Term Deposits`

Proactive recommendations — replace:
- `Roth conversion opportunities` → `Transition to Retirement (TTR) strategies`, `Super contribution strategies (salary sacrifice, spouse contributions, carry-forward)`
- `Tax-loss harvesting` → `Capital loss harvesting (noting Part IVA)`, `Franking credit optimisation`
- `Beneficiary updates` → `Binding Death Benefit Nomination (BDBN) review`, `Super nomination currency check (lapsing vs non-lapsing)`
- `Insurance review (life, disability, LTC)` → `Insurance review (life, TPD, income protection, trauma — inside and outside super)`
- Add `Centrelink Age Pension review (means testing impact)`

---

### 2. Client Report (`/client-report`) — Low Adaptation

**What works as-is:**
- Report structure (cover, executive summary, performance, allocation, holdings, commentary, activity, planning notes, disclosures)
- Performance summary tables (QTD, YTD, 1-Year, 3-Year, 5-Year, ITD)
- Allocation overview with charts
- Holdings detail
- Market commentary approach
- Activity summary

**What to change:**

Account table — replace example:
```
| Account          | Type                 | Value | QTD | YTD |
|------------------|----------------------|-------|-----|-----|
| Personal         | Individual           |       |     |     |
| John Super       | Accumulation         |       |     |     |
| Jane Super       | Pension Phase        |       |     |     |
| Family Trust     | Discretionary Trust  |       |     |     |
| Total            |                      |       |     |     |
```

Benchmarks — replace:
- `S&P 500, 60/40 blend` → `S&P/ASX 200, ASX 200 + Bloomberg AusBond Composite blend, MSCI World (AUD hedged)`

Reporting period:
- Align to Australian financial year (July-June) for YTD and annual
- Quarterly still works as calendar quarters

Add to holdings detail:
- Franking credit income (grossed-up yield vs cash yield)
- CGT discount eligibility (held >12 months indicator)

Disclosures:
- Must comply with AFSL obligations and SOA/ROA requirements
- Reference ASIC regulatory guidance, not SEC

---

### 3. Investment Proposal (`/proposal`) — Low Adaptation

**What works as-is:**
- Proposal structure (About Firm, Understanding Needs, Strategy, Expected Outcomes, Fees, Getting Started)
- Prospect context gathering
- Customisation advice (match tone to prospect type)
- Follow-up and compliance notes

**What to change:**

"About Our Firm" section:
- Reference AFSL number and authorised representative details
- Mention AFCA (Australian Financial Complaints Authority) membership
- Reference Code of Ethics compliance

Fee structure:
- Must comply with Fee Disclosure Statement (FDS) requirements
- Include ongoing fee arrangement renewal requirements
- Disclose any platform fees, insurance commissions, or conflicted remuneration

Proposed allocation vehicles:
- Replace `SPY, VTI, AGG` style examples with ASX-listed equivalents: `VAS (Vanguard Australian Shares), VGS (Vanguard International Shares), VAF (Vanguard Australian Fixed Interest)`
- Include LICs, A-REITs, managed funds on platforms (Netwealth, HUB24, BT Panorama, Macquarie Wrap)

"Getting Started" section:
- Account opening → include super rollover process, ATO rollover form
- Must issue a Statement of Advice (SOA) before implementation
- 14-day cooling-off period for most financial products

---

### 4. Financial Plan (`/financial-plan`) — High Adaptation

This is where the US assumptions are deepest. Major rework needed.

**Step 1 — Client Profile: Replace**

Income sources:
- `Social Security estimates` → `Age Pension estimate (Centrelink)`, `Super pension income`, `Account-based pension drawdown`
- Add: `Franking credit refunds`, `Rental income (with negative gearing)`, `Centrelink benefits`

Accounts:
- `401(k), IRA, Roth` → `Super (accumulation)`, `Super (pension phase)`, `SMSF`, `Personal investments`, `Family trust`, `Company`, `Insurance bonds`

Liabilities:
- `Student loans` → `HECS-HELP debt` (repaid through tax system at income-based rates)

Insurance:
- `Life, disability, LTC, health` → `Life (inside/outside super)`, `TPD (any occupation vs own occupation)`, `Income protection (indemnity value, 2-year benefit inside super)`, `Trauma/critical illness (outside super only)`, `Private health insurance (Medicare Levy Surcharge relevance)`

Estate:
- Remove: `Gifting strategy (annual exclusion, lifetime exemption)` — no gift tax in AU
- Replace with: `Binding Death Benefit Nomination status`, `Testamentary trust planning`, `Super death benefits tax (dependant vs non-dependant recipients)`, `Enduring Power of Attorney / Enduring Guardian (state-specific)`

**Step 2 — Cash Flow Analysis: Replace**

Tax calculation:
- Use Australian tax brackets (0% up to $18,200, then 16%/30%/37%/45%)
- Add Medicare Levy (2%)
- Model franking credit offsets and refunds
- Financial year is July-June, not calendar year

Savings direction:
- `Pre-tax, Roth, taxable` → `Concessional super contributions (salary sacrifice)`, `Non-concessional super contributions`, `Personal investments`, `Trust distributions`

**Step 3 — Retirement Projections: Replace entirely**

Accumulation phase:
- `401(k), IRA contributions` → `Super Guarantee (11.5%, rising to 12%)`, `Salary sacrifice`, `Non-concessional contributions`, `Carry-forward unused concessional cap`
- Contribution caps: $30,000 concessional, $120,000 non-concessional (with bring-forward rule up to $360,000)
- Earnings taxed at 15% in accumulation (10% for discounted CGT gains)

Distribution phase:
- `Social Security start age 62/67/70` → `Age Pension eligibility at 67`, model Centrelink means testing (income test and assets test)
- `RMDs` → `Minimum pension drawdown rates` (4% age 60-64, 5% age 65-74, 6% age 75-79, 7% age 80-84, 9% age 85-89, 11% age 90-94, 14% age 95+)
- `Roth conversions` → `Transition to Retirement (TTR) strategies`
- Transfer Balance Cap: $1.9 million limit on pension phase transfers
- Pension phase earnings: tax-free (within TBC)
- Division 293 tax for high earners (>$250,000)

Scenarios to model (replacing US scenarios):
| Scenario | Probability of Success | Portfolio at 90 |
|----------|----------------------|-----------------|
| Base case | | |
| Retire at preservation age (60) | | |
| Maximise salary sacrifice to retirement | | |
| Downsize home (downsizer contribution $300k each) | | |
| 20% market drop in Year 1 | | |
| One spouse needs aged care | | |
| Centrelink Age Pension partial eligibility | | |

**Step 4 — Goal-Specific Analysis: Replace**

Education funding:
- Remove 529 plan references (no Australian equivalent)
- Model education costs directly — no tax-advantaged vehicle
- Consider HECS-HELP as an alternative to upfront payment

Estate planning — completely rework:
- Remove: estate tax exposure, federal/state estate tax, lifetime exemption, annual exclusion gifting
- Add: Super death benefits tax planning (taxable component to non-dependants at 15-30% + Medicare levy)
- Add: Testamentary trust planning (income splitting for minor beneficiaries at adult rates)
- Add: BDBN management (lapsing vs non-lapsing, 3-year renewal)
- Add: Enduring Power of Attorney and Enduring Guardian (state-specific legislation)
- Add: Aged care planning (RAD vs DAP, means-tested care fees)

Risk management:
- `Life insurance needs` → model inside-super vs outside-super trade-off (premium cost vs super balance erosion)
- `TPD` → note "own occupation" can only be held outside super since April 2020
- `Income protection` → APRA reforms limit inside-super IP to indemnity value, 2-year benefit period
- `Trauma / critical illness` → must be held outside super
- `LTC` → not a standard AU product; model aged care costs instead
- Add `Private health insurance review (Medicare Levy Surcharge avoidance)`

**Step 6 — Recommendations: Replace**

1. Super contribution strategy (maximise concessional, consider non-concessional)
2. Asset allocation adjustments
3. Tax optimisation (franking credit strategies, CGT discount timing, salary sacrifice, negative gearing)
4. Centrelink optimisation (structuring assets to maximise Age Pension)
5. Insurance structure review (inside vs outside super)
6. BDBN and estate document updates
7. Aged care planning (if relevant)

---

### 5. Portfolio Rebalance (`/rebalance`) — Medium Adaptation

**What works as-is:**
- Drift analysis methodology
- Rebalancing band thresholds (3-5%)
- "Don't rebalance for rebalancing's sake"
- Tax-aware trade prioritisation
- Document rationale for compliance

**What to change:**

Account types:
- `Taxable, IRA, Roth, 401(k)` → `Personal, Super (accumulation), Super (pension), SMSF, Family Trust`

Tax-aware rebalancing rules — replace:
- `Prefer tax-advantaged accounts (IRA, Roth) first` → `Prefer super accounts first (no personal tax on trades; accumulation taxed at 15% / pension phase tax-free)`
- `Watch for wash sale rules (30-day window)` → Remove. Australia has no wash sale rule. However, note that the ATO can challenge schemes under **Part IVA** (general anti-avoidance) if the dominant purpose of a transaction is a tax benefit
- Add: `Consider CGT discount — if selling profitable positions, prefer assets held >12 months (50% CGT discount for individuals, 33% for super funds)`
- Add: `Consider franking credit impact — selling Australian equities near ex-dividend dates affects franking credit entitlement`

Asset location — replace:
- `Tax-deferred (IRA/401k): Bonds, REITs` → `Super (accumulation): Higher-growth assets benefit from 15% tax rate vs marginal rates`
- `Roth: Highest growth` → `Super (pension): Tax-free earnings — hold highest-growth assets here`
- `Taxable: Tax-efficient equity, munis` → `Personal: Australian equities (franking credits reduce tax), ETFs (tax-efficient), consider negative gearing for property`

Cash flow considerations:
- `RMDs` → `Minimum pension drawdown requirements`
- Add: `Pending super contributions (concessional cap space remaining this FY)`

---

### 6. Tax-Loss Harvesting (`/tlh`) — Medium Adaptation

**What works as-is:**
- Basic concept of realising losses to offset gains
- Scanning for unrealised losses
- Prioritisation framework (largest loss first)
- Replacement security concept
- Post-harvest tracking

**What to change:**

Gain/loss budget — replace:
- `Short-term losses × marginal ordinary income rate` → In Australia, there is no separate short-term/long-term rate distinction. All capital gains are added to assessable income at marginal rates. The key distinction is:
  - Assets held **<12 months**: full capital gain is assessable
  - Assets held **>12 months**: 50% CGT discount for individuals (only half the gain is assessable)
  - Super funds: 33% CGT discount (taxed at effectively 10%)
- `$3,000 net loss deduction against ordinary income` → Remove. In Australia, **capital losses can ONLY offset capital gains** — they cannot offset ordinary income. Unused capital losses carry forward indefinitely
- `Carryforward losses` → Same concept exists in AU

Tax savings calculation:
```
Harvested loss offsets gains at:
- Individual marginal rate (up to 45% + 2% Medicare levy) on undiscounted gains
- Half that on discounted gains (held >12 months)
- 15% (or 10% discounted) within super accumulation
- 0% within super pension phase (no tax benefit from harvesting)
```

Wash sale rules — replace entirely:
- Australia has **no wash sale rule**. You can sell and immediately repurchase the same security
- **However**: the ATO can apply **Part IVA** (general anti-avoidance provisions) if the **dominant purpose** of the transaction is obtaining a tax benefit
- Practical guidance: if there is a genuine investment reason for the trade (e.g., rebalancing, switching to a lower-cost fund), harvesting the loss alongside that is fine. Selling and immediately buying the same security purely for a tax loss may be challenged
- Remove the 30-day wash sale window tracking entirely
- Remove "substantially identical" security analysis — not an Australian concept

Replacement securities — update examples:
```
| Sell | Replace With | Reason |
|------|-------------|--------|
| Vanguard Australian Shares (VAS) | iShares Core S&P/ASX 200 (IOZ) | Similar AU equity exposure |
| Vanguard International Shares (VGS) | iShares Core MSCI World (IWLD) | Similar global equity exposure |
| BHP Group (BHP) | Rio Tinto (RIO) | Same sector, different company |
```

Important notes — add:
- Capital losses in super pension phase provide no tax benefit (earnings are already tax-free)
- Capital losses cannot offset franking credit refunds
- Keep records for CGT schedule in tax return
- Consider timing relative to 30 June (end of financial year, not 31 December)
- EOFY (end of financial year) is prime harvesting season in Australia, not calendar year-end

---

## AU-Specific Concepts Not Covered by Any Existing Skill

These are common Australian financial planning workflows that have no equivalent in the current plugin:

1. **Superannuation strategy** — contribution optimisation, TTR, SMSF setup and compliance, pension phase transition, transfer balance cap management
2. **Centrelink optimisation** — means testing (income test / assets test), deeming rates, structuring to maximise Age Pension
3. **Franking credit strategy** — portfolio construction to maximise imputation credits, especially for retirees in zero-tax pension phase
4. **Negative gearing analysis** — investment property cash flow modelling with tax deductions
5. **SMSF administration** — investment strategy documentation, audit preparation, sole purpose test compliance
6. **Statement of Advice (SOA)** — regulatory document generation compliant with Corporations Act requirements
7. **Aged care planning** — RAD (Refundable Accommodation Deposit) vs DAP (Daily Accommodation Payment), means-tested care fees, impact on Age Pension

---

## Regulatory Compliance Differences

| Requirement | US (Current Plugin) | Australia (What You Need) |
|-------------|--------------------|-----------------------|
| Licensing | SEC/FINRA registration | AFSL or Authorised Representative |
| Advice documentation | Fiduciary disclosure | Statement of Advice (SOA) / Record of Advice (ROA) |
| Ethical standard | Fiduciary duty (varies) | FASEA Code of Ethics (12 standards) |
| Complaints | FINRA arbitration | AFCA (Australian Financial Complaints Authority) |
| Regulator | SEC + FINRA | ASIC |
| Prudential | N/A (for advisers) | APRA (for super funds, insurers) |
| Education | CFP, Series exams | FASEA-approved degree + national exam + professional year |
| Fee disclosure | Form ADV Part 2 | Fee Disclosure Statement (FDS) + ongoing fee renewal |
| Best interest | Reg BI (broker-dealers) / fiduciary (RIAs) | Best Interest Duty s961B (universal for personal advice) |
| Cooling-off | Varies | 14 days for most financial products |

---

## Recommendation

For an Australian financial planner, the **client-facing workflows** (client review, client report, investment proposal) are immediately useful with minor terminology swaps. The **financial planning, rebalancing, and tax** workflows need significant rework to handle superannuation, franking credits, CGT discount, Centrelink means testing, and Part IVA anti-avoidance provisions.

The highest-value adaptation would be to create Australian-specific versions of:
1. **Financial plan skill** — the most heavily US-dependent
2. **Super strategy skill** — entirely new, no US equivalent
3. **Tax-loss harvesting skill** — different rules, different year-end, no wash sales

The plugin architecture makes this straightforward — each skill is a standalone markdown file that can be edited or duplicated without affecting the others.
