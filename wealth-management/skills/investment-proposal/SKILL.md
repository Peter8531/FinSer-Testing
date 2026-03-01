# Investment Proposal

description: Produce an adviser working paper (paraplanning brief) for investment proposals for prospective clients. Covers the firm's approach, proposed allocation, expected outcomes, fee structure, and regulatory requirements. Use when pitching new clients or presenting a new investment strategy. Output goes to paraplanning for formal SOA/ROA drafting. Triggers on "investment proposal", "prospect presentation", "pitch new client", "proposal for [client]", or "new client presentation".

## Workflow

### Step 1: Prospect Context

Gather:
- **Prospect name** and household details
- **Current situation**: Existing financial adviser? Self-directed? What prompted the meeting?
- **Assets**: Estimated total wealth, account types (personal, super funds, SMSF, property, trust), current holdings (if shared)
- **Super details**: Fund name(s), balance(s), insurance inside super, investment options
- **Goals**: Retirement, wealth preservation, growth, income, education, estate, aged care
- **Risk profile**: Conservative, moderate, balanced, growth, high growth (or risk profiling questionnaire score)
- **Constraints**: Ethical/ESG preferences, concentrated stock positions, illiquidity needs, Centrelink considerations
- **Fee sensitivity**: What are they paying now? Platform fees, adviser fees, fund MERs?
- **Competition**: Who else are they considering? Industry super fund? Another adviser? Self-directed?

### Step 2: Proposal Structure

**I. About Our Practice** (1 page)
- Practice overview, AFSL details (or authorised representative of which licensee)
- Investment philosophy (in plain English)
- Team bios (relevant to this client)
- Client service model — how often do we meet, how do they contact us
- Professional qualifications (CFP, relevant degree, FASEA compliance)
- AFCA membership details

**II. Understanding Your Needs** (1 page)
- Restate their goals and concerns — show you listened
- Key planning considerations identified in discovery
- What success looks like for them
- Relevant life stage considerations (accumulation, pre-retirement, retirement)

**III. Proposed Investment Strategy** (2-3 pages)
- Recommended asset allocation with rationale
- How allocation maps to their goals and risk profile
- Investment vehicles: ASX-listed ETFs, LICs, managed funds (on platform), direct Australian equities, A-REITs, term deposits
- Super strategy: recommended fund/platform, investment option, contribution strategy
- Tax-aware approach: franking credit optimisation, CGT discount timing, asset location between super and personal

Proposed allocation:

| Asset Class | Allocation | Vehicle | Rationale |
|------------|-----------|---------|-----------|
| Australian Equities | | e.g., VAS, IOZ, direct | |
| International Equities | | e.g., VGS, IWLD, IVV | |
| Australian Fixed Income | | e.g., VAF, IAF | |
| Property (A-REITs) | | e.g., VAP, direct | |
| Cash / Term Deposits | | | |

**IV. Expected Outcomes** (1-2 pages)
- Projected growth scenarios (conservative, moderate, optimistic)
- Monte Carlo probability of meeting goals
- Retirement income projections (super pension + Age Pension if eligible)
- Risk metrics (max drawdown, volatility)
- Comparison to current portfolio/super fund (if known)
- Franking credit income projections (for income-focused clients)

**V. Fee Structure** (1 page)
- Advisory fee: fixed fee, percentage-based, or hybrid (tiered if applicable)
- Platform/administration fees
- Underlying fund MERs (Management Expense Ratios)
- Total all-in cost estimate ($ and %)
- How fees compare to industry averages and their current arrangement
- Value proposition — what they get for the fee
- Ongoing Fee Arrangement (OFA) — annual renewal requirement and client's right to opt out
- Fee Disclosure Statement (FDS) will be provided annually

**VI. Getting Started** (1 page)
- Statement of Advice (SOA) — explain that a full SOA will be prepared before implementation
- Account opening / platform onboarding process
- Super rollover process and timeline (if consolidating funds)
- Transition plan (if moving from another adviser — including authority to proceed forms)
- Insurance review timeline (inside and outside super)
- First 90 days — what to expect
- Required documents: ID (100-point check), super fund details, tax file number, existing statements

### Step 3: Customisation

- Match the tone to the prospect (corporate executive vs small business owner vs retiree)
- If they have a concentrated stock position, address it directly (CGT discount, staged sell-down, protective strategies)
- If they're comparing you to an industry super fund, emphasise personal advice, holistic planning, and accountability
- If they're price-sensitive, lead with total value and outcomes, not just fees — emphasise the cost of not getting advice (missed super strategies, tax inefficiency, insurance gaps)
- For retirees, lead with income security, Age Pension optimisation, and estate planning
- For business owners, address business succession, super catch-up contributions, and trust structures

### Step 4: Output — SOA Summary Request Input

This skill produces the **analytical working papers** that feed into the SOA Summary Request (assembled by the `strategy-request` skill). See [CONVENTIONS.md](../../CONVENTIONS.md) for house style rules.

**Feeds into Summary of Advice:**
- Recommended investment strategy mapped to goals and risk profile
- Super strategy (fund/platform, investment option, contribution strategy)
- Tax-aware approach (franking credits, CGT discount timing, asset location)
- Fee structure: advisory fees, platform fees, fund MERs, total all-in cost
- Each item as a short, directive sentence

**Feeds into Projection Parameters:**
- Proposed asset allocation with vehicle selection and rationale
- Projected growth scenarios (conservative, moderate, optimistic)
- Monte Carlo probability of meeting goals
- Retirement income projections (super pension + Age Pension if eligible)
- Risk metrics (max drawdown, volatility)
- Source-of-Truth table for each input (document name, date, section)

**Feeds into Alternatives:**
- Strategies considered and dismissed with rationale (e.g., industry super, self-directed, other advisers)
- Comparison to current portfolio/super fund (if known)

**Feeds into Product Considerations:**
- Platform and vehicle selection rationale (ETFs, LICs, managed funds, direct equities)
- Products or platforms dismissed with reasoning

**Feeds into Notes to AA or Paraplanning:**
- Gap items to request from prospect
- Risk profile confirmation
- Getting started plan: SOA process, account opening, super rollover, transition plan, first 90 days
- Flag any areas requiring compliance review before presenting to prospect

**Calculation Workings (appendix):**
- Franking credit income projections (for income-focused clients)
- Fee comparison (current arrangement vs proposed)
- How the proposed strategy addresses the prospect's specific goals and concerns
- Legislative references supporting each recommendation

## Important Notes

- **This output is an adviser working paper. It is not a client-facing document.** The `strategy-request` skill assembles the final SOA Summary Request for paraplanning.
- All tables must follow house style: no bullets in cells, no em dashes, short directive sentences.
- The proposal should feel personalised, not templated. Reference their specific situation.
- Do not oversell performance. Set realistic expectations and emphasise process and planning value.
- Always include disclaimers (projections are hypothetical, past performance does not indicate future performance).
- Include AFSL general advice warning on all materials.
- The transition plan matters. Clients fear the disruption of switching advisers or rolling over super.
- A full Statement of Advice (SOA) is required before implementing any recommendations. The proposal is not a substitute.
- Follow up within 48 hours with the proposal and a clear next step.
- Compliance must review before presenting to prospects.
- Best Interest Duty (s961B) applies from the moment personal advice is provided.
- Record all interactions in the client file for AFSL compliance.
- 14-day cooling-off period applies to most financial products. Inform the client.
