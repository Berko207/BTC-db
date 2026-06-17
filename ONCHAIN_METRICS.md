# On-Chain Metrics & Indicators for Bitcoin Trading Context

**Purpose**: Key historical on-chain data points and metrics that are commonly used in trading systems, dashboards, and on-chain analysis integrations. This provides context rather than real-time data.

## Why On-Chain Data Matters for Trading Integrations

On-chain metrics often lead or confirm price action:
- **Accumulation/Distribution** signals from long-term holders
- **Network health** (hashrate, active addresses)
- **Realized price** vs spot price (MVRV)
- **Exchange flows** (inflows often precede selling pressure)

## Core Historical On-Chain Milestones & Trends

### Hashrate & Network Security

| Period          | Hashrate Milestone                  | Context / Trading Implication                     |
|-----------------|-------------------------------------|---------------------------------------------------|
| 2009–2012      | From <1 TH/s to ~10 TH/s           | Early hobbyist mining era                        |
| 2013–2016      | Explosive growth to ~1 EH/s        | Industrial mining begins; China dominance       |
| 2017–2020      | Multiple all-time highs            | Bull market mining profitability                 |
| May 2021       | ~180 EH/s peak then China ban drop | Major hashrate migration event                   |
| 2022–2024      | Recovery to new ATHs (>600 EH/s)   | Post-China professionalization                   |
| 2025–2026      | Continued growth (>700 EH/s range) | Institutional-grade infrastructure               |

**Trading note**: Sudden hashrate drops can signal miner capitulation (often local bottoms).

### Active Addresses & Network Activity

- **2017 Bull**: Daily active addresses peaked near 1.2M during mania.
- **2021 Bull**: Higher peak (~1.5M+ daily) showing broader adoption.
- **2022 Bear**: Dropped significantly during FTX collapse.
- **2024–2025**: New highs in active addresses post-ETF approval, driven by institutional wallets and Layer-2 activity.

**Integration tip**: Spikes in active addresses during price consolidation can precede breakouts.

### Exchange Balances & Flows

| Event                  | Exchange BTC Balance Trend       | Typical Price Reaction       |
|------------------------|----------------------------------|------------------------------|
| 2020–2021 Accumulation | Steady decline                   | Bullish (coins moving to self-custody) |
| Nov 2022 (FTX)        | Sharp inflows then stabilization | Capitulation low             |
| 2024 ETF Launch       | Accelerated outflows             | Strong bullish signal        |
| 2025–2026             | Continued net outflows           | Institutional holding preference |

**Key metric**: Exchange Reserve (lower = bullish long-term).

### Realized Price & MVRV Ratio

- **Realized Price**: Average price at which all coins last moved (on-chain cost basis).
- **MVRV Ratio** (Market Value / Realized Value): >3.5 often marks local tops; <1 marks deep bear market bottoms.

Historical examples:
- 2017 top: MVRV > 3.5–4
- 2021 top: MVRV ~3.8–4
- 2022 bottom: MVRV approached 0.8–1.0
- 2024–2025 cycle: MVRV stayed elevated longer due to ETF buying (new paradigm?)

**Trading use**: MVRV divergences from price can provide mean-reversion or momentum signals.

### Long-Term Holder (LTH) Behavior

- LTH supply (coins held >155 days) tends to decrease during bull markets (profit-taking) and increase in bears (accumulation).
- **2024–2025**: Record LTH accumulation despite new ATHs — strong conviction signal.

## Recommended On-Chain Data Providers for Integrations

| Provider       | Strengths                              | Best For Trading Systems          | Access          |
|----------------|----------------------------------------|-----------------------------------|-----------------|
| Glassnode      | Comprehensive on-chain dashboards     | Professional analytics            | API / Paid     |
| Dune Analytics | Custom SQL queries on blockchain data | Flexible backtesting              | Free + Paid    |
| CryptoQuant    | Exchange flows & whale alerts         | Real-time flow monitoring         | API            |
| Arkham         | Entity labeling & intelligence        | Institutional wallet tracking     | API            |
| Bitquery       | On-chain event streaming              | Custom dashboards & bots          | GraphQL API    |

## Gaps & Notes

- Exact historical numbers fluctuate; use the providers above for precise time-series data.
- Post-2024 ETF era introduced new on-chain patterns (custodial wallets, ETF-related flows) that traditional metrics interpret differently.
- Combine on-chain with derivatives data (funding rates, open interest) for stronger signals.

---

*This file is meant to be extended with specific time-series data or API integration examples.*