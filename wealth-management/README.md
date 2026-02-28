# Wealth Management Plugin (Australian)

Wealth management tools for Australian financial advisers covering client reviews, financial planning, superannuation strategy, portfolio analysis, and client reporting. Adapted for Australian tax law, superannuation rules, Centrelink means testing, AFSL obligations, and ASIC regulatory requirements.

## Features

- **Client Management** - Review prep, performance reports, investment proposals
- **Financial Planning** - Superannuation strategy, retirement projections, Age Pension modelling, estate planning
- **Portfolio Management** - Rebalancing with CGT discount awareness, capital loss harvesting with Part IVA compliance
- **Australian-Specific** - Franking credit optimisation, Centrelink means testing, super contribution strategy

## Installation

```bash
claude --plugin-dir /path/to/wealth-management
```

Or copy to your project's `.claude-plugin/` directory.

## Commands

| Command | Description |
|---------|-------------|
| `/client-review [client]` | Prep for client review meetings |
| `/client-report [client] [period]` | Generate professional performance reports |
| `/financial-plan [client]` | Build or update comprehensive financial plans |
| `/proposal [prospect]` | Create investment proposals for prospective clients |
| `/rebalance [client]` | Analyse drift and generate rebalancing trades |
| `/tlh [client]` | Identify capital loss harvesting opportunities |
| `/super-strategy [client]` | Optimise superannuation contributions and strategy |
| `/centrelink [client]` | Model Age Pension eligibility and optimise means testing |
| `/franking [client]` | Analyse and optimise franking credit strategy |

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

## Australian Context

This plugin is adapted for Australian financial planning and covers:

- **Superannuation**: Concessional/non-concessional caps, SG, salary sacrifice, TTR, pension phase, transfer balance cap, SMSF, downsizer contributions
- **Tax**: Australian tax brackets, Medicare Levy, CGT discount (50% for individuals), franking credits/dividend imputation, Part IVA anti-avoidance
- **Centrelink**: Age Pension means testing (income test, assets test), deeming rates, gifting rules
- **Regulatory**: AFSL obligations, Best Interest Duty (s961B), SOA/ROA requirements, FASEA Code of Ethics, ASIC oversight
- **Estate Planning**: No estate/gift tax, super death benefits tax, BDBNs, testamentary trusts
- **Insurance**: Life/TPD/IP inside and outside super, APRA reforms, own occupation restrictions

## Example Workflows

### Superannuation Strategy
```
/super-strategy Smith Family

# Reviews:
# - Contribution cap usage and carry-forward availability
# - Salary sacrifice opportunity
# - TTR strategy if approaching preservation age
# - Insurance inside super review
# - Pension phase transition planning
```

### Centrelink Optimisation
```
/centrelink Jones Household

# Calculates:
# - Income test (deeming on financial assets)
# - Assets test (homeowner thresholds)
# - Estimated Age Pension entitlement
# - Optimisation strategies (asset restructuring, gifting plan)
```

### Franking Credit Strategy
```
/franking Smith Family

# Analyses:
# - Franking credits across portfolio
# - Grossed-up vs cash yields
# - After-tax income at client's marginal rate
# - Portfolio tilt recommendations
# - Holding period rule compliance
```

## Configuration

Copy the example config to personalise:

```bash
cp .claude/wealth-management.local.md.example .claude/wealth-management.local.md
```

Edit to include your name, AFSL details, preferred platforms, client list, and default assumptions.
