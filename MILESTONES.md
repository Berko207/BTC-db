# Bitcoin Key Milestones & Data Tables

This file contains structured tables optimized for parsing by trading systems, scripts, and analytics tools.

## Bitcoin Halvings

| Halving # | Date              | Block Height | Previous Reward | New Reward | Price on Halving Day (approx) | Cycle ATH (approx) |
|-----------|-------------------|--------------|-----------------|------------|-------------------------------|--------------------|
| 1         | Nov 28, 2012     | 210,000     | 50 BTC         | 25 BTC    | ~$12                          | ~$1,150 (2013)    |
| 2         | Jul 9, 2016      | 420,000     | 25 BTC         | 12.5 BTC  | ~$650                         | ~$19,800 (2017)   |
| 3         | May 11, 2020     | 630,000     | 12.5 BTC       | 6.25 BTC  | ~$8,600                       | ~$69,000 (2021)   |
| 4         | Apr 20, 2024     | 840,000     | 6.25 BTC       | 3.125 BTC | ~$64,000                      | ~$126,000 (2025)  |
| 5 (next)  | ~Apr 2028        | 1,050,000   | 3.125 BTC      | 1.5625 BTC| -                             | -                 |

## Major All-Time Highs (ATH)

| Date              | Price (USD)    | Context                              |
|-------------------|----------------|--------------------------------------|
| Dec 2013         | ~$1,150       | First major bubble peak             |
| Dec 2017         | ~$19,800      | ICO mania peak                      |
| Nov 2021         | ~$69,000      | Post-2020 halving bull run          |
| Mar 2024         | ~$73,664      | Pre-4th halving + ETF anticipation  |
| Oct 2025         | ~$126,000     | Post-ETF + institutional cycle peak |

## Major Protocol Upgrades

| Upgrade   | Activation Date   | Block     | Key Benefits                              | Impact on Trading/Integrations          |
|-----------|-------------------|-----------|-------------------------------------------|-----------------------------------------|
| SegWit    | August 2017      | ~481,824 | Block capacity increase, malleability fix | Better transaction reliability         |
| Taproot   | November 2021    | ~709,632 | Schnorr signatures, improved privacy     | More efficient smart contracts & privacy|

## Notable Institutional & Regulatory Milestones

- **2020**: MicroStrategy starts corporate Bitcoin treasury
- **2021**: El Salvador makes Bitcoin legal tender
- **Jan 2024**: U.S. SEC approves spot Bitcoin ETFs
- **2024–2025**: Massive ETF inflows drive institutional adoption
- **2025**: Discussions around strategic Bitcoin reserves in multiple countries

## Notes for Integrators

- All dates and prices are approximate and sourced from public records.
- For precise on-chain data, cross-reference with explorers (mempool.space, blockstream.info).
- This repo focuses on high-level context rather than tick-level price data.

*Last updated: June 2026*