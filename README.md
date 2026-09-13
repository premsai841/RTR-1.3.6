# RTR 1.3.6 — TradingView Indicator

> An independent TradingView Pine Script project focused on trend identification, volatility filtering, multi-timeframe analysis, and structured trade-level visualization.

## Portfolio context

RTR is my independent digital-product project. It is separate from my main Customer Success portfolio, but it demonstrates product thinking, user-focused configuration, documentation, iteration, and experience working with a technical product.

## Overview

**RTR 1.3.6** is a TradingView indicator built with Pine Script v5 around a practical workflow:

**Identify trend → filter market conditions → visualize trade levels → monitor multiple timeframes → configure alerts.**

The indicator combines an EMA ribbon, ATR-based filtering, structure-aware trade levels, multiple take-profit targets, and an on-chart multi-timeframe dashboard.

## Core features

- EMA ribbon for trend-state identification
- ATR-based volatility filtering
- Structure-aware Stop Loss with ATR buffer
- Up to 7 configurable Take Profit targets
- Multi-timeframe dashboard
- Buy/Sell and trade-setup alerts
- Configurable chart and dashboard settings

## Project structure

```text
RTR-1.3.6/
├── README.md
└── RTR.pine
```

The Pine Script source is kept at the repository root.

## Installation

1. Open TradingView and Pine Editor.
2. Open `RTR.pine` from this repository.
3. Copy the complete Pine Script source.
4. Paste it into Pine Editor.
5. Save the script and add it to a chart.

## Design approach

```text
Market Data
    ↓
EMA Ribbon → Trend State
    ↓
ATR Filter → Market Condition
    ↓
Structure + ATR Buffer → Stop Level
    ↓
Risk / Reward Inputs → TP1 … TP7
    ↓
MTF Dashboard + Alerts → Monitoring Support
```

The project is designed as a decision-support and visualization tool rather than a guarantee of market outcomes.

## Version

**Current version:** `1.3.6`

Configuration, calculations, visual behavior, and supported features may change as the product evolves.

## Technical note

This repository contains Pine Script source code. It should be viewed as an independent product/technical project and not as evidence of professional software-development experience.

## Risk disclaimer

RTR is a technical-analysis tool. It does not guarantee profitable trades or future market performance. Trading involves substantial risk; users should evaluate any strategy independently before using it with real capital.

## Author

**Prem Sai Bachchala**  
GitHub: [@premsai841](https://github.com/premsai841)
