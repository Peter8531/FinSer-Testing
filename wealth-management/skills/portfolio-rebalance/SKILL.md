# Portfolio Rebalance

description: Analyse portfolio allocation drift and generate rebalancing trade recommendations across accounts. Considers CGT discount, franking credits, super fund tax rules, and Part IVA anti-avoidance provisions. Triggers on "rebalance", "portfolio drift", "allocation check", "rebalancing trades", or "my portfolio is out of balance".

## Workflow

### Step 1: Current State

For each account, capture:
- **Account type**: Personal (individual/joint), super (accumulation), super (pension phase), SMSF, family trust, company
- **Holdings** with current market value
- **Cost base** (for personal and trust accounts — CGT applies)
- **Unrealised gains/losses per position** and whether held >12 months (CGT discount eligibility)
- **Franking credits** attached to Australian equity holdings

### Step 2: Drift Analysis

Compare current allocation to target (from Investment Policy Statement or Statement of Advice):

| Asset Class | Target % | Current % | Drift | $ Over/Under |
|------------|----------|-----------|-------|-------------|
| Australian Equities (ASX 200) | | | | |
| Australian Small/Mid Cap | | | | |
| International Developed | | | | |
| Emerging Markets | | | | |
| Australian Fixed Income | | | | |
| International Fixed Income | | | | |
| Australian Property (A-REITs / direct) | | | | |
| Alternatives | | | | |
| Cash / Term Deposits | | | | |

Flag positions exceeding the rebalancing band (typically ±3-5%).

### Step 3: Trade Recommendations

Generate trades to bring allocation back to target.

**Tax-Aware Rebalancing Rules (Australian context):**

1. **Prefer rebalancing inside super first:**
   - Pension phase: trades are **tax-free** — no CGT consequences at all
   - Accumulation phase: CGT at 15% (10% with CGT discount for assets held >12 months) — much lower than personal marginal rates

2. **In personal/trust accounts:**
   - **Prefer selling positions held >12 months** — 50% CGT discount means only half the gain is assessable (individuals and trusts)
   - **Harvest losses** while rebalancing where possible (offset gains with losses before triggering new gains)
   - Avoid selling positions held <12 months with large unrealised gains (full gain assessable at marginal rates, no discount)
   - Consider directing new contributions/savings to underweight asset classes instead of selling

3. **Franking credit considerations:**
   - Avoid selling Australian equities just before ex-dividend dates (forfeits franking credits)
   - For clients in low/nil tax brackets (especially pension phase), franking credit refunds may outweigh rebalancing benefits
   - Check 45-day holding period rule for franking credit eligibility

4. **Part IVA awareness:**
   - Australia has no wash sale rule — you can sell and repurchase immediately
   - However, if rebalancing trades are structured primarily to generate tax losses rather than for genuine portfolio management, Part IVA anti-avoidance may apply
   - Document the investment rationale for each trade

**Trade List:**

| Account | Type | Action | Security | Units/$ | Reason | Tax Impact |
|---------|------|--------|----------|---------|--------|-----------|
| | Super (pension) | Buy/Sell | | | Rebalance | Tax-free |
| | Super (accum) | Buy/Sell | | | Rebalance | 15% / 10% |
| | Personal | Buy/Sell | | | Rebalance / Harvest | Marginal rate / CGT discount |

### Step 4: Asset Location Review

Optimise which assets are held in which account types:

- **Super (pension phase)**: Highest-growth assets (tax-free earnings — maximise the benefit of zero tax). Australian equities with high franking credits (refunded in full)
- **Super (accumulation)**: Growth assets benefit from 15% tax cap. Bonds and income-generating assets benefit from lower tax rate vs personal marginal rates
- **Personal accounts**: Tax-efficient investments — Australian equities (franking credits reduce effective tax), broad index ETFs (low turnover = fewer CGT events), assets you may want to access before preservation age
- **Family trust**: Income-producing assets that can be distributed to lower-income beneficiaries. Consider streaming franking credits and capital gains to appropriate beneficiaries
- **Company**: Generally avoid holding growth assets in company structures (no CGT discount, 25-30% flat rate, trapped profits)

### Step 5: Implementation

- Total trades by account
- Estimated brokerage costs
- Estimated tax impact:
  - Capital gains triggered (discounted vs non-discounted)
  - Capital losses harvested
  - Net CGT position
  - Franking credits at risk (if selling near ex-dividend)
- Net effect on allocation drift (before vs after)

### Step 6: Output

- Drift analysis table
- Recommended trade list (Excel)
- Tax impact summary (CGT, franking credits)
- Before/after allocation comparison
- Asset location recommendations

## Important Notes

- Don't rebalance for rebalancing's sake — small drift within bands is fine
- Tax costs can outweigh rebalancing benefits in personal accounts — calculate the breakeven, especially for positions with large unrealised gains without CGT discount eligibility
- Consider pending cash flows (super contributions, pension drawdowns, salary sacrifice, dividends) before trading
- Check for any client-specific restrictions (ESG preferences, concentrated stock, platform restrictions)
- Document rationale for every trade for compliance records and SOA/ROA requirements
- No wash sale rule in Australia, but Part IVA anti-avoidance applies to schemes with a dominant tax purpose
- Minimum pension drawdown requirements may create natural rebalancing opportunities (sell overweight assets to fund drawdowns)
- Super contribution caps reset each 1 July — consider timing of contributions to underweight asset classes
- Rebalancing across super and personal accounts requires coordinating with the client's overall tax position
