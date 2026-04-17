## Global Crude Oil Price Trends and Market Dynamics Analysis

### 1. Project Description
This project analyses how global crude oil prices have changed over time and what drives those changes. It examines the price behaviour of Brent crude, the world's primary oil benchmark, alongside related market indicators including natural gas prices and the US Dollar Index. The goal is to provide clear insights into price trends, volatility patterns, and the statistical relationships between oil and the broader economy. It combines data cleaning, feature engineering, and visualisation using the PyData ecosystem to present findings through a series of analytical charts and an interactive dashboard.



### 2. Problem Statement
Oil price movements affect nearly every aspect of daily life, from fuel and transport costs to inflation and government revenues, yet most people have no data-driven framework for understanding what causes these changes. Raw historical price data is publicly available but difficult to interpret without proper processing and context. This project aims to solve that by analysing historical Brent crude oil price data to identify trends, highlight periods of extreme volatility, pinpoint the influence of geopolitical events, and support a clearer understanding of how global energy markets behave over time.



### 3. Proposed Features

1. Data integration — Fetch and merge Brent crude price data, market indices, and currency data from yfinance, selecting only relevant columns and aligning all sources to a consistent date index.

2. Trend analysis — Analyse how Brent crude prices change over time using rolling averages and annotated time-series line charts highlighting key shocks such as the 2008 financial crisis, the 2015–16 supply glut, the COVID-19 crash, and the Russia-Ukraine war.

3. Volatility insights — Calculate daily percentage returns and rolling standard deviation to identify which periods experienced the most extreme price swings and how long elevated volatility lasted after each shock.

4. Comparative correlation analysis — Merge Brent prices with the US Dollar Index and natural gas data to identify and quantify statistical relationships between oil and these market indicators using a correlation matrix and heatmap.

6. Interactive dashboard — Visualise trends, rolling averages, volatility, and key insights using a Plotly interactive dashboard with event markers and a date range slider for exploring any period within the dataset.



### 4. Tools and Concepts
1. Pandas.

2. NumPy.

3. Matplotlib & Seaborn.

4. Plotly.

5. yfinance.



### 5. Data Sources
1. yfinance — market price data. Daily historical data for Brent crude (BZ=F), natural gas (NG=F), and the US Dollar Index (DX-Y.NYB) fetched directly via Python. Data is from July 2007 to December 2025.


### 6. Expected Insights
1. Which periods in the data saw the most extreme Brent price crashes or spikes, and how long did recovery take?

2. Is there a consistent relationship between US Dollar strength and Brent crude prices in the data?

3. How does Brent price volatility during the 2022 Russia-Ukraine war compare statistically to the 2020 COVID crash and the 2008 financial crisis?

4. Which market indicator — natural gas or the US Dollar Index — has the strongest correlation with Brent crude prices over this period?