# Purple Dot Indicator

A Pine Script indicator for TradingView that combines volume, rate of change (ROC), and moving averages to enhance technical analysis. This script includes optional visualizations for SMAs and VWAP across multiple timeframes.

---

## Features

1. **Purple Dot Plot**

    - Displays a purple dot below bars when specific conditions are met:
        - Volume is greater than the specified threshold.
        - Rate of change (ROC) meets or exceeds the defined percentage.

2. **Simple Moving Averages (SMA)**

    - Displays the following SMAs for enhanced trend visualization:
        - 10-period SMA (green)
        - 20-period SMA (navy)
        - 50-period SMA (fuchsia)
    - SMA visibility can be toggled via settings.

3. **Volume Weighted Average Price (VWAP)**
    - Plots the VWAP for lower timeframes (1, 5, 15, and 30 minutes).

---

## Inputs

| Input Name                | Type     | Default Value | Description                                  |
| ------------------------- | -------- | ------------- | -------------------------------------------- |
| `Combine the conditions?` | Checkbox | `true`        | Combines multiple conditions for plotting.   |
| `Show 10 Period SMA`      | Checkbox | `true`        | Toggles visibility of the 10-period SMA.     |
| `Show 20 Period SMA`      | Checkbox | `true`        | Toggles visibility of the 20-period SMA.     |
| `Show 50 Period SMA`      | Checkbox | `true`        | Toggles visibility of the 50-period SMA.     |
| `Volume above`            | Number   | `1,000,000`   | Minimum volume for the condition to trigger. |
| `% check`                 | Number   | `4`           | Minimum rate of change (ROC) percentage.     |

---

## Timeframe-Specific Behavior

-   **Daily or Weekly Timeframes**:
    -   SMAs are displayed when enabled.
-   **1, 5, 15, 30-Minute Timeframes**:
    -   VWAP is displayed.

---

## Plotted Elements

-   **Purple Dot**: Appears below bars when conditions are met.
-   **SMA Lines**: Trend-following indicators for short, medium, and long-term trends.
-   **VWAP Line**: Weighted average price for intraday timeframes.

---

## How to Use

1. **Add to Chart**: Copy the script into Pine Script editor on TradingView and add it to your chart.
2. **Adjust Inputs**: Use the settings panel to configure the conditions and visibility of SMAs.
3. **Interpret the Plots**:
    - Look for purple dots below bars to identify potential setups based on volume and ROC.
    - Use SMAs and VWAP for additional trend and price level analysis.

---

## Notes

-   This script is optimized for daily, weekly, and intraday analysis.
-   Ensure proper timeframe selection for SMA and VWAP to work as intended.

---

## Disclaimer

This indicator is for educational and informational purposes only. It is not financial advice. Use at your own risk.
