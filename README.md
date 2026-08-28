# 💻 Laptop Price Predictor

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.5-orange.svg)](https://scikit-learn.org/)
[![XGBoost](https://img.shields.io/badge/XGBoost-2.1-green.svg)](https://xgboost.readthedocs.io/)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.37-red.svg)](https://streamlit.io/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

A machine learning web application that predicts laptop prices based on hardware specifications — brand, processor, RAM, GPU, storage, display, and operating system. Built end-to-end: raw data → cleaning → feature engineering → model training → interactive Streamlit UI.

---

## 📸 Demo

> *(Add a screenshot or GIF of the running Streamlit app here once deployed)*

---

## ✨ Features

- **Automated data cleaning pipeline** — parses messy spec strings (e.g. `"Intel Core i5 7200U 2.5GHz"`) into structured, model-ready columns
- **Rich feature engineering** — extracts CPU brand/tier, GPU brand, effective PPI (pixels-per-inch) from resolution + screen size, storage type/capacity (HDD/SSD/Hybrid/Flash)
- **Log-transformed target** — stabilizes variance and improves regression performance on skewed price data
- **Model comparison** — benchmarks Random Forest vs. XGBoost regressors with cross-validation
- **Production-ready inference pipeline** — a single serialized `model.pkl` (preprocessing + model) ready to drop into any Python service
- **Interactive Streamlit app** — real-time price prediction from a clean web form, no code required to use it

---

## 🗂️ Project Structure