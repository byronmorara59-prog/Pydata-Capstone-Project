## Global Crude Oil Price Trends and Market Dynamics Analysis

### 1. Project Description
This project analyses how global crude oil prices have changed over time and what drives those changes. It examines the price behaviour of two key benchmarks — Brent and WTI — alongside related market indicators including natural gas prices, the US Dollar Index, and the S&P 500. The goal is to provide clear insights into price trends, volatility patterns, and the statistical relationships between oil and the broader economy. It combines data cleaning, feature engineering, and visualisation using the PyData ecosystem to present findings through a series of analytical charts and an interactive dashboard.



### 2. Problem Statement
Oil price movements affect nearly every aspect of daily life — from fuel and transport costs to inflation and government revenues — yet most people have no data-driven framework for understanding what causes these changes. Raw historical price data is publicly available but difficult to interpret without proper processing and context. This project aims to solve that by analysing historical crude oil price data to identify trends, highlight periods of extreme volatility, pinpoint the influence of geopolitical events, and support a clearer understanding of how global energy markets behave over time.



### 3. Proposed Features

1. Data integration — Fetch and merge oil price data, market indices, and currency data from yfinance alongside OPEC monthly production figures from an EIA CSV, selecting only relevant columns and aligning all sources to a consistent date index.

2. Trend analysis — Analyse how Brent and WTI prices change over time using rolling averages, annotated time-series line charts, and event markers highlighting key shocks such as the COVID-19 crash and the Russia-Ukraine war.

3. Volatility insights — Calculate daily percentage returns and rolling standard deviation to identify which periods experienced the most extreme price swings and how long elevated volatility lasted after each shock.

4. Comparative correlation analysis — Merge oil prices with the US Dollar Index, natural gas, and S&P 500 data to identify and quantify statistical relationships between oil and the broader market using a correlation matrix and heatmap.

5. Supply vs price analysis — Overlay EIA OPEC production volume data against price charts to examine whether production cut periods visibly correspond to upward price movements in the data.

6. Interactive dashboard — Visualise trends, rolling averages, volatility, and key insights using a Plotly interactive dashboard with a date range slider for exploring any period within the dataset.



### 4. Tools and Concepts
1. Pandas.

2. NumPy.

3. Matplotlib & Seaborn.

4. Plotly.

5. yfinance.



### 5. Data Sources
1. yfinance — market price data
Daily historical data for Brent crude (BZ=F), WTI crude (CL=F), natural gas (NG=F), the S&P 500 (^GSPC), and the US Dollar Index (DX-Y.NYB) fetched directly via Python. Data spans from 2018 to present with full OHLCV fields. Source: Yahoo Finance market data.

2. EIA — OPEC crude oil production
Monthly OPEC+ production volume figures in thousand barrels per day, downloaded as a single CSV. Data covers 2018 to present across major producing nations. Source: U.S. Energy Information Administration (eia.gov), free and publicly available.



### 6. Expected Insights
1. Which periods in the data saw the most extreme price crashes or spikes, and how long did recovery take?

2. Is there a consistent relationship between the US Dollar strength and oil prices in the data?

3. Do OPEC+ production cuts reliably translate into price increases, or does the market react before the official announcement?

4. How does oil price volatility in the 2022 war period compare statistically to the 2020 COVID crash?

5. Which market indicator — natural gas, the S&P 500, or the Dollar Index — has the strongest correlation with oil prices over this period?