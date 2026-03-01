# Client Report

description: Produce an adviser working paper (paraplanning brief) for client performance reports with portfolio returns, allocation breakdowns, franking credit summaries, and market commentary. Suitable for annual or ad-hoc distribution. Output goes to paraplanning for formal SOA/ROA drafting. Triggers on "client report", "performance report", "annual report for [client]", "generate reports", or "client statement".

## Workflow

### Step 1: Report Parameters

- **Client name** and household
- **Reporting period**: Financial year (July-June), half-year, quarter, or custom range
- **Accounts**: All accounts or specific account(s)
- **Benchmark**: S&P/ASX 200, blended benchmark matching target allocation, or custom benchmark from SOA
- **Firm branding**: Logo, colours, AFSL number, disclaimers

### Step 2: Performance Summary

**Household Summary:**

| | QTD | FYTD | 1-Year | 3-Year Ann. | 5-Year Ann. | ITD Ann. |
|---|-----|------|--------|-------------|-------------|----------|
| Portfolio | | | | | | |
| Benchmark | | | | | | |
| +/- | | | | | | |

**By Account:**

| Account | Type | Value | QTD | FYTD | Benchmark |
|---------|------|-------|-----|------|-----------|
| Personal | Individual | | | | |
| John Super | Accumulation | | | | |
| Jane Super | Pension Phase | | | | |
| Family Trust | Discretionary | | | | |
| SMSF | Self-Managed | | | | |
| **Total** | | | | | |

**Income Summary:**

| Category | Amount | Tax Treatment |
|----------|--------|---------------|
| Dividends (cash) | | |
| Franking credits received | | After-tax value: $ |
| Interest income | | |
| Trust distributions | | |
| Super pension income | | Tax-free (age 60+) |
| **Total income** | | |

### Step 3: Allocation Overview

Current allocation with visual (pie chart or bar chart):

| Asset Class | % of Portfolio | $ Value | Benchmark % |
|------------|---------------|---------|-------------|
| Australian Equities | | | |
| International Equities | | | |
| Australian Fixed Income | | | |
| International Fixed Income | | | |
| Property (A-REITs / direct) | | | |
| Alternatives | | | |
| Cash / Term Deposits | | | |

### Step 4: Holdings Detail

| Security | Asset Class | Units | Price | Value | % of Portfolio | Period Return | Franked Yield |
|----------|-----------|-------|-------|-------|---------------|-------------|---------------|
| | | | | | | | |

For Australian equities, include:
- Cash dividend yield
- Grossed-up yield (including franking credits)
- CGT discount eligibility (held >12 months)

### Step 5: Market Commentary

Brief market summary tailored to the client's level of sophistication:
- RBA monetary policy and interest rate movements
- ASX performance and key sector themes
- Global markets and currency (AUD/USD) impact on international holdings
- How it affected the portfolio
- Outlook and positioning rationale (2-3 sentences)
- No jargon for retail clients; can be more technical for sophisticated investors

### Step 6: Activity Summary

- Trades executed during the period
- Super contributions (concessional and non-concessional)
- Pension drawdowns (and compliance with minimum drawdown requirements)
- Dividends and interest received (including franking credits)
- Trust distributions
- Advisory fees charged
- Insurance premiums deducted from super (if applicable)
- Rebalancing activity

### Step 7: Planning Notes

- Progress toward financial goals (retirement, debt reduction, education, etc.)
- Super contribution cap usage this financial year (concessional and non-concessional)
- Any changes to recommendations or strategy
- Centrelink / Age Pension status (if applicable)
- BDBN expiry dates (flag if approaching 3-year renewal)
- Upcoming action items
- Next review date
- Ongoing Fee Arrangement renewal date

### Step 8: Output — SOA Summary Request Input

This skill produces the **analytical working papers** that feed into the SOA Summary Request (assembled by the `strategy-request` skill). See [CONVENTIONS.md](../../CONVENTIONS.md) for house style rules.

**Feeds into Summary of Advice:**
- Progress toward financial goals
- Any changes to recommendations or strategy
- Upcoming action items and next review date, each as a short directive sentence

**Feeds into Projection Parameters:**
- Performance summary tables (household and by account, QTD/FYTD/1-Year/3-Year/5-Year/ITD)
- Income summary including dividends, franking credits, interest, trust distributions, super pension income
- Allocation overview with current vs. benchmark percentages
- Source-of-Truth table for each input (document name, date, section)

**Feeds into Alternatives:**
- Strategies considered and dismissed with rationale (e.g., alternative benchmark selections, different reporting approaches)

**Feeds into Notes to AA or Paraplanning:**
- Gap items to request from client
- Contribution cap usage, Centrelink status, BDBN expiry dates, OFA renewal date
- Firm branding requirements (logo, AFSL number, disclaimers)
- Flag any areas requiring compliance review before client distribution

**Calculation Workings (appendix):**
- Holdings detail with yields, franked yields, and CGT discount eligibility
- Activity summary (trades, contributions, drawdowns, fees, distributions)
- Market commentary tailored to client sophistication level
- Rationale for current positioning and any recommended changes

## Important Notes

- **This output is an adviser working paper. It is not a client-facing document.** The `strategy-request` skill assembles the final SOA Summary Request for paraplanning.
- All tables must follow house style: no bullets in cells, no em dashes, short directive sentences.
- Performance must be calculated net of fees unless client/compliance requires gross.
- Always include appropriate disclaimers and AFSL general advice warning.
- Include franking credits in income summaries. They are a material component of Australian equity returns.
- Reports should be consistent across clients. Use a standard template.
- Match the level of detail to the client. Some want every holding, others want a one-page summary.
- Benchmark selection matters. Use the benchmark from the SOA/IPS, not whatever looks most flattering.
- Report periods should align with the Australian financial year (1 July to 30 June) for YTD/annual figures.
- Review for compliance approval before first distribution of a new template.
- Ensure compliance with AFSL obligations and ASIC Regulatory Guide 175 (licensing) requirements.
