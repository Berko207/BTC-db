# Data Sources, APIs & Tools for Bitcoin Trading Integrations

**Purpose**: Curated list of reliable data providers, APIs, and tools commonly used when building trading systems, dashboards, analytics platforms, or on-chain monitoring tools that reference Bitcoin history and context.

## Core Categories

### 1. Price & Market Data

| Provider          | Coverage                          | Granularity     | Strengths                          | Pricing      | Notes for Integrations                  |
|-------------------|-----------------------------------|-----------------|------------------------------------|--------------|-----------------------------------------|
| Binance / Coinbase| Spot, futures, options            | Tick to daily  | High liquidity, WebSocket          | Free tier   | Good for execution & historical OHLCV  |
| Kaiko             | Institutional-grade market data   | Tick + order book | Clean, normalized, multi-exchange | Paid        | Excellent for backtesting              |
| CryptoCompare     | Aggregated prices + on-chain      | Various        | Easy API, broad coverage           | Free + Paid | Good starting point                    |
| CoinGecko / CoinMarketCap | Broad market data + historical | Daily + hourly | Free API, easy to use             | Free tier   | Quick prototyping                      |

### 2. On-Chain Data

| Provider       | Key Data                          | Best Use Case                     | Access          |
|----------------|-----------------------------------|-----------------------------------|-----------------|
| Glassnode      | Full suite (MVRV, SOPR, exchange flows, LTH supply) | Professional on-chain analysis   | API (paid)     |
| Dune Analytics | Custom queries on raw blockchain data | Flexible dashboards & backtests  | Free + Pro     |
| CryptoQuant    | Exchange inflows/outflows, whale movements | Real-time flow alerts            | API            |
| Arkham Intelligence | Wallet labeling & entity clustering | Institutional flow tracking     | API            |
| Bitquery       | On-chain events, transfers, smart contract activity | Custom bots & streaming         | GraphQL        |

### 3. Prediction Markets & Sentiment

| Provider       | Focus                             | Relevance to BTC                  | Access          |
|----------------|-----------------------------------|-----------------------------------|-----------------|
| Polymarket     | Yes/No event contracts            | Short-term price & event markets | Web + API      |
| Kalshi         | Regulated event contracts         | 15m BTC up/down markets          | Web + API      |
| PredictIt / others | Broader event betting          | Sentiment proxy                  | Web            |

### 4. Derivatives & Order Flow

| Provider       | Data Type                         | Use Case                          | Access          |
|----------------|-----------------------------------|-----------------------------------|-----------------|
| Binance / Bybit| Funding rates, open interest, liquidation data | Perp market structure           | API            |
| Skew / Laevitas| Options flow & skew               | Volatility & positioning         | Paid           |
| Coinalyze      | Aggregated derivatives data       | Multi-exchange perp analysis     | Web + API      |

### 5. News, Social & On-Chain Intelligence

| Tool           | Type                              | Trading Use                       | Access          |
|----------------|-----------------------------------|-----------------------------------|-----------------|
| LunarCrush     | Social sentiment + on-chain       | Narrative & hype cycle tracking  | API            |
| Santiment      | On-chain + social metrics         | Early signal detection           | API            |
| The Block / CoinDesk | News + research               | Fundamental context              | Web + API      |
| Arkham         | Wallet intelligence               | Smart money tracking             | API            |

### 6. Historical Datasets (Free/Public)

- **Kaggle**: Multiple BTC 5m Polymarket resolution datasets + order book snapshots
- **CryptoDataDownload.com**: Free daily/hourly/1m OHLCV CSVs
- **Bitcoin blockchain explorers** (mempool.space, blockstream.info) for manual verification

## Recommended Stack for Trading System Builders

**Minimal viable stack**:
- Price data: Binance WebSocket + historical from Kaiko or CryptoDataDownload
- On-chain: Dune (for custom queries) + Glassnode (for polished metrics)
- Execution: Binance / Coinbase Advanced Trade API
- Monitoring: Custom dashboard (Grafana + InfluxDB or lightweight Python)

**Advanced stack**:
- Real-time on-chain streaming: Bitquery or custom node
- Wallet intelligence: Arkham
- Prediction market arbitrage / hedging: Polymarket API + on-chain settlement monitoring

## Important Notes

- Always cross-verify critical data (especially resolution of prediction markets).
- Post-2024 ETF era changed some traditional on-chain interpretations (large custodial wallets behave differently from retail).
- Rate limits and data freshness vary significantly between providers.
- For production systems, combine multiple sources and implement fallback logic.

---

*This file should be updated as new high-quality data providers emerge.*