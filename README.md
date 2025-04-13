# Time Series Forecasting of Major Indian Stocks using Meta Prophet

## Objective  
This project aims to **forecast the closing prices of some of India’s most influential companies over the next 30 days** using **Meta’s Prophet** time series forecasting model. In today's volatile economic environment shaped by global events, policy changes, and market cycles this project provides a robust tool for short-term forecasting and long-term investment analysis.

The study combines deep historical analysis with machine learning to uncover patterns, volatility trends, and stock-specific behaviors between **January 1, 2020 and April 10, 2025**. It also evaluates how a diversified portfolio of these companies would have performed over the last 5 years and projects what the next month may look like for investors.

---

## Tech Stack  
- **Python**  
- **Prophet (by Meta)**  
- **Pandas, NumPy** for data manipulation  
- **Matplotlib, Seaborn, Plotly** for visualization  
- **yFinance** for stock data retrieval  
- **Jupyter Notebook** for analysis workflow

---

## Companies Analyzed  
The following Indian companies were selected for their significance in the stock market and influence in the economy:

- **Tata Consultancy Services (TCS)**  
- **Infosys**  
- **HDFC Bank**  
- **Bharti Airtel**  
- **State Bank of India (SBI)**  
- **Tata Motors**  
- **Reliance Industries**

---

## General Observations (2020–2025)

### Market Events & Trends  
- **Sharp decline in early 2020** due to the COVID-19 crash.  
- **2021–2023 marked a recovery phase**, with most companies rebounding steadily.  
- In **early 2025**, many stocks (TCS, Infosys, Tata Motors) faced corrections, possibly triggered by Trump-era tariffs and economic policy shifts.

### Stock-Specific Insights  
- **TCS** maintained the highest stock price, peaking near ₹4500 before correcting in 2025.  
- **Infosys** and **Airtel** showed strong long-term growth and steady uptrends.  
- **Tata Motors** and **SBI** saw strong upward momentum post-2021 but remained volatile.  
- **HDFC** exhibited the **most stable** growth, ideal for low-risk portfolios.  
- **Reliance** grew consistently, supported by diversification into retail and digital sectors.

---

## Volatility Analysis  

### Daily Returns  
- High volatility across all stocks in early 2020 during the pandemic crash.  
- Post-2021: Most companies showed **stabilized return patterns**.  
- **Tata Motors** showed the **highest daily return swings**, indicating risk.  
- **HDFC**, **TCS**, and **Infosys** displayed relatively **stable return profiles**.

### Rolling Volatility (30-Day Window)  
- Massive volatility spikes in 2020 (6–7%) for most companies.  
- Post-2022: Volatility for most stocks converged around **1–2%**, indicating market stabilization.  
- **Tata Motors** and **SBI** had periodic volatility spikes due to market sensitivity.  
- **HDFC** maintained the **lowest rolling volatility**, highlighting its conservative nature.

---

## Portfolio Performance (Equal-Weighted)

### Key Metrics  
- **Annualized Return**: 20.03%  
- **Annualized Volatility**: 20.74%  
- **Sharpe Ratio**: 0.97  

### Insights  
- Strong long-term growth across the portfolio.  
- Portfolio stayed resilient during crashes and corrections.  
- Equal weighting helped maintain balance between aggressive and defensive stocks.  
- Noticeable portfolio correction in early 2025 aligns with observed stock-specific dips.

---

## Stock vs. Nifty 50 (2020–2025)

- **Tata Motors** delivered the **highest return**, especially from 2022 to 2024.  
- **Airtel** and **Infosys** **outperformed** the Nifty 50 index consistently.  
- **Reliance** and **TCS** grew steadily but closely tracked the index.  
- **HDFC** underperformed the index but offered the most consistent returns.  
- **SBI** showed strong mid-period growth but higher fluctuations.  
- The **Nifty 50** served as a reliable benchmark for market trends and relative performance.

---

## Forecasting with Prophet

### Why Prophet?  
Prophet, developed by Meta, is designed for accurate forecasting of time series data with strong seasonal effects and multiple trend changepoints. Features include:

- Automatic detection of **weekly, monthly, and yearly seasonality**  
- Handles **missing values and outliers**  
- Provides **interpretable trend and uncertainty intervals**  
- Allows for future forecasting even with limited historical data  

### Forecast Workflow  
- Trained a separate Prophet model for each company using the `ds` (date) and `y` (closing price) format.  
- Generated **30-day future forecasts** from April 10, 2025.  
- Visualized forecasts and decomposed trends using `plot_components()` to understand seasonal behavior.  

---

## Final Takeaways  
- **HDFC, Infosys, and TCS** are ideal for low-volatility, long-term investment strategies.  
- **Tata Motors** and **SBI** offer high reward but come with higher risk.  
- **Forecasts can be used for short-term positioning and swing trading** based on the next 30 days of expected movement.  
- Prophet performs well in handling complex, real-world time series data like stock prices.  
- A data-driven strategy significantly enhances portfolio decision-making in unpredictable market conditions.

---

## How to Use  
1. **Clone the repository**  
   ```bash  
   git clone https://github.com/Mindmasterparav/Finance.git
  
