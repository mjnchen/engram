---
title: Prophet
url: https://facebook.github.io/prophet/
maker: Meta (Facebook Research)
tags: [forecasting, time-series, python, r, anomaly-detection]
created: 2026-05-15
---

# Prophet

## What it is

Open-source time series forecasting library from Facebook Research. Fits an additive model with trend, yearly/weekly/daily seasonality, and holiday effects. Works well on business time series with strong seasonal patterns and missing data.

## What problem it solves

Makes reliable forecasting accessible without deep time-series expertise. Automatically detects changepoints in trend and handles irregular data. Outputs uncertainty intervals useful for anomaly detection (flag actuals outside predicted bounds).

## Concepts

- [[time-series-anomaly-detection]]

## Notes

- [Prophet paper: Forecasting at scale (Facebook Research)](https://research.fb.com/prophet-forecasting-at-scale/)
- Python and R interfaces
- Frequently used as the forecasting backbone in anomaly detection systems
