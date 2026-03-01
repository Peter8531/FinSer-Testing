# Wealth Management Plugin (Australian)

Adviser working paper and paraplanning brief generator for Australian wealth management. Produces strategy analysis, calculations with full workings, and recommendation summaries that go to **paraplanning** for formal SOA/ROA documentation.

**This plugin does not produce client-facing advice.** It produces internal adviser working papers — the analysis, calculations, and rationale that form the basis for paraplanning to draft compliant documentation. See [CONVENTIONS.md](CONVENTIONS.md) for the output format.

Adapted for Australian tax law, superannuation rules, Centrelink means testing, AFSL obligations, and ASIC regulatory requirements.

## Features

- **Client Management** - Review prep, performance reports, investment proposals
- **Financial Planning** - Superannuation strategy, retirement projections, Age Pension modelling, estate planning
- **Portfolio Management** - Rebalancing with CGT discount awareness, capital loss harvesting with Part IVA compliance
- **Wealth Building** - Debt recycling (non-deductible to deductible mortgage conversion)
- **Australian-Specific** - Franking credit optimisation, Centrelink means testing, super contribution strategy

## Installation

```bash
claude --plugin-dir /path/to/wealth-management
```

Or copy to your project's `.claude-plugin/` directory.

## Commands

Each command produces a **paraplanning brief** — an adviser working paper with full calculation workings.

| Command | Paraplanning Brief For |
|---------|----------------------|
| `/client-review [client]` | Client review meeting — performance, allocation, talking points |
| `/client-report [client] [period]` | Performance report — returns, income, franking summaries |
| `/financial-plan [client]` | Financial plan — super, retirement, Age Pension, debt recycling, estate |
| `/proposal [prospect]` | Investment proposal — prospect analysis, strategy rationale |
| `/rebalance [client]` | Portfolio rebalancing — drift analysis, tax-aware trades |
| `/tlh [client]` | Capital loss harvesting — harvestable losses, Part IVA rationale |
| `/super-strategy [client]` | Superannuation strategy — contributions, TTR, pension, TBC |
| `/centrelink [client]` | Centrelink optimisation — means testing, asset structuring |
| `/franking [client]` | Franking credit strategy — grossed-up yields, holding periods |
| `/debt-recycling [client]` | Debt recycling — loan structure, projections, cost of carry |

## Skills

### Client Management
| Skill | Description |
|-------|-------------|
| **client-review** | Meeting prep with performance, allocation, talking points |
| **client-report** | Quarterly/annual reports with franking credit summaries |
| **investment-proposal** | Prospect proposals with AFSL details and ASX vehicles |

### Financial Planning
| Skill | Description |
|-------|-------------|
| **financial-plan** | Super strategy, retirement projections, Age Pension modelling, estate planning |
| **super-strategy** | Contribution optimisation, TTR, pension phase, transfer balance cap, SMSF |
| **centrelink-optimisation** | Income test, assets test, deeming rates, gifting rules |

### Portfolio Management
| Skill | Description |
|-------|-------------|
| **portfolio-rebalance** | Drift analysis with CGT discount and franking credit awareness |
| **tax-loss-harvesting** | Capital loss harvesting with Part IVA anti-avoidance compliance |
| **franking-strategy** | Dividend imputation optimisation, grossed-up yields, holding period rules |

### Wealth Building
| Skill | Description |
|-------|-------------|
| **debt-recycling** | Convert non-deductible mortgage to deductible investment debt, year-by-year projections, franking integration, exit strategies |

## Australian Context

This plugin is adapted for Australian financial planning and covers:

- **Superannuation**: Concessional/non-concessional caps, SG, salary sacrifice, TTR, pension phase, transfer balance cap, SMSF, downsizer contributions
- **Debt Recycling**: Non-deductible to deductible mortgage conversion, loan structuring, franking credit integration, exit strategies
- **Tax**: Australian tax brackets, Medicare Levy, CGT discount (50% for individuals), franking credits/dividend imputation, Part IVA anti-avoidance
- **Centrelink**: Age Pension means testing (income test, assets test), deeming rates, gifting rules
- **Regulatory**: AFSL obligations, Best Interest Duty (s961B), SOA/ROA requirements, FASEA Code of Ethics, ASIC oversight
- **Estate Planning**: No estate/gift tax, super death benefits tax, BDBNs, testamentary trusts
- **Insurance**: Life/TPD/IP inside and outside super, APRA reforms, own occupation restrictions

## Example Workflows

Each example produces an adviser working paper that goes to paraplanning — not a client-facing document.

### Financial Plan (with debt recycling)
```
/financial-plan Smith Family

# Produces paraplanning brief with:
# - Cash flow projections (FY-aligned, full workings)
# - Super contribution modelling (SG + salary sacrifice + NCC)
# - Retirement projection with Age Pension means testing
# - Debt recycling assessment (if mortgage exists)
# - Scenario comparison table
# - Basis for advice (calculations supporting each recommendation)
# - Paraplanning notes (product research, disclosures, gaps to resolve)
```

### Debt Recycling
```
/debt-recycling Smith Family

# Produces paraplanning brief with:
# - Suitability assessment
# - Loan restructure specification (Split A / Split B)
# - Year-by-year debt composition shift (every row calculable)
# - After-tax cost of carry analysis (full workings)
# - Franking credit integration at client's marginal rate
# - Stress test results (rate rise, market crash, job loss)
# - Exit strategy options with CGT modelling
# - Basis for advice (legislative refs: TR 2000/2, s8-1 ITAA 1997)
```

### Superannuation Strategy
```
/super-strategy Smith Family

# Produces paraplanning brief with:
# - Contribution cap analysis and carry-forward availability
# - Salary sacrifice modelling (tax saving workings)
# - TTR strategy if approaching preservation age
# - Pension phase transition and TBC tracking
# - Insurance inside super review
```

### Centrelink Optimisation
```
/centrelink Jones Household

# Produces paraplanning brief with:
# - Income test calculation (deeming on financial assets)
# - Assets test calculation (homeowner thresholds)
# - Estimated Age Pension entitlement (full workings)
# - Optimisation strategies with quantified pension increase
```

## Configuration

Copy the example config to personalise:

```bash
cp .claude/wealth-management.local.md.example .claude/wealth-management.local.md
```

Edit to include your name, AFSL details, preferred platforms, client list, and default assumptions.
