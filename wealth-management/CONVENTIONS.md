# Output Conventions

## Purpose

This plugin produces **SOA Summary Requests** (Strategy Requests). These are structured adviser working papers that go to associates and paraplanners as CRM-ready instructions for drafting the formal Statement of Advice (SOA) or Record of Advice (ROA).

The adviser uses this tool to run client analysis, model strategies, and produce a Strategy Request in the standard template format. The output must be clean enough to paste directly into CRM.

## These outputs are NOT

- Client-facing advice documents
- Statements of Advice (SOA) or Records of Advice (ROA)
- Compliant advice documents ready for distribution to clients
- Instructions for the client (SOA comes first, implementation later)

The adviser and paraplanner remain responsible for ensuring all formal documentation meets AFSL, ASIC, and Best Interest Duty requirements.

## These outputs ARE

- **SOA Summary Requests** with strategy analysis and CRM-ready instructions
- **Calculations with full workings** as the evidentiary basis for recommendations
- **Paraplanning briefs** with clear separation of actions, assumptions, and notes
- **Internal documents** for associates and paraplanners only

## SOA Summary Request Format

Every output must follow this mandatory section structure. See the `strategy-request` skill for the full template.

### Entities Receiving Advice
Table listing all clients and entities receiving advice.

### Summary of Advice
Numbered table rows. Each row is one action item. Short, directive sentences. Actions only. Assumptions and modelling parameters go to Projection Parameters, not here.

### Alternative Strategies (Considered and Dismissed)
Multi-row single-column table. Each row is one dismissed strategy. Each cell contains: heading, explanation of why it was viable, and clear dismissal reason. The recommended strategy is never listed here.

### Alternative Product Considerations
Multi-row single-column table. Each row is one dismissed product or platform. Each cell contains: product/platform name, why it was viable, and dismissal reason. The recommended product is never listed here.

### Projection Parameters / Requests / Assumptions
Table with Parameter and Value columns. All modelling inputs go here (salary, super balance, cash, liquidity floor, savings, spending, risk profile, investment assumptions, insurance handling, contributions and timing, carry-forward).

### Target Market Determination (TMD)
Table confirming TMD for each client/entity.

### Notes to AA or Paraplanning
Table listing gap items to request from client and any specific paraplanning instructions.

### Change Log
Version, date, and notes for each revision.

## House Style Rules

These rules apply to all output. No exceptions.

1. **All tables.** Every section must be structured as a table. No hanging text, no loose bullets, no paragraphs outside tables.
2. **No bullets inside table cells.** Use sentences.
3. **No nested tables.** One level only.
4. **No em dashes.** Use commas, semicolons, or full stops.
5. **Bold only where needed.** Do not over-format.
6. **Short, directive sentences.** CRM-pasteable. No flowery language.
7. **Single-client default.** When there is no partner, do not include partner columns or references.
8. **Actions separate from assumptions.** Summary of Advice is action-only. Assumptions go to Projection Parameters.
9. **Key numbers twice where helpful.** Annual and monthly (e.g., "$15,600 p.a. ($1,300/month)").
10. **Platform selection.** State that paraplanning will determine lowest total cost unless a specific platform is required.
11. **Related-party loans.** Handled by client's lawyer with accountant input. No loan-term drafting in the SOA.
12. **SOA before implementation.** Do not ask the client to confirm sequencing. SOA comes first, implementation later. Exception only where explicitly noted (e.g., "Post-SOA action").

## Calculation Standards

- **Show workings**: every calculation must show inputs, formula, and result
- **State assumptions**: all modelling inputs stated explicitly in Projection Parameters
- **Source-of-Truth**: for each key input (salary, SG, balances, contributions, expenses, beneficiaries), log the document name, date, and section the figure came from
- **Current legislative thresholds**: use current rates and caps
- **Financial year alignment**: all tax modelling uses the Australian financial year (1 July to 30 June)
- **Nominal and real values**: show both where relevant (especially retirement projections over 10+ years)
- **Marginal vs average tax rates**: use marginal rates for strategy benefit calculations
- **Rounding**: calculations to the nearest dollar, percentages to two decimal places

## Global Rules

These rules apply across all SOA Summary Requests. They are derived from case experience and must be checked on every engagement.

### Mandatory Information Gathering
Before running any calculations, confirm the following critical inputs are available. If any are missing, **ask the adviser for them** rather than estimating or proceeding without them. All calculations must be fully worked from verified data.

**Always required:**
- Total superannuation balance (TSB) for each member (as at prior 30 June and current estimate). TSB determines eligibility for carry-forward, NCC cap, bring-forward, co-contributions, and spouse contribution offset
- Carry-forward concessional cap: verified via ATO portal (MyGov > ATO Online > Super > Concessional contributions). Do not estimate. Record verified amounts by FY with retrieval date
- Recent non-concessional contributions (NCC): any NCC made in the current or prior FYs that may affect the annual cap ($120,000) or bring-forward trigger ($360,000 over 3 years). If bring-forward was triggered, confirm which FY it started and remaining capacity
- Current FY concessional contributions to date (SG + salary sacrifice + personal deductible): needed to calculate remaining cap space
- Salary (ex-super) and employment details
- Current super fund(s), balances, and investment options
- Cash balances (bank, offset, term deposits)
- Debt balances and terms (mortgage, HECS, investment loans)
- Annual expenses and surplus cashflow

**Ask if not provided:**
- Risk profile (scored and selected)
- Insurance status (inside/outside super, cover amounts)
- Beneficiary nominations (type, percentages, expiry)
- Trust or entity structures
- Estate planning status (will, POA, BDBN)
- Recent capital gains events or large transactions

Do not run projections on assumed or placeholder data for the items listed above. If the adviser provides incomplete information, flag the gaps and ask before proceeding.

### Carry-Forward Verification
Before finalising contributions, obtain MyGov > ATO Online > Super > More Information > Concessional contributions screenshots/PDFs showing unused cap amounts by FY. Use FIFO and check expiry (e.g., 2020-21 expiring 30 June 2026). Record the verified dollar amounts and the as-at retrieval date.

### June Processing Cut-Offs
Contributions count in the FY the fund receives them. Highlight processing cut-offs and advise client on bank transfer windows.

### Risk Profile Mismatch Disclosure
If risk score does not equal selected portfolio (e.g., B scored, C selected), include a short rationale: risk required, timeframe, and ongoing invested through drawdown. Confirm client acceptance.

### Beneficiary and Estate Notes
Capture current nomination types and percentages. Where nominees may be non-tax dependants, add short plain-English tax implication note and "review at retirement".

### Insurance Scope Discipline
Insurance product advice is out of scope by default. Model premium cashflow drag only. Insurance product advice is handled by Akambo (part of the group, shared licensee). If retaining an existing fund for cover continuity, specify cash amount to retain and purpose.

### Alternatives Doctrine
Alternatives must be viable strategy or product options and must include a clear dismissal (cohesive single-cell entry per alternative). The recommended platform/portfolio is never listed as an alternative. Keep Alternatives (Strategies) and Alternative Product Considerations as separate sections.

### Mandatory Call-Outs
Always call out the following where applicable:
- Liquidity floor integrity (default per adviser preferences)
- Insurance continuity for super rollovers
- +3.0% interest-rate stress test (modelling requirement, not an alternative)
