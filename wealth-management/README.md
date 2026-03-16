# Wealth Management Plugin (Australian)

SOA Summary Request generator for Australian wealth management. Produces strategy analysis with full calculation workings, then assembles CRM-ready **Strategy Requests** for associates and paraplanning to draft formal SOA/ROA documentation.

**This plugin does not produce client-facing advice.** It produces adviser working papers: the analysis, calculations, and rationale that feed into your SOA Summary Request template. See [CONVENTIONS.md](CONVENTIONS.md) for house style rules and output format.

Adapted for Australian tax law, superannuation rules, Centrelink means testing, AFSL obligations, and ASIC regulatory requirements.

## Features

- **Strategy Request Assembly** - SOA Summary Request output in standard template format, CRM-ready
- **Strategic Library** - Alternatives doctrine, common dismissals, operational patterns, case learnings
- **Financial Planning** - Superannuation strategy, retirement projections, Age Pension modelling, estate planning
- **Wealth Building** - Debt recycling (non-deductible to deductible mortgage conversion)
- **Portfolio Management** - Rebalancing with CGT discount awareness, capital loss harvesting with Part IVA compliance
- **Client Management** - Review prep, performance reports, investment proposals

## Installation

```bash
claude --plugin-dir /path/to/wealth-management
```

Or copy to your project's `.claude-plugin/` directory.

## Commands

Analytical commands produce working papers. The `/strategy-request` command assembles them into the final SOA Summary Request.

| Command | Output |
|---------|--------|
| `/strategy-request [client]` | **SOA Summary Request** (full template: Entities, Summary, Alternatives, Products, Projections, TMD, Notes) |
| `/financial-plan [client]` | Financial plan analysis (super, retirement, Age Pension, debt recycling, estate) |
| `/debt-recycling [client]` | Debt recycling analysis (loan structure, projections, cost of carry) |
| `/super-strategy [client]` | Super strategy analysis (contributions, TTR, pension, TBC) |
| `/centrelink [client]` | Centrelink analysis (means testing, asset structuring) |
| `/franking [client]` | Franking credit analysis (grossed-up yields, holding periods) |
| `/rebalance [client]` | Portfolio rebalancing analysis (drift, tax-aware trades) |
| `/tlh [client]` | Capital loss harvesting analysis (harvestable losses, Part IVA) |
| `/client-review [client]` | Client review meeting prep (performance, allocation, talking points) |
| `/client-report [client] [period]` | Performance report data (returns, income, franking summaries) |
| `/proposal [prospect]` | Investment proposal analysis (prospect analysis, strategy rationale) |

## Skills

### Strategy Assembly
| Skill | Description |
|-------|-------------|
| **strategy-request** | Assembles the final SOA Summary Request from analytical working papers |
| **strategic-library** | Reusable guidance: alternatives doctrine, common dismissals, operational patterns |

### Financial Planning
| Skill | Description |
|-------|-------------|
| **financial-plan** | Super strategy, retirement projections, Age Pension modelling, estate planning |
| **super-strategy** | Contribution optimisation, TTR, pension phase, transfer balance cap, SMSF |
| **centrelink-optimisation** | Income test, assets test, deeming rates, gifting rules |
| **debt-recycling** | Non-deductible to deductible mortgage conversion, year-by-year projections, franking integration |

### Portfolio Management
| Skill | Description |
|-------|-------------|
| **portfolio-rebalance** | Drift analysis with CGT discount and franking credit awareness |
| **tax-loss-harvesting** | Capital loss harvesting with Part IVA anti-avoidance compliance |
| **franking-strategy** | Dividend imputation optimisation, grossed-up yields, holding period rules |

### Client Management
| Skill | Description |
|-------|-------------|
| **client-review** | Meeting prep with performance, allocation, talking points |
| **client-report** | Quarterly/annual reports with franking credit summaries |
| **investment-proposal** | Prospect proposals with AFSL details and ASX vehicles |

## Workflow

The typical workflow is:

1. **Analyse**: Run one or more analytical commands (`/financial-plan`, `/debt-recycling`, `/super-strategy`, etc.) to model strategies and produce calculation workings
2. **Assemble**: Run `/strategy-request` to assemble the analysis into the SOA Summary Request template (Entities, Summary of Advice, Alternatives, Product Considerations, Projection Parameters, TMD, Notes)
3. **Send**: Paste the SOA Summary Request into CRM for paraplanning

The analytical skills produce the working papers. The strategy-request skill assembles them into the final CRM-ready output.

## Example Workflows

### Full Strategy Request (new client)
```
/financial-plan Client A
# Run analysis first, then:

/strategy-request Client A
# Assembles into SOA Summary Request with all mandatory sections
# Output is CRM-ready tables
```

### Debt Recycling Strategy Request
```
/debt-recycling Client A
# Produces: suitability assessment, loan restructure spec,
# year-by-year projections, cost of carry analysis,
# stress tests, exit strategy options

/strategy-request Client A
# Assembles debt recycling actions into Summary of Advice,
# dismissed alternatives, projection parameters, notes
```

### Super Contribution Strategy
```
/super-strategy Client A
# Produces: carry-forward analysis, bracket-targeting model,
# salary sacrifice calculations, contribution timing

/strategy-request Client A
# Assembles into SOA Summary Request format
```

## Configuration

Copy the example config to personalise:

```bash
cp .claude/wealth-management.local.md.example .claude/wealth-management.local.md
```

Edit to include your name, AFSL details, preferred platforms, partners (Akambo is part of the group; external referrals for estate planning, accounting, mortgage broking), strategy request preferences (liquidity floor, surplus allocation, risk mapping), and default assumptions.

## Key Files

| File | Purpose |
|------|---------|
| `CONVENTIONS.md` | House style rules, SOA Summary Request format, global rules, calculation standards |
| `skills/strategy-request/SKILL.md` | SOA Summary Request assembly process and template |
| `skills/strategic-library/SKILL.md` | Reusable guidance, alternatives doctrine, case learnings |
| `.claude/wealth-management.local.md` | Your personal preferences (gitignored) |
