# RTR 1.3.6 — Trend & Trade Zone Indicator

> A TradingView Pine Script™ v5 indicator for trend identification, volatility filtering, multi-timeframe analysis, and structured trade-level visualization.

[![Pine Script](https://img.shields.io/badge/Pine%20Script-v5-2962FF?style=flat-square&logo=tradingview&logoColor=white)](https://www.tradingview.com/pine-script-docs/)
[![Version](https://img.shields.io/badge/version-1.3.6-111827?style=flat-square)](#version)
[![Status](https://img.shields.io/badge/status-private%20development-6B7280?style=flat-square)](#project-status)

---

## Overview

**RTR 1.3.6** is a TradingView indicator built with Pine Script v5 and designed around a simple workflow:

**Identify trend → filter market conditions → visualize trade levels → monitor multiple timeframes → configure alerts.**

The indicator combines an EMA ribbon, ATR-based volatility filtering, structure-aware trade levels, multiple take-profit targets, and an on-chart multi-timeframe dashboard in a single workspace.

## Core Features

### Trend Detection
- Six-level EMA ribbon using **31, 35, 40, 45, 51, and 58** periods.
- Bullish and bearish trend-state identification based on ribbon alignment.
- Configurable signal visibility and lookback settings.

### Dynamic Trade Levels
- Entry level visualization.
- Structure-based Stop Loss with an ATR buffer.
- Up to **7 configurable Take Profit targets**.
- Custom risk-to-reward ratios for TP1–TP7.

### Volatility Filter
- Optional ATR baseline filter.
- Adjustable ATR ratio threshold.
- Designed to help filter lower-volatility market conditions.

### Multi-Timeframe Dashboard
- Monitor trend alignment across **5 customizable timeframes**.
- Configurable dashboard placement.
- Displays active unrealized PnL alongside timeframe information.

### Alerts
- Built-in `alertcondition` triggers for RTR Buy/Sell signals and trade setups.
- Intended for TradingView alert workflows.

---

## Project Structure

```text
RTR-1.3.6/
├── README.md
└── RTR.pine
```

> The Pine Script source is currently kept at the repository root.

## Installation

1. Open [TradingView](https://www.tradingview.com/).
2. Open **Pine Editor**.
3. Open `RTR.pine` from this repository.
4. Copy the complete Pine Script source.
5. Paste it into the TradingView Pine Editor.
6. Save the script.
7. Add the indicator to a chart.

## Configuration

| Area | Available Controls |
|---|---|
| **Signals** | Buy/Sell labels and signal lookback/size settings |
| **Filter** | ATR baseline filter and ATR ratio threshold |
| **Trade Levels** | Stop Buffer ATR and TP1–TP7 risk-to-reward ratios |
| **Dashboard** | Dashboard position and five monitored timeframes |

## Design Approach

RTR is organized around a small number of practical charting components rather than a collection of unrelated signals:

```text
Market Data
    ↓
EMA Ribbon ──────────────→ Trend State
    ↓
ATR Filter ──────────────→ Market Condition
    ↓
Structure + ATR Buffer ──→ Stop Level
    ↓
Risk / Reward Inputs ────→ TP1 … TP7
    ↓
MTF Dashboard + Alerts ─→ Monitoring & Execution Support
```

This structure keeps the indicator focused on **decision support and visual trade management** rather than attempting to predict market outcomes.

## Version

**Current version:** `1.3.6`

RTR is under active private development. Configuration, calculations, visual behavior, and supported features may change between versions.

## Project Status

🔒 **Private development repository**

This repository contains the working source for RTR 1.3.6. Distribution and access are controlled by the project owner.

## Important Note

RTR is a charting and technical-analysis tool. It does **not** guarantee profitable trades or future market performance. Trading involves substantial risk, and users should evaluate any strategy independently before using it with real capital.

---

## Author

**Prem Sai Bachchala**  
GitHub: [@premsai841](https://github.com/premsai841)

Built as an independent technical product project focused on practical charting workflows, indicator design, and iterative product development.
