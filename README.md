# RTR 1.3.6 - Trend & Trade Zone Indicator

A comprehensive TradingView Pine Script (v5) indicator designed for trend-following and dynamic trade management. RTR utilizes an advanced EMA ribbon for trend identification, an ATR filter to avoid low-volatility chop, and an integrated multi-timeframe (MTF) dashboard.

## Key Features

*   **EMA Ribbon Trend Detection:** Uses a 6-level EMA ribbon (31, 35, 40, 45, 51, 58) to determine pure bullish or bearish trends.
*   **Dynamic Trade Zones:** Automatically calculates and plots Entry, Stop Loss (based on structure highs/lows + ATR buffer), and up to 7 Take Profit (TP) targets.
*   **ATR Volatility Filter:** Optional toggle to ensure trades are only taken during periods of sufficient market volatility.
*   **Multi-Timeframe Dashboard:** Real-time on-chart display monitoring trend alignments across 5 customizable timeframes, plus active unrealized PnL.
*   **RTR Alerts:** Built-in `alertcondition` triggers for automated RTR Buy/Sell signals and trade setups.

## Installation

1. Open [TradingView](https://www.tradingview.com/).
2. Navigate to the **Pine Editor** tab at the bottom of the screen.
3. Open the `src/RTR.pine` file from this repository and copy all the code.
4. Paste the code into the Pine Editor, replacing any existing code.
5. Click **Save** and then **Add to Chart**.

## Configuration & Inputs

*   **Signals:** Toggle Buy/Sell labels and adjust signal lookback length (Tiny, Small, Mid, Large).
*   **Filter:** Enable/disable the ATR baseline filter and adjust the ATR ratio threshold.
*   **Trade Levels:** Define the Stop Buffer ATR and customize risk-to-reward ratios for TP1 through TP7. 
*   **Dashboard:** Position the MTF dashboard anywhere on the chart and customize the 5 monitored timeframes.
