# Copula-Based Portfolio Risk Analysis: NVDA & ORCL

This project analyzes the joint risk structure of two major technology stocks—**NVIDIA (NVDA)** and **Oracle (ORCL)**—using statistical methods, copula modeling, and portfolio tail-risk metrics such as **Value at Risk (VaR)** and **Expected Shortfall (ES)**.  
All computations, visualizations, and simulations are performed in **R**.

---

## 📌 Project Overview

The goal of this study is to:

- Collect historical stock price data (2020–2025)
- Compute monthly losses and descriptive statistics
- Test normality of loss distributions
- Fit theoretical distributions and compare with empirical data
- Estimate **VaR** and **ES** (empirical & theoretical)
- Fit several **copula models** (Clayton, Frank, Gumbel, Gaussian, t-copula)
- Visualize 2D and 3D dependence structures
- Simulate portfolio losses using the best-fit copula
- Evaluate portfolio VaR & ES for weights β ∈ [0, 1]

---

## 📂 Contents

- `data collection` – retrieving historical stock data via **quantmod**
- `loss calculations` – computing NVDA & ORCL monthly losses
- `descriptive statistics` – mean, variance, skewness, kurtosis
- `normality tests` – Shapiro–Wilk, Anderson–Darling
- `VaR & ES estimation` – empirical and analytical formulas
- `distribution fitting` – histograms, density overlays
- `copula modeling` – parameter estimation + model comparison (AIC/BIC)
- `2D/3D visualization` – Plotly surface & contour plots
- `portfolio simulation` – copula-based Monte Carlo modeling
- `results table` – VaR/ES for portfolio weights

---

## 🧪 Methods Used

- **Statistical tests:** Shapiro–Wilk, Anderson–Darling  
- **Risk metrics:** VaR (95%), Expected Shortfall  
- **Copulas:**  
  - Clayton  
  - Frank  
  - Gumbel  
  - Gaussian  
  - t-Student  
- **Simulation:** Monte Carlo (100,000 samples)  

---

## 🔧 Required R Libraries

```r
dplyr
quantmod
moments
ggplot2
gridExtra
fitdistrplus
nortest
copula
plotly
```
## 📊 Key Outputs

- Stock price time-series plots  
- Histograms with fitted normal curves  
- VaR & ES comparisons  
- Copula log-likelihood & AIC table  
- 2D density contour plots  
- 3D copula surface plots  
- Portfolio VaR & ES curves across weights  

---

## 🚀 How to Run

1. Clone the repository  
2. Open the `.Rmd` file in RStudio  
3. Ensure all packages are installed (see list above)  
4. Knit to HTML or run code chunks  

---

## 👥 Authors

- Oleksandra Krykun  
- Daryna Lycachenko  
- Tobiasz Jasiński  
