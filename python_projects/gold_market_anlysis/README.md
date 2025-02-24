# **Gold Market Analysis: Data Sources and Methodology**

## **Introduction**
This project analyzes gold market trends by integrating financial and macroeconomic data to uncover key insights into price movements and influencing factors. The analysis involves data extraction, processing, statistical modeling, and visualization to enhance the understanding of the dynamics affecting gold prices. 

---

## **Data Sources**
Multiple data sources are leveraged to construct a comprehensive dataset, including:
- **Yahoo Finance (`yfinance` Python library)** for market price retrieval.
- **Federal Reserve Economic Data (`FRED` API)** for macroeconomic indicators.
- **Locally stored Excel files** containing historical gold price data.

---

## **1. Gold Price Data**
Historical gold spot price data is obtained from Excel files, covering the period from January 1, 2023, to February 20, 2025. The following preprocessing steps are applied:
- The dataset is imported into a Pandas DataFrame.
- The date column is converted to `datetime` format and set as the index.
- The dataset is filtered to include only records from January 1, 2024, onward for a more focused analysis.

---

## **2. Macroeconomic Indicators from FRED**
To assess external economic influences on gold prices, key macroeconomic indicators are retrieved via the FRED API:
- **Consumer Price Index (CPIAUCSL)**: Measures inflation and impacts gold’s role as an inflation hedge.
- **10-Year Treasury Yield (DGS10)**: Represents the risk-free rate, influencing investor decisions between gold and bonds.
- **Yield Curve Spread (T10Y2Y)**: Measures economic outlook via the difference between 10-year and 2-year Treasury yields.

To maintain data consistency:
- Indicators are resampled to a daily frequency.
- Forward-filling is applied to handle missing values.
- A uniform time range is enforced across datasets.

---

## **3. Methodology**
### **Data Preprocessing**
To ensure high data quality, the following steps are taken:
- Missing values are handled using forward-filling.
- Data types are standardized for computational efficiency.
- A consistent time range is maintained across datasets.  

---

### **Statistical and Technical Analysis**
To analyze gold price trends and volatility, several statistical and technical indicators are applied:

- **Bollinger Bands & Average True Range (ATR)**: Measure price volatility.  
- **Relative Strength Index (RSI)**: Identifies overbought or oversold conditions.  
- **Moving Averages (MACD & SMA)**: Detect trend direction and momentum.  
- **GARCH Model (Generalized Autoregressive Conditional Heteroskedasticity)**: Analyzes volatility clustering and future uncertainty.  

---

### **4. Data Visualization**
The following charts provide an intuitive and comprehensive visual representation of gold market trends:

1. **Gold Price Trends**  
   A time-series line chart tracks gold price movements, marking key events and trend shifts.  

2. **Macroeconomic Correlations**  
   A heatmap illustrates correlations between gold prices and economic indicators, such as CPI, treasury yields, and the yield curve spread.  

3. **Volatility Analysis**  
   Bollinger Bands and ATR overlays provide a direct visualization of price volatility and trend strength.  

4. **Momentum and Trend Detection**  
   RSI and MACD are plotted in separate subplots to highlight market reversals and momentum shifts.  

5. **GARCH Model Forecasts**  
   A volatility forecast chart identifies periods of high and low price uncertainty, helping assess potential risks.  

Aesthetic considerations include:
- Consistent color schemes for clarity.  
- Dual-axis charts to compare multiple variables without overwhelming the audience.  
- Seaborn and Matplotlib used for enhanced visual appeal and exploratory analysis.  

---

## **Conclusion**
This project integrates macroeconomic and financial data to provide a comprehensive view of the gold market. Future enhancements include:
- Machine learning integration for predictive modeling of gold price movements.  
- Expanded economic indicators, including geopolitical risk factors.  
- Market commentary incorporating both quantitative findings and personal observations, to be published on my LinkedIn <https://www.linkedin.com/in/chloehan24nw>.  
