# AutoReg (AR) Time Series Analysis

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=0a0f1c&height=120&section=header&text=AutoReg%20Time%20Series%20Model&fontSize=38&fontColor=00e5ff" />
</p>

---

## Overview

This project demonstrates **time series modeling using the AutoRegressive (AR) model** from `statsmodels`. It focuses on understanding lag-based dependencies, model diagnostics, and statistical interpretation using a clean, production-ready workflow.

The implementation is suitable for **data science portfolios, interviews, and academic submissions**.

---

## Visual Architecture

```text
Time Series Data
       ↓
 Lagged Features (y(t-1), y(t-2))
       ↓
 AutoReg Model (Conditional MLE)
       ↓
 Statistical Summary
       ↓
 Prediction & Diagnostics
```

---

## Tech Stack

| Category      | Tools            |
| ------------- | ---------------- |
| Language      | Python           |
| Libraries     | NumPy, Pandas    |
| Visualization | Matplotlib       |
| Modeling      | statsmodels      |
| Environment   | Jupyter Notebook |

---

## Skills Demonstrated

* Time Series Forecasting
* AutoRegressive (AR) Modeling
* Lag Feature Engineering
* Statistical Inference (p-values, confidence intervals)
* Model Stability Analysis (Roots)
* Model Selection (AIC, BIC, HQIC)
* Data Visualization
* Research-Oriented Interpretation

---

## Mathematical Foundation

The AutoRegressive model of order (p):

[
Y_t = c + \sum_{i=1}^{p} \phi_i Y_{t-i} + \varepsilon_t
]

Where:

* (Y_t) is the current value
* (\phi_i) are lag coefficients
* (c) is a constant
* (\varepsilon_t) is white noise

---

## Implementation

```python
from statsmodels.tsa.ar_model import AutoReg

model = AutoReg(data, lags=2)
model_fit = model.fit()
print(model_fit.summary())
```

---

## Model Diagnostics Explained

### Coefficients

* Measure the influence of past values
* Statistical significance evaluated using p-values

### Information Criteria

* AIC / BIC used for model comparison
* Lower values indicate better trade-off between fit and complexity

### Roots Analysis

* Stability condition: all roots must have modulus > 1
* Ensures stationarity and reliable forecasting

---

## Interpretation Highlights

* AR(1) captures short-term dependency
* AR(2) captures medium-term memory
* Model stability verified through root modulus
* Limited observations lead to higher uncertainty

---

## Project Structure

```text
├── ARLM/
│   └── Times Series Forcasting.ipynb
├── README.md
```

---

## Interactive Enhancements (Optional)

* Movable diagram support via Mermaid.js
* Cursor-follow animations using CSS (for web export)
* Dynamic model comparison dashboard (Streamlit-ready)

---

## Use Cases

* Financial time series forecasting
* Sensor data trend modeling
* Academic AR model demonstrations
* Baseline comparison for ARIMA / LSTM

---

## Limitations

* Requires stationary data
* Sensitive to outliers
* Performance depends on lag selection

---

## Future Enhancements

* ARIMA and SARIMA integration
* Automated lag selection
* Residual diagnostics dashboard
* LSTM benchmark comparison

---

## Author

**Debashish Parida**
Data Science | Machine Learning | Time Series Analysis

---

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=0a0f1c&height=80&section=footer&text=Time%20Series%20Modeling%20with%20AutoReg&fontSize=20&fontColor=00e5ff" />
</p>
