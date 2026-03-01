# Strategy Request

description: Assemble an SOA Summary Request (Strategy Request) for paraplanning. Takes the adviser's strategy analysis and outputs a CRM-ready document in the standard template format with all mandatory sections. This is the final assembly step after running analytical skills (financial-plan, debt-recycling, super-strategy, etc.). Triggers on "strategy request", "SOA request", "SOA summary", "brief paraplanning", or "assemble request".

## Workflow

### Step 1: Confirm Inputs

Before assembling the Strategy Request, confirm the following are available. **If any critical input is missing, ASK the adviser for it before proceeding.** Do not estimate or use placeholder data for items marked as critical.

| Input | Source | Critical | Status |
|-------|--------|----------|--------|
| Client/entity names and advice recipients | Fact find | Yes | |
| Salary (ex-super) and employment details | Payslips | Yes | |
| Cashflow baseline (net income, expenses, current repayments, surplus) | Payslips, bank statements | Yes | |
| Cash balances (inside/outside offset) | Bank/offset statements | Yes | |
| Debt balances (PPR, investment, HECS) | Loan statements | Yes | |
| Total superannuation balance (TSB) per member (as at prior 30 June) | ATO portal, super statements | Yes | |
| Super platforms (current), balances, investment options | Super statements, portal screenshots | Yes | |
| Current FY concessional contributions to date (SG + salary sacrifice + personal deductible) | Payslips, ATO portal | Yes | |
| Carry-forward concessional cap (verified via ATO, not estimated) | MyGov > ATO Online > Super | Yes | |
| Recent NCC (current and prior FYs, bring-forward trigger status) | ATO portal, fund statements | Yes | |
| Insurance status (inside/outside super) | Fund statements | | |
| Trust/entity status | Trust deed, accountant | | |
| Risk profile (scored and selected) | Risk profiling tool | | |
| Special goals (children funding, car purchase, etc.) | Fact find | | |
| Gap items still needed from client | Adviser notes | | |

**Rules:**
- All calculations must be fully worked from verified data. TSB, carry-forward, and NCC history are critical because they determine eligibility for contribution strategies
- If carry-forward concessional cap data is not provided, ask for ATO portal screenshots before modelling contribution strategies
- If TSB is not provided, ask before assessing NCC eligibility, bring-forward availability, or co-contribution entitlement
- If recent NCC is not provided, ask before modelling non-concessional strategies
- Flag any remaining missing items in Notes to AA or Paraplanning

### Step 2: Source-of-Truth Table

For each key modelling input, log the source document, date, and section the figure came from. This table supports the Projection Parameters and is included in the working papers.

| Input | Value | Source Document | Date | Section/Page |
|-------|-------|----------------|------|-------------|
| Salary (ex-super) | | | | |
| SG rate | | | | |
| Super balance(s) | | | | |
| Cash at bank | | | | |
| Current contributions | | | | |
| Expenses | | | | |
| Beneficiary nominations | | | | |

### Step 3: Assemble Entities Receiving Advice

| | Client / Entity | Receiving Advice |
|---|----------------|-----------------|
| 1 | | Yes |

Rules:
- Single-client default. When there is no partner, do not include partner columns or references anywhere in the document.
- List all entities (personal, trust, company, SMSF) that will receive advice.

### Step 4: Assemble Summary of Advice

Numbered rows. Each row is one discrete action item. Short, directive sentences.

| | # | Item |
|---|---|------|
| 1 | 1 | |
| 2 | 2 | |

Rules:
- Actions only. Assumptions and modelling parameters go to Projection Parameters.
- Do not ask the client to confirm sequencing. SOA comes first, implementation later.
- Where platform selection is referenced, state that paraplanning will determine lowest total cost.
- Where related-party loans are involved, note: handled by client's lawyer with accountant input.
- Put key numbers twice where helpful (annual and monthly).
- Add rows as needed. Typical range: 4-12 items depending on complexity.

Typical action items include:
- Super consolidation/rollover (specify from/to, amounts, insurance continuity)
- Contribution strategy (salary sacrifice, NCC, carry-forward, spouse)
- Investment strategy (risk profile, asset allocation, SMA mapping)
- Debt strategy (PPR paydown, refinance, debt recycling structure)
- Trust lending (amount, purpose, accountant/lawyer involvement)
- Insurance scope note (product advice handled by Akambo, part of group; model premium drag only)
- Estate planning referral (BDBN, will update, testamentary trust)
- Post-SOA actions (sell-down, transfers, implementation steps after acceptance)

### Step 5: Assemble Alternative Strategies (Considered and Dismissed)

Each row is one dismissed strategy. Single column. Each cell contains: heading, explanation of why it was viable, and clear dismissal reason combined into one cohesive entry.

| | Alternative (Heading + Explanation + Dismissal) |
|---|------------------------------------------------|
| 1 | |
| 2 | |
| 3 | |

Rules:
- Alternatives must be viable strategies. Do not list straw-man options.
- The recommended strategy is never listed here.
- Each cell is self-contained: heading, why it was considered, why it was dismissed.
- No bullets inside cells. Use sentences.
- Typical minimum: 2-3 alternatives.

Common alternatives library (adapt per case):
- One-hit vs two-year bracket-targeting for contributions
- Non-super investing (dismiss: loses 15% concessional tax advantage at this marginal rate)
- Retaining legacy super fund vs platform rollover (dismiss: higher fees, limited investment menu)
- Salary sacrifice only vs salary sacrifice + NCC (dismiss or accept based on cashflow)
- Full debt paydown vs debt recycling (dismiss based on opportunity cost and time horizon)
- Direct shares vs ETF/SMA (dismiss: concentration risk, higher transaction costs)
- Self-managed (SMSF) vs retail/industry fund (dismiss based on balance, cost, complexity)

### Step 6: Assemble Alternative Product Considerations

Each row is one dismissed product or platform. Single column.

| | Alternative Product (Heading + Explanation + Dismissal) |
|---|-------------------------------------------------------|
| 1 | |
| 2 | |

Rules:
- Product/platform comparisons only. Not strategies.
- The recommended product is never listed here.
- Each cell is self-contained.

Common product alternatives (adapt per case):
- Netwealth vs HUB24 (dismiss on fee comparison, feature set, or SMA availability)
- Morningstar/Mason Stevens vs adviser's preferred SMA provider
- Retain legacy fund vs platform SMA (dismiss on cost, investment menu, reporting)
- Industry fund vs retail wrap (dismiss based on advice integration, flexibility)

### Step 7: Assemble Projection Parameters

All modelling inputs go here. The adviser's analysis (from financial-plan, debt-recycling, super-strategy skills) provides these values.

| | Parameter | Value |
|---|-----------|-------|
| 1 | Salary (ex-super) | |
| 2 | Super balance (as-at date) | |
| 3 | Cash at bank | |
| 4 | Liquidity floor | |
| 5 | Monthly savings | |
| 6 | Pre-retirement spend | |
| 7 | Retirement spend target | |
| 8 | Risk score / Selected profile | |
| 9 | Investment assumptions | |
| 10 | Insurance handling | |
| 11 | Contributions and Timing | Detail |
| 12 | This FY | |
| 13 | Next FY | |
| 14 | Carry-Forward (Estimated; confirm via ATO) | Detail |
| 15 | Estimated availability and expiry | |

Add rows for case-specific parameters:
- Debt recycling: interest rate, recycling amount, investment yield, franking percentage
- Centrelink: means test thresholds, deeming rates, asset restructuring amounts
- Retirement: drawdown rate, longevity assumption, Age Pension commencement age
- Stress tests: +3.0% interest rate stress test (mandatory where debt exists)

### Step 8: Assemble TMD

| | Client / Entity | Confirmation |
|---|----------------|-------------|
| 1 | | Yes / No |

### Step 9: Assemble Notes to AA or Paraplanning

| | Notes |
|---|-------|
| 1 | |

Rules:
- List gap items to request from client.
- List specific paraplanning instructions only where the adviser provides them.
- Flag any risk profile mismatches with rationale.
- Flag any beneficiary/estate concerns (non-tax dependants, lapsing BDBNs).
- Flag any insurance continuity requirements for rollovers.

### Step 10: Change Log

| | Version | Date | Notes |
|---|---------|------|-------|
| 1 | v1 | [Today's date] | Initial Strategy Request |

### Step 11: Output

The assembled SOA Summary Request in full, formatted as clean tables ready to paste into CRM.

All underlying calculation workings from analytical skills (financial-plan, debt-recycling, super-strategy, etc.) are included as an appendix or separate working paper, providing the evidentiary basis for each action item in the Summary of Advice.

## Important Notes

- **This output is an adviser working paper for associates and paraplanning. It is not a client-facing document.** Paraplanning drafts the formal SOA/ROA from this request.
- All tables must paste cleanly to Word/CRM. No bullets, no special characters, no em dashes.
- Summary of Advice is action-only. Assumptions go to Projection Parameters.
- Alternatives are adviser-considered and dismissed. Not new strategies to add.
- Product Considerations are platform/product comparisons. Not strategies.
- Notes list gap items to request from client (not paraplanning instructions unless the adviser asks).
- SOA comes first, implementation later. Do not instruct the client to take action before SOA acceptance.
- The adviser and paraplanner ensure the final SOA/ROA meets Best Interest Duty (s961B) and FASEA Code of Ethics.
- When updating a Strategy Request, update the Change Log with version, date, and what changed.
