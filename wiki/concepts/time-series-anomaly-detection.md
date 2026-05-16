---
title: Time-Series Anomaly Detection
tags: [anomaly-detection, time-series, statistics, ml]
created: 2026-05-15
source:
---

# Time-Series Anomaly Detection

## Summary

Detecting anomalous points or intervals in sequential data. Approaches range from classical statistical methods (Holt-Winters, STL decomposition) to ML-based models (LSTM, isolation forest) to learned thresholds on forecasts.

## Key Ideas

- **Decomposition-based**: separate trend, seasonality, residual; flag outliers in residuals (STL, Twitter Anomaly Detection)
- **Forecasting-based**: predict expected value, flag when actual deviates beyond confidence interval (Holt-Winters ETS, Prophet, ARIMA)
- **Change-point detection**: detect structural shifts in mean/variance rather than individual outliers (Twitter BreakoutDetection, PELT, ecp)
- **ML-based**: LSTM reconstruction error, isolation forest, RBM-based detectors
- **Multivariate**: harder — must model cross-signal correlations; most production systems use univariate per-metric

Key challenge: seasonality makes naive z-score approaches fail. Must account for time-of-day/week patterns before flagging.

## Related

- [[mamba]] (state space models — different use of "state space")
- [[scaling-laws]]

## Resources

- [github.com/rob-med/awesome-TS-anomaly-detection](https://github.com/rob-med/awesome-TS-anomaly-detection)
- [github.com/yzhao062/anomaly-detection-resources](https://github.com/yzhao062/anomaly-detection-resources)
- [Time-Series Anomaly Detection Service at Microsoft (arxiv 1906.03821)](https://arxiv.org/abs/1906.03821)
- [Twitter BreakoutDetection (R)](https://github.com/twitter/BreakoutDetection)
- [LinkedIn Luminol](https://github.com/linkedin/luminol)
- [Numenta NAB benchmark](https://github.com/numenta/NAB)
