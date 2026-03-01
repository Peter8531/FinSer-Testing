# Strategic Library

description: Reusable strategy design guidance, operational patterns, and case learnings that apply across all SOA Summary Requests. Contains alternatives doctrine, global prompt rules, common dismissals library, client communication stubs, and governance. This is a reference skill loaded automatically when assembling Strategy Requests. Triggers on "strategic library", "strategy rules", "alternatives doctrine", or "case learnings".

## Alternatives Doctrine

Alternatives must be viable strategy or product options and must include a clear dismissal. Each alternative is a cohesive single-cell entry combining heading, explanation, and dismissal.

Rules:
- The recommended strategy/product is never listed as an alternative.
- Alternatives (Strategies) and Alternative Product Considerations are separate sections.
- Each cell is self-contained. No bullets inside cells. Use sentences.
- Minimum 2-3 alternatives per section.

## Common Strategy Dismissals Library

Adapt per case. Do not use these verbatim without tailoring to client facts.

| Strategy | Typical Viability Reason | Typical Dismissal |
|----------|------------------------|-------------------|
| One-hit contributions (single FY) | Simpler administration, single contribution event | Does not optimise bracket-targeting across FYs; higher tax drag if income pushes into higher band in single year |
| Two-year bracket-targeting | Spreads contributions across FYs to target specific tax bracket | Accepted where cashflow supports and carry-forward is available; dismissed where no carry-forward or time constraint |
| Non-super investing (personal portfolio) | Flexibility, no preservation, no contribution caps | Loses 15% concessional tax advantage at this marginal rate; super is more tax-effective for retirement savings |
| Retain legacy super fund | Continuity of insurance, familiarity | Higher fees, limited investment menu, no SMA access, no integrated reporting |
| Self-managed (SMSF) | Full control, broader investment options | Balance below cost-effective threshold; administrative burden; trustee compliance obligations |
| Full debt paydown before investing | Eliminates interest cost, simplest approach | Opportunity cost over the time horizon; debt recycling converts non-deductible to deductible and builds investment portfolio alongside paydown |
| Direct shares vs ETF/SMA | Potential for stock-specific alpha | Concentration risk, higher transaction costs, no automatic rebalancing |
| TTR pension strategy | Boosts super while maintaining income | Only effective from preservation age; earnings still taxed at 15% until full condition of release |

## Common Product Dismissals Library

| Product/Platform | Typical Viability Reason | Typical Dismissal |
|-----------------|------------------------|-------------------|
| Netwealth Super/Wrap | Competitive admin fees, strong SMA range, good adviser portal | Paraplanning to confirm; listed as recommendation or dismissed based on total cost comparison |
| HUB24 Super/Wrap | Strong platform features, SMA access, reporting | Paraplanning to confirm; listed as recommendation or dismissed based on total cost comparison |
| Akambo SMA | Managed portfolio solution, insurance integration | Primary SMA provider. Listed as recommendation or dismissed based on client needs and portfolio fit |
| Morningstar Wealth | Broad investment menu, managed account capability | Higher total cost at this balance; limited SMA customisation vs Akambo |
| Mason Stevens | Wide investment universe, alternative asset access | Higher minimum, more complex fee structure, less integrated reporting |
| Industry fund (e.g., AustralianSuper, Aware) | Low admin fees, strong default options, insurance pricing | Limited adviser integration, no SMA access, limited portfolio customisation, no wrap reporting |
| Retain legacy fund | Insurance continuity, no rollover paperwork | Higher total cost, limited investment menu, no integrated reporting; retain only if insurance continuity required |

## Operational Patterns (Case Learnings)

These patterns are derived from real engagements. Apply where relevant.

### Bracket-Targeting Contributions
For high-income clients, target deductions that keep contributions primarily in the highest marginal band rather than lumping all in one FY. Model the tax uplift and expiry constraints. Consider carry-forward FIFO and expiry dates.

### Liquidity Policy
Express liquidity as a floor (e.g., $50,000 minimum) and show the contribution funding waterfall: cash on hand, earmarked lump sums, monthly savings. The floor applies after all strategy implementation.

### Partial Rollover for Insurance Continuity
If insurance is under review or referral is pending, specify partial rollover to the new platform with cash left in the legacy fund (e.g., $10,000) to maintain cover until review completes. State the cash amount and its purpose.

### Data Hygiene
Standardise names (beneficiaries). Confirm as-at dates on balances. Require portal screenshots for investment option names and percentages before mapping to SMA.

### Post-SOA Actions
Where an action must occur after SOA acceptance (e.g., sell-down of an existing portfolio, transfer of cash), label it clearly as "Post-SOA action" in the Summary of Advice.

### Surplus Allocation
Where surplus cashflow is directed to a Family Trust for investment, specify the allocation split (e.g., retain 20% in personal offset; 80% loaned to Family Trust). Note: loan documentation handled by client's lawyer with accountant input.

### Risk Profile Mapping
Risk profile is determined per client based on their circumstances, risk tolerance, and investment timeframe. There are no default mappings. Where different entities have different risk profiles, specify the mapping explicitly per client. If risk score does not match selected portfolio, include a short rationale: risk required, timeframe, and ongoing invested through drawdown. Confirm client acceptance.

## Client Communication Stubs

### Request: ATO Carry-Forward and Statements

Hi [Client], could you please upload the following:

1. MyGov > ATO Online > Super > Concessional contributions page screenshot/PDF showing unused cap amounts by year
2. Your current super statement (or a portal screenshot) showing balance, investment option names and exact percentages
3. (If applicable) a summary of current insurance premiums for modelling purposes

Thanks, [Your Name]

### Request: Trust and Entity Documents

Hi [Client], for the advice document we need:

1. Current trust deed (or most recent amendment)
2. Latest trust tax return (for income/distribution history)
3. Confirmation from your accountant on the proposed loan arrangement

Thanks, [Your Name]

## Governance

- This library is a living document. When a case surfaces a repeatable improvement, add a concise rule and note the source in the Change Log.
- When updating rules, ensure alignment across: (1) CONVENTIONS.md, (2) strategy-request skill template, and (3) this strategic library.
- All rules in this library must be harmonised with CONVENTIONS.md.

### Change Log

| | Date | Update |
|---|------|--------|
| 1 | 2026-02-18 | Initial creation from case learnings; added global rules, alternatives doctrine, operational patterns, and email stubs |
| 2 | 2026-03-01 | Adapted from Copilot export into plugin format; integrated with CONVENTIONS.md and strategy-request skill |

## Important Notes

- **This is a reference skill for the adviser and paraplanning team. It is not a client-facing document.**
- Alternatives and product dismissals must be tailored to client facts. Do not use the library entries verbatim without confirming they apply.
- Case learnings are operational patterns, not compliance requirements. The adviser retains judgement on applicability.
- The adviser and paraplanner ensure the final SOA/ROA meets Best Interest Duty (s961B) and FASEA Code of Ethics.
