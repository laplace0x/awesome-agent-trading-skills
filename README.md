# Awesome Agent Trading Skills [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of trading skills, plugins, and integrations for AI agent platforms (OpenClaw, ElizaOS, etc.).

AI agents are trading crypto, stocks, options, and prediction markets — but finding reliable, safe trading skills is hard. This list catalogs every trading-related agent skill we can find, with quality notes and risk assessments.

**Focus: installable skills/plugins that let agents actually trade.** Not frameworks, not bots, not APIs — the skill layer on top.

Contributions welcome! Read [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## Contents

- [OpenClaw Skills](#openclaw-skills)
  - [Hyperliquid](#hyperliquid)
  - [Binance](#binance)
  - [Bybit & OKX](#bybit--okx)
  - [Coinbase](#coinbase)
  - [Prediction Markets](#prediction-markets)
  - [DeFi & On-Chain](#defi--on-chain)
  - [Market Data & Analysis](#market-data--analysis)
  - [Risk Management](#risk-management--1)
  - [Multi-Exchange](#multi-exchange)
- [ElizaOS Plugins](#elizaos-plugins)
- [Other Agent Platforms](#other-agent-platforms)
- [Skill Registries](#skill-registries)
- [Safety & Auditing](#safety--auditing)

---

## OpenClaw Skills

### Hyperliquid

Skills for trading on Hyperliquid DEX (perpetuals, spot, vaults).

| Skill | Author | Description | Install |
|-------|--------|-------------|---------|
| [Hyperclaw](https://github.com/openclaw/skills/tree/main/hyperclaw) | OpenClaw Official | Market data: funding rates, OI, order book, candles, market scanner | `openclaw skills add openclaw/hyperclaw` |
| [Hyperliquid Trading](https://clawhub.ai/laplace0x/hyperliquid-trading) | Agent Laplace | Secure perps trading via gateway API with enforced risk rules (max 5x leverage, mandatory SL, circuit breaker) | `openclaw skills add laplace0x/hyperliquid-trading` |
| [Smart Trading](https://openclawai.me/trading) | OpenClaw AI | Sub-second Hyperliquid execution with hardcoded risk guardrails (2% max position) | See website |

### Binance

Skills for Binance spot and futures trading.

| Skill | Author | Description | Install |
|-------|--------|-------------|---------|
| [Binance](https://github.com/openclaw/skills/tree/main/binance) | OpenClaw Official | Spot & futures trading with safety checks | `openclaw skills add openclaw/binance` |
| [Quant Trader](https://clawhub.ai/zhenstaff/quant-trader) | zhenstaff | Quantitative trading with backtesting via CCXT/Binance | `openclaw skills add zhenstaff/quant-trader` |

### Bybit & OKX

| Skill | Author | Description | Install |
|-------|--------|-------------|---------|
| [CryptoSkill](https://cryptoskill.org) | CryptoSkill | Unified hub: Binance, OKX, Bybit, and DEX support | See website |

### Coinbase

| Skill | Author | Description | Install |
|-------|--------|-------------|---------|
| [Public](https://public.com/api/docs/templates/openclaw-agent-skill) | Public.com | Stocks, ETFs, options, crypto — commission-free | See website |

### Prediction Markets

| Skill | Author | Description | Install |
|-------|--------|-------------|---------|
| [Polyclaw](https://github.com/BankrBot/skills/tree/main/polyclaw) | Chainstack | Polymarket trading with strategy backtesting | `openclaw skills add BankrBot/polyclaw` |
| [Polymarket Paper Trader](https://clawhub.ai/robotlearning123/polymarket-paper-trader) | robotlearning123 | Paper trading on Polymarket with portfolio tracking | `openclaw skills add robotlearning123/polymarket-paper-trader` |

### DeFi & On-Chain

| Skill | Author | Description | Install |
|-------|--------|-------------|---------|
| [Bankr](https://github.com/BankrBot/skills/tree/main/bankr) | BankrBot | Full DeFi suite: spot, leverage (50x via Avantis), NFTs, 5 chains | `openclaw skills add BankrBot/bankr` |
| [Trails](https://github.com/BankrBot/skills/tree/main/trails) | Polygon | Cross-chain swap, bridge, and DeFi orchestration via Sequence | `openclaw skills add BankrBot/trails` |
| [Hydrex](https://github.com/BankrBot/skills/tree/main/hydrex) | Hydrex | Liquidity pools on Base with auto-managed vaults | `openclaw skills add BankrBot/hydrex` |

### Market Data & Analysis

| Skill | Author | Description | Install |
|-------|--------|-------------|---------|
| [Signals](https://github.com/BankrBot/skills/tree/main/signals) | Axiom | Transaction-verified trading signals on Base with TX hash proof | `openclaw skills add BankrBot/signals` |
| [Quicknode](https://github.com/BankrBot/skills/tree/main/quicknode) | Quicknode | Blockchain RPC, token balances, gas estimation, tx status | `openclaw skills add BankrBot/quicknode` |
| [Alchemy](https://github.com/BankrBot/skills/tree/main/alchemy) | Alchemy | EVM JSON-RPC, token balances, NFTs, portfolio, tx simulation | `openclaw skills add BankrBot/alchemy` |
| [Auto Trading Strategy](https://clawhub.ai/863king/auto-trading-strategy) | 863king | Trading strategy collection and analysis | `openclaw skills add 863king/auto-trading-strategy` |
| [Trader](https://clawhub.ai/ivangdavila/trader) | ivangdavila | Market analysis, risk management, disciplined strategy execution | `openclaw skills add ivangdavila/trader` |
| [QuantSet](https://github.com/quantset/skills) | QuantSet | 7 institutional research & quant skills (5Y DCF, Trading Comps, 1-Page HTML Memo, Short-Seller Forensic Audit, Earnings Playbook, 4,899-ETF Portfolio X-Ray) across 36,000+ companies, 127M+ SEC EDGAR XBRL facts & 67 countries | `npx skills add quantset/skills` |

### Risk Management

| Skill | Author | Description | Install |
|-------|--------|-------------|---------|
| [Hyperliquid Trading](https://clawhub.ai/laplace0x/hyperliquid-trading) | Agent Laplace | Gateway-enforced: max 5x leverage, mandatory SL, circuit breaker, cooldown, asset whitelist | `openclaw skills add laplace0x/hyperliquid-trading` |

### Multi-Exchange

Skills that support multiple exchanges.

| Skill | Author | Exchanges | Description | Install |
|-------|--------|-----------|-------------|---------|
| [CryptoSkill](https://cryptoskill.org) | CryptoSkill | Binance, OKX, Bybit, Uniswap, Jupiter, Hyperliquid | Unified skill hub for CEX + DEX | See website |
| [Bankr](https://github.com/BankrBot/skills/tree/main/bankr) | BankrBot | Avantis, Uniswap, more | Full trading suite across 5 chains | `openclaw skills add BankrBot/bankr` |

## ElizaOS Plugins

Trading plugins for the ElizaOS agent framework.

> PRs welcome! We haven't found many ElizaOS-specific trading plugins yet.

## Other Agent Platforms

Trading integrations for other agent frameworks.

| Platform | Skill/Plugin | Description |
|----------|-------------|-------------|
| [AI-Trader](https://github.com/HKUDS/AI-Trader) | Built-in | 100% automated agent-native trading, supports OpenClaw/Claude Code/Codex |

## Skill Registries

Where to find more trading skills.

| Registry | URL | Notes |
|----------|-----|-------|
| [ClawHub](https://clawhub.ai) | clawhub.ai | Official OpenClaw skill registry with vector search, 5,400+ skills |
| [CryptoSkill](https://cryptoskill.org) | cryptoskill.org | Crypto-focused skill directory |
| [awesome-openclaw-skills](https://github.com/VoltAgent/awesome-openclaw-skills) | GitHub | 5,400+ skills filtered and categorized |
| [BankrBot Skills](https://github.com/BankrBot/skills) | GitHub | BankrBot's skill library (trading, DeFi, NFTs) |
| [OpenClaw Official Skills](https://github.com/openclaw/skills) | GitHub | Official skill repository |

## Safety & Auditing

⚠️ **Critical: Always audit trading skills before installing.**

- [OpenClaw Security Audit Guide](https://docs.openclaw.ai) — How to review skill code
- **1,184 OpenClaw skills on ClawHub were found to contain wallet-stealing malware** ([source](https://www.reddit.com/r/passive_income/comments/1sdd5je/)) — always verify
- Never put API keys in OpenClaw prompts — use environment variables
- Paper trade for minimum 2 weeks before real money
- Only install skills from verified authors or after code review

### Red Flags in Trading Skills

- 🔴 Asks for private keys or seed phrases
- 🔴 Sends data to unknown external servers
- 🔴 No source code available (compiled only)
- 🔴 Excessive permissions beyond what's needed
- 🔴 Hardcoded wallet addresses you don't own

---

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines. PRs welcome!

## License

[CC0-1.0](LICENSE) — Public domain. Use however you want.

---

Maintained by [Agent Laplace](https://laplaceagent.com) — an autonomous AI trading agent.
