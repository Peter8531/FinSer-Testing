# Capital Loss Harvesting

description: Produce an adviser working paper (paraplanning brief) for identifying capital loss harvesting opportunities across taxable investment accounts. Finds positions with unrealised losses, suggests replacement securities, and manages Part IVA anti-avoidance compliance. Output goes to paraplanning for formal SOA/ROA drafting. Triggers on "capital loss harvesting", "tax-loss harvesting", "TLH", "harvest losses", "tax losses", "unrealised losses", or "end of financial year tax planning".

## Workflow

### Step 1: Identify Candidates

Scan personal investment accounts and family trust accounts for positions with unrealised losses:

| Security | Asset Class | Cost Base | Current Value | Unrealised Loss | Held >12 Months? | % Loss |
|----------|-----------|-----------|---------------|-----------------|-------------------|--------|
| | | | | | Yes / No | |

**Prioritise by:**
1. Largest absolute loss (biggest tax benefit)
2. Positions held <12 months first (gains on these are not eligible for CGT discount, so losses offset full-rate gains)
3. Positions with the largest % loss (less likely to recover quickly)

**Important — where NOT to harvest:**
- Super in pension phase: earnings are already tax-free, harvesting provides no benefit
- Super in accumulation phase: tax is only 15% (10% on discounted gains) — lower benefit, consider whether transaction costs justify it

### Step 2: Capital Gains Budget

Calculate the client's capital gains tax position for the current **financial year (1 July - 30 June)**:

| Category | Amount |
|----------|--------|
| Realised capital gains YTD (before discount) | |
| Less: CGT discount (50% for assets held >12 months) | |
| Net capital gains (after discount) | |
| Realised capital losses YTD | |
| Carry-forward capital losses from prior years | |
| **Net capital gain / (loss) position** | |
| **Target harvesting amount** | |

**Tax savings calculation:**
- Capital losses first offset **non-discounted gains** (held <12 months), then offset **discounted gains before the discount is applied**
- Losses at the client's marginal tax rate: up to 45% + 2% Medicare levy = 47%
- Capital losses can **ONLY offset capital gains** — they cannot be deducted against salary, dividends, or other ordinary income
- Unused capital losses carry forward indefinitely (but cannot be carried back)
- No $3,000 deduction against ordinary income (that is a US rule)

**CGT discount reminder:**
- Individuals and trusts: 50% discount on gains for assets held >12 months
- Super funds: 33% discount (effectively taxed at 10% instead of 15%)
- Companies: no CGT discount

### Step 3: Replacement Securities

For each harvest candidate, suggest a replacement that:
- Maintains similar market exposure (same asset class, sector, geography)
- Has similar risk/return characteristics
- Minimises tracking error during the holding period

| Sell | Replace With | Reason | Tracking Error Risk |
|------|-------------|--------|-------------------|
| Vanguard Australian Shares (VAS) | iShares Core S&P/ASX 200 (IOZ) | Similar AU equity exposure, different index construction | Minimal |
| Vanguard International Shares (VGS) | iShares Core MSCI World (IWLD) | Similar global equity exposure | Low |
| BHP Group (BHP) | Rio Tinto (RIO) or Fortescue (FMG) | Same resources sector, different company | Moderate |
| Vanguard Aus Fixed Interest (VAF) | iShares Core Composite Bond (IAF) | Similar AU bond exposure | Minimal |

**Note on wash sales:** Australia does **not** have a US-style wash sale rule. There is no 30-day buyback restriction, and there is no "substantially identical" security test. You can technically sell and immediately repurchase the same security. **However** — see Step 4.

### Step 4: Part IVA Anti-Avoidance Check

Before executing, assess **Part IVA** (Income Tax Assessment Act 1936) compliance:

The ATO can deny a tax benefit if a scheme's **dominant purpose** is to obtain a tax benefit. When harvesting losses, ensure:

- There is a **genuine investment reason** for the trade beyond the tax benefit (e.g., rebalancing, switching to a lower-cost fund, improving diversification, changing risk profile)
- The replacement security represents a **genuine change** in the investment position
- Document the non-tax reasons for each trade
- Selling and immediately repurchasing the **exact same security** purely for a tax loss is the highest-risk scenario under Part IVA

**Risk assessment for each trade:**

| Security Sold | Replacement | Non-Tax Rationale | Part IVA Risk |
|--------------|-------------|-------------------|---------------|
| | | e.g., "Lower MER", "Better diversification" | Low / Medium / High |

**Practical guidance:**
- Switching between different ETF providers tracking different indices = **low risk** (genuine change in investment)
- Selling an individual stock and buying a sector ETF = **low risk** (improved diversification)
- Selling and buying back the same security after a short period with no other rationale = **high risk**
- Harvesting losses as part of a broader portfolio rebalance = **low risk** (investment rationale exists independently)

### Step 5: Franking Credit Considerations

Before selling Australian equities, check:
- Is the stock about to go ex-dividend? Selling before ex-dividend date forfeits the franking credits
- Has the client held the shares for at least 45 days around ex-dividend (holding period rule for franking credit eligibility)?
- For clients in pension phase or low tax brackets, franking credit refunds may be more valuable than the capital loss

### Step 6: Execution Plan

| Trade # | Account | Action | Security | Units | Est. Proceeds | Est. Loss | Replacement | Non-Tax Rationale |
|---------|---------|--------|----------|-------|--------------|-----------|-------------|-------------------|
| | | Sell | | | | | | |
| | | Buy | | | | | | |

**Summary:**
- Total estimated losses harvested: $
- Estimated tax savings: $ (at marginal rate of %)
- Net portfolio impact: minimal (replacement securities maintain exposure)
- Franking credits at risk: $ (if any sales near ex-dividend)
- Part IVA risk assessment: Low / Medium

### Step 7: Post-Harvest Actions

- Update cost base records for replacement securities (new, lower cost base — future gains will be larger)
- Document rationale for each trade (retain for ATO audit purposes)
- Consider timing of any switch back to original securities — no mandatory waiting period, but a very quick switch-back strengthens a Part IVA argument
- Update CGT schedule for the tax return
- Advise accountant/tax agent of harvested losses for inclusion in the tax return

### Step 8: Output — SOA Summary Request Input

This skill produces the **analytical working papers** that feed into the SOA Summary Request (assembled by the `strategy-request` skill). See [CONVENTIONS.md](../../CONVENTIONS.md) for house style rules.

**Feeds into Summary of Advice:**
- Recommended trades with replacement securities
- Updated portfolio allocation (before/after)
- Net tax savings summary
- Each item as a short, directive sentence

**Feeds into Projection Parameters:**
- Harvest opportunity list with prioritisation
- Tax savings estimate at client's marginal rate
- Capital gains budget (realised gains YTD, carry-forward losses)
- Source-of-Truth table for each input (document name, date, section)

**Feeds into Alternatives:**
- Strategies considered and dismissed with rationale (e.g., alternative replacement securities, different harvest timing, partial vs full position sales)
- Trade-offs considered (cost base step-down, transaction costs, tracking error)

**Feeds into Notes to AA or Paraplanning:**
- Gap items to request from client
- Part IVA compliance documentation for each trade
- CGT schedule updates required for tax return
- Items needing client or accountant confirmation

**Calculation Workings (appendix):**
- Part IVA risk assessment for each trade
- Franking credit impact analysis (if selling Australian equities)
- Non-tax investment rationale for each trade (rebalancing, cost reduction, diversification improvement)
- Client tax position (marginal rate, account types) and current portfolio holdings with unrealised gains/losses

## Important Notes

- **This output is an adviser working paper. It is not a client-facing document.** The `strategy-request` skill assembles the final SOA Summary Request for paraplanning.
- All tables must follow house style: no bullets in cells, no em dashes, short directive sentences.
- Capital losses can ONLY offset capital gains. They cannot reduce ordinary income (salary, interest, dividends).
- There is no wash sale rule in Australia, but Part IVA anti-avoidance provisions can deny tax benefits for schemes with a dominant tax purpose.
- Always document a genuine, non-tax investment rationale for each trade.
- Consider the long-term cost base step-down. Harvesting resets cost base, meaning larger gains when eventually sold.
- **End of financial year (30 June)** is prime harvesting season, not 31 December.
- Harvesting in super pension phase provides no tax benefit. Earnings are already tax-free.
- Harvesting in super accumulation saves tax at only 15% (or 10% on discounted gains). Ensure transaction costs justify it.
- Check franking credit entitlements before selling Australian equities (45-day holding period rule).
- Capital losses cannot offset franking credit refunds.
- Not all losses are worth harvesting. Brokerage costs, bid-ask spreads, and tracking error have real costs.
- Keep detailed records for the CGT schedule in the tax return.
- The adviser and paraplanner ensure the final SOA/ROA meets Best Interest Duty (s961B) and FASEA Code of Ethics.
