# Hourly Electricity Consumption & Production Dataset

Hourly electricity consumption and power generation data across energy sources (**46,011** hourly records, **10** columns).

## Files

- `Electricity.csv` — Hourly time-series dataset of electricity demand and generation by source.

## Columns

| Column | Type | Description |
| :--- | :--- | :--- |
| `DateTime` | Timestamp | Exact hour of the record (`YYYY-MM-DD HH:MM:SS`) |
| `Consumption` | Integer | Total electricity consumed during the hour (MWh) |
| `Production` | Integer | Total electricity produced during the hour (MWh) |
| `Nuclear` | Integer | Nuclear power generation (MWh) |
| `Wind` | Integer | Wind turbine generation (MWh) |
| `Hydroelectric` | Integer | Hydroelectric power generation (MWh) |
| `Oil and Gas` | Integer | Oil and natural gas generation (MWh) |
| `Coal` | Integer | Coal-based thermal power generation (MWh) |
| `Solar` | Integer | Solar power generation (MWh) |
| `Biomass` | Integer | Biomass / waste-to-energy generation (MWh) |

## Assignment

Build a time-series forecasting model for **`Consumption`** (and/or **`Production`**):

1. **Explore & Index**: Parse `DateTime` as a datetime index, check for missing timestamps or anomalies, and visualize hourly/daily/seasonal trends.
2. **Feature Engineering**: Extract time-based features (hour, day of week, month, weekend/holiday) and lag/rolling features without data leakage.
3. **Train & Evaluate**: Use a **chronological train/test split** (no random shuffling), train forecasting model(s), and report **MAE**, **RMSE**, and **MAPE**.
4. **Analyze**: Compare renewable (`Wind`, `Hydroelectric`, `Solar`, `Biomass`) vs. non-renewable (`Nuclear`, `Oil and Gas`, `Coal`) generation trends.
