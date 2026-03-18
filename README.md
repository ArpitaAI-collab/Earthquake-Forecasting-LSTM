# 📡 Earthquake Forecasting — LSTM
### Deep Learning · Time Series | Seismic Magnitude & Frequency Forecasting

> LSTM time series model for earthquake magnitude and frequency forecasting using sliding window sequences on multi-year seismic data. Achieves **RMSE of 6.0** on holdout test set.

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=flat-square&logo=python)
![LSTM](https://img.shields.io/badge/Model-LSTM-teal?style=flat-square)
![Keras](https://img.shields.io/badge/Framework-Keras%20%7C%20TensorFlow-orange?style=flat-square&logo=tensorflow)
![RMSE](https://img.shields.io/badge/RMSE-6.0-gold?style=flat-square)
![Domain](https://img.shields.io/badge/Domain-Geoscience%20%7C%20Time%20Series-brown?style=flat-square)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=flat-square)

> 🔒 **Private Repo · README only.** Source code not publicly accessible.

---

## 📌 Overview

Earthquake forecasting differs from prediction — rather than classifying whether an event will occur, forecasting aims to **estimate when and how strongly** seismic activity will manifest over time. This project applies a **Long Short-Term Memory (LSTM)** neural network to multi-year seismic time series data, using sliding window sequences to learn temporal patterns in earthquake magnitude and frequency. The model achieves an **RMSE of 6.0** on the holdout test set.

---

## 🎯 Objective

Forecast earthquake magnitude and/or frequency over a future time horizon by learning temporal dependencies in historical seismic sequences — capturing patterns like aftershock decay, periodic stress release, and regional seismic cycles.

---

## 🧱 Technical Approach

| Component | Detail |
|---|---|
| **Dataset** | Multi-year historical seismic event time series |
| **Sequence Design** | Sliding window approach — fixed-length input sequences mapped to future target values |
| **Model** | Stacked LSTM network |
| **Framework** | Keras / TensorFlow |
| **Loss Function** | Mean Squared Error (MSE) |
| **Evaluation** | RMSE on holdout test set |
| **RMSE** | **6.0** |

---

## 🔬 Methodology

1. **Time Series Construction** — converted raw seismic event records into regularly sampled time series; aggregated events by time window (magnitude, frequency, energy release)
2. **Sliding Window Sequences** — created supervised learning sequences: each input window of *n* timesteps maps to a forecast target *k* steps ahead
3. **LSTM Architecture** — stacked LSTM layers to capture both short-term aftershock patterns and longer-term seismic cycle dependencies; dropout regularisation to prevent overfitting on limited seismic data
4. **Training** — trained on the majority of the multi-year sequence; validated on a held-out recent period to simulate real forecasting conditions
5. **Evaluation** — RMSE computed on the holdout test set as the primary forecasting quality metric

---

## 📊 Results

| Metric | Score |
|---|---|
| RMSE (Holdout Test Set) | **6.0** |
| Task | Seismic magnitude / frequency forecasting |
| Architecture | Stacked LSTM with sliding window sequences |

---

## 🔑 Key Takeaways

- LSTM effectively captures temporal dependencies in seismic sequences including aftershock decay patterns
- Sliding window design critical for transforming irregular seismic event data into supervised sequences
- Multi-year training horizon allows model to learn seasonal and cyclical seismic patterns
- RMSE of 6.0 reflects the inherent stochasticity of seismic systems — forecasting is fundamentally probabilistic

---

## 🛠️ Tech Stack

`Python` `Keras` `TensorFlow` `NumPy` `Pandas` `Matplotlib` `scikit-learn`

---

## 👩‍💻 Author

**Arpita Paul** · Senior Data Scientist · *From Seismology to GenAI 🚀*

[![GitHub](https://img.shields.io/badge/GitHub-ArpitaAI--collab-black?style=flat-square&logo=github)](https://github.com/ArpitaAI-collab)
