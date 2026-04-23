# Examples — Time Series & Anomaly Detection

## Example 1 — Initial time-series visualization

Plot a series and detect visual trend/seasonality cues.

## Example 2 — Forecast baseline

Implement a naive forecast and a moving average.

## Example 3 — Improved temporal model

Apply ARIMA/Prophet-style ideas and compare metrics.

## Example 4 — Anomaly detection

Use residuals or z-scores to flag anomalous points.

## Rules

- Each example must include the objective, steps, and expected output.
- Record observations in `notes/`.

## Ejemplos disponibles

### Executable scripts (phase-2 continuation)

1. `01_time_series_visualization_baseline.py`

   - Reads a synthetic series and computes lightweight trend signals.
   - Expected output: upward/downward trend label and trailing moving average.

1. `02_naive_vs_moving_average_forecast.py`

   - Compares two baseline forecasting strategies.
   - Expected output: MAE comparison between naive and moving-average forecast.

1. `03_seasonal_baseline_forecast.py`

   - Forecasts by repeating the last observed season.
   - Expected output: seasonal prediction list and MAPE score.

1. `04_zscore_anomaly_detection.py`

   - Flags outliers using z-score thresholding.
   - Expected output: anomaly count plus index/value/z-score triples.

1. `05_residual_anomaly_detection.py`

   - Detects anomalies from one-step forecast residuals.
   - Expected output: residual anomaly count and index/residual values.

1. `06_reproducible_timeseries_pipeline.py`

   - Runs a deterministic mini pipeline for generation + forecast.
   - Expected output: `same_result=True` when seed is unchanged.

## Como usar estos ejemplos

```bash
python modules/07-time-series-anomaly-detection/examples/01_time_series_visualization_baseline.py
python modules/07-time-series-anomaly-detection/examples/02_naive_vs_moving_average_forecast.py
python modules/07-time-series-anomaly-detection/examples/03_seasonal_baseline_forecast.py
python modules/07-time-series-anomaly-detection/examples/04_zscore_anomaly_detection.py
python modules/07-time-series-anomaly-detection/examples/05_residual_anomaly_detection.py
python modules/07-time-series-anomaly-detection/examples/06_reproducible_timeseries_pipeline.py
```

Recommended order: run from `01` to `06` to preserve the baseline-to-anomaly progression.

## Proximos pasos

1. Add a simplified rolling-origin backtesting example.
1. Add precision/recall style scoring for anomaly detection.
1. Record observed failure modes in `notes/README.md`.
