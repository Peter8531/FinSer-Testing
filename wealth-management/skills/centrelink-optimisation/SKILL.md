# Centrelink Optimisation

description: Produce an adviser working paper (paraplanning brief) for modelling Age Pension eligibility and optimising asset structuring to maximise Centrelink entitlements. Covers income test, assets test, deeming rates, gifting rules, and the interaction between super, investments, and pension eligibility. Output goes to paraplanning for formal SOA/ROA drafting. Triggers on "centrelink", "age pension", "means testing", "deeming rates", "pension eligibility", "assets test", or "income test".

## Workflow

### Step 1: Eligibility Check

Confirm basic eligibility:
- **Age**: Must be 67 or older (Age Pension age)
- **Residency**: Australian resident, generally 10+ years of Australian residence (with at least 5 continuous years)
- **Not receiving another pension** that would preclude Age Pension

### Step 2: Asset Inventory

Categorise all assets for the assets test:

**Assessable Assets:**

| Asset | Owner | Value |
|-------|-------|-------|
| Bank accounts / transaction accounts | | |
| Term deposits | | |
| Shares / ETFs / managed funds | | |
| Super in pension phase (account-based pension) | | |
| Investment property (market value less mortgage) | | |
| Business assets | | |
| Motor vehicles, boats, caravans | | |
| Personal effects and household contents | | |
| Funeral bonds (above exempt amount) | | |
| Loans to family/friends | | |
| Other financial investments | | |
| **Total assessable assets** | | |

**Exempt Assets:**
- Principal home (exempt from assets test, but homeowner status affects thresholds)
- Super in **accumulation phase** (exempt until the member reaches Age Pension age, then assessed)
- Funeral bonds up to the exempt amount (~$15,000)
- Special disability trusts (up to the asset value limit)
- Certain complying income streams (legacy pensions)

**Key distinction**: Homeowner vs non-homeowner status significantly affects the assets test thresholds (non-homeowners get higher thresholds).

### Step 3: Assets Test Assessment

**Assets test thresholds (approximate — indexed twice yearly on 20 March and 20 September):**

| Status | Full Pension Threshold | Part Pension Cut-off |
|--------|----------------------|---------------------|
| Single, homeowner | ~$301,750 | ~$674,000 |
| Couple combined, homeowner | ~$451,500 | ~$1,012,500 |
| Single, non-homeowner | ~$543,750 | ~$916,000 |
| Couple combined, non-homeowner | ~$693,500 | ~$1,254,500 |

**Taper rate**: Pension reduces by **$3.00 per fortnight** for every **$1,000** of assets above the full pension threshold.

**Calculate:**

| Item | Amount |
|------|--------|
| Total assessable assets | |
| Less: full pension threshold | |
| Excess assets | |
| Pension reduction (excess × $3 / $1,000 per fortnight) | |
| Maximum pension (fortnightly) | |
| **Estimated pension under assets test** | |

### Step 4: Income Test Assessment

**Deemed income from financial assets:**

| Tier | Threshold (Single) | Threshold (Couple) | Deeming Rate |
|------|--------------------|--------------------|-------------|
| Lower | First ~$60,400 | First ~$100,200 | 0.25% |
| Upper | Balance above | Balance above | 2.25% |

**Financial assets** (subject to deeming): Bank accounts, term deposits, shares, managed funds, super in pension phase, account-based pensions, loans to others.

**Non-financial income** (assessed at actual amount): Employment income, rental income (net of expenses), foreign pensions, business income.

**Calculate deemed income:**

| Item | Amount |
|------|--------|
| Total financial assets | |
| Deemed income on first tier (× 0.25%) | |
| Deemed income on balance (× 2.25%) | |
| **Total deemed income** | |
| Plus: non-financial income | |
| **Total assessable income** | |

**Income test free area**: ~$204/fortnight (single), ~$360/fortnight (couple combined)

**Taper rate**: Pension reduces by **50 cents** for every **$1** of income above the free area.

**Calculate:**

| Item | Amount |
|------|--------|
| Total assessable income (fortnightly) | |
| Less: income free area | |
| Excess income | |
| Pension reduction (excess × 50c) | |
| Maximum pension (fortnightly) | |
| **Estimated pension under income test** | |

### Step 5: Determine Entitlement

The **more restrictive test** applies — whichever produces the lower pension amount:

| Test | Estimated Pension (fortnightly) |
|------|-------------------------------|
| Assets test | |
| Income test | |
| **Pension payable** (lower of the two) | |
| **Annual pension** | |

**Additional benefits** that come with the Pensioner Concession Card (even partial pension):
- Pharmaceutical Benefits Scheme (PBS) concession
- Reduced council rates (varies by council)
- Energy and utility concessions (state-specific)
- Transport concessions
- These can be worth $2,000-$5,000+ per year — even a $1/fortnight pension can be worth claiming

### Step 6: Optimisation Strategies

#### Strategy A: Asset Restructuring

| Strategy | Impact on Assets Test | Impact on Income Test | Net Pension Increase | Considerations |
|----------|---------------------|--------------------|---------------------|---------------|
| Spend on home renovations (reduce assessable assets, home is exempt) | Reduces | Reduces deemed income | | Must be genuine renovation, not just parking money |
| Prepay expenses (rates, insurance, medical) | Reduces | Reduces deemed income | | Temporary — resets each year |
| Purchase a new car / replace household items | Reduces | Reduces deemed income | | Depreciating asset |
| Pay down debt on assessable assets (investment property mortgage) | No change (net value unchanged) | May change | | Reduces debt but also reduces deductible interest |
| Pay down home mortgage | Reduces assessable assets (cash) | Reduces deemed income | | Home remains exempt |

#### Strategy B: Super Structuring

| Strategy | Detail |
|----------|--------|
| Keep super in accumulation phase as long as possible | Super in accumulation is **exempt** from the assets test until Age Pension age. Once Age Pension age is reached, it is assessed regardless of phase |
| Timing of pension phase commencement | If turning 67, consider delaying conversion to pension phase if it would push assets above the cut-off. But weigh against tax-free pension earnings |
| Younger spouse's super | If spouse is under Age Pension age, their super in accumulation is exempt from the assets test — consider retaining funds there |

#### Strategy C: Gifting Considerations

**Centrelink gifting rules** (separate from tax — there is no gift tax in Australia):
- Can gift up to **$10,000 per financial year** and **$30,000 over 5 years** without affecting the means test
- Amounts above these limits are **still assessed** as an asset for **5 years** from the date of the gift (even though the money is gone)
- This is called "deprivation" — designed to prevent gifting assets to qualify for the pension

**Gifting strategy:**
- Plan gifts well in advance of Age Pension age (5+ years ideally)
- Use the annual $10,000 allowance each year
- Do not gift large sums just before applying for the pension — the assets will still be assessed

#### Strategy D: Income Stream Selection

| Income Stream Type | Assets Test | Income Test |
|-------------------|-------------|-------------|
| Account-based pension (started after 1 Jan 2015) | Assessed at account balance | Deemed |
| Account-based pension (started before 1 Jan 2015, grandfathered) | Assessed at account balance | Actual income assessed (may be more favourable) |
| Lifetime/life-expectancy income streams (innovative) | Assessed at 60% of purchase price (or reduces over time) | Deemed on 60% |

### Step 7: Scenario Modelling

| Scenario | Assets (assessable) | Deemed + Other Income | Assets Test Pension | Income Test Pension | Pension Payable | Annual Value |
|----------|--------------------|-----------------------|--------------------|--------------------|----------------|-------------|
| Current structure | | | | | | |
| After home renovation $X | | | | | | |
| After prepaying expenses | | | | | | |
| After gifting strategy (5-year plan) | | | | | | |
| Spouse super in accumulation | | | | | | |

### Step 8: Output — Paraplanning Brief

This output is an **adviser working paper** — it goes to paraplanning, not to the client. See [CONVENTIONS.md](../../CONVENTIONS.md) for the standard format.

**1. Client Facts & Assumptions**
- Client age, residency status, homeowner/non-homeowner classification
- Asset inventory (assessable and exempt) with valuations and ownership
- Income sources (financial and non-financial)

**2. Strategy Analysis & Calculations**
- Means test assessment (income test and assets test calculations)
- Scenario comparison table (current structure vs optimised alternatives)
- Gifting plan modelling (if applicable, with 5-year tracking)

**3. Recommendations Summary**
- Estimated Age Pension entitlement (full, part, or nil)
- Optimisation recommendations with projected pension increase
- Pensioner Concession Card benefits estimate
- Action items and timing

**4. Basis for Advice**
- Rationale for each optimisation strategy (asset restructuring, super structuring, gifting, income stream selection)
- Trade-offs considered (investment returns, flexibility, estate planning impacts)

**5. Paraplanning Notes**
- Thresholds and rates used (confirm current as at advice date)
- Items requiring further verification with Services Australia
- Any assumptions that need client confirmation before SOA/ROA drafting

## Important Notes

- **This output is an adviser working paper for paraplanning — it is not a client-facing document.** Paraplanning drafts the formal SOA/ROA from this brief
- Thresholds and rates are indexed and change on 20 March and 20 September each year — always use current figures
- Deeming rates are set by the government and can change — current rates (0.25% / 2.25%) are historically low
- The Pensioner Concession Card alone can be worth thousands per year — even $1/fortnight of pension is worth claiming
- Super in accumulation phase is exempt from the assets test for the member until they reach Age Pension age — but once they reach 67, it is assessed regardless
- A younger spouse's super in accumulation remains exempt from the couple's assets test until that spouse reaches Age Pension age — this can be a significant planning lever
- Gifting more than allowed limits is still assessed for 5 years — plan ahead
- Centrelink can request a review at any time — ensure all strategies are genuine and documented
- Work Test exemption: from age 67-74, contributions may require meeting the work test (40 hours in 30 consecutive days) unless using the work test exemption (balance <$300,000, first year after ceasing work)
- The adviser and paraplanner ensure the final SOA/ROA meets Best Interest Duty (s961B) and FASEA Code of Ethics
- Refer to Services Australia (Centrelink) for current threshold amounts — rates change regularly
- Consider the whole picture: optimising for Age Pension eligibility may involve trade-offs (lower investment returns, reduced flexibility, estate planning impacts)
