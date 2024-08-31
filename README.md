# TESS-data
# 🌟 Machine Learning-Based Gap Filling in Stellar Light Curves Using TESS Data

This repository contains code and instructions for performing machine learning-based gap filling in stellar light curves. The analysis is centered around the **transit method** using data from NASA's TESS (Transiting Exoplanet Survey Satellite). The project leverages `lightkurve`, a Python library for analyzing time series data of celestial objects.

## 🚀 Overview

The goal of this project is to preprocess light curve data, identify gaps, and use a neural network to predict and fill these gaps. The steps involved include:

1. **Loading TESS Data**: We use `lightkurve` to access and download light curves directly from TESS.
2. **Preprocessing**:
   - **Flattening**: Remove long-term trends to better analyze periodic signals.
   - **Folding**: Align data points by their period to enhance the visibility of periodic features.
   - **Periodogram**: Identify the most likely period using a periodogram.
3. **Machine Learning**:
   - Train a neural network model to predict missing flux values in the light curve.
   - Evaluate the model's performance using cross-validation.

## 🛠️ Installation

To get started, clone the repository and install the necessary dependencies:

```bash
git clone https://github.com/Krishna17-bit/TESS-data.git
cd TESS-data
pip install -r requirements.txt
