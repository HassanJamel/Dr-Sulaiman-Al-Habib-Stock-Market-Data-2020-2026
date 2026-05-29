
<p align="center">
  <a href="https://www.kaggle.com/code/hassanjameelahmed/dr-sulaiman-al-habib-stock-market-data-2020-2026"target="_blank">
    <img src="HMG-Stock-Data-Analysis-2026.png" alt="dr-sulaiman-al-habib" alt="dr-sulaiman-al-habib" width="600">
  </a>
</p>
<br>



# Project Requirements Document (PRD)

## Project Overview
This document serves as the official Kaggle Project Requirements Document (PRD) for the **Dr. Sulaiman Al Habib Medical Services Group Company** dataset. It outlines the dataset's structure, metadata, scope, and potential analytical applications.

---

## d. SEO-Optimized Project Name and Description

**Project Name:** Dr. Sulaiman Al Habib Medical Services Group Historical Stock Data (2020-2026)

**Project Description:** 
Unlock comprehensive historical stock market data for Dr. Sulaiman Al Habib Medical Services Group Company (Tadawul: 4013), a premier private healthcare provider in Saudi Arabia. This high-quality dataset features daily trading information—including Open, High, Low, Close prices, and Trading Volume—from the company's IPO in March 2020 through early 2026. Ideal for financial analysts, data scientists, and quantitative researchers focusing on time series forecasting, algorithmic trading, and Middle Eastern healthcare sector analysis.

---

## c. Top 5 Kaggle Tags
1. `Finance`
2. `Healthcare`
3. `Stock Market`
4. `Time Series`
5. `Saudi Arabia`

---

## b. Dataset Columns and Details

The dataset provides a structured daily summary of the stock's trading activity. 

| Column Name | Data Type | Description |
| :--- | :--- | :--- |
| **Date** | Date/String | The date of the trading session (Format: MM/DD/YYYY). |
| **Close** | Float | The last price at which the stock traded during the regular trading day (in SAR). |
| **High** | Float | The highest price at which the stock traded during the trading day. |
| **Low** | Float | The lowest price at which the stock traded during the trading day. |
| **Open** | Float | The initial price at which the stock traded upon the opening of the market. |
| **Volume** | Integer | The total number of shares traded during the trading day. |

---

## e. Dataset Coverage
This dataset comprehensively covers the daily stock trading history of Dr. Sulaiman Al Habib Medical Services Group on the Saudi Stock Exchange (Tadawul). It reflects the financial performance, market valuation, and investor sentiment regarding one of the most prominent healthcare operators in the Middle East over a significant multi-year period.

---

## f. Temporal and Geospatial Scope

* **Start Date:** 03/17/2020 (Coinciding with the company's Initial Public Offering)
* **End Date:** 01/29/2026
* **Geospatial Scope:** Riyadh, Saudi Arabia (Data originates from the Tadawul Stock Exchange).

---

## g. Data Provenance
The raw data originates directly from the **Saudi Stock Exchange (Tadawul)**. It is typically routed through major global financial data aggregators (such as Yahoo Finance, Bloomberg, or Investing.com). 

**Transformations:** To make the data highly reusable for machine learning and data science workflows, the data was parsed into a standardized tabular CSV format. Dates were formatted uniformly to `MM/DD/YYYY`, and pricing columns were verified for consistent float representations.

---

## h. Dataset Collecting Methodology
The dataset was aggregated using automated financial data extraction techniques. The methodology involved querying historical financial APIs or securely scraping structured tables from trusted financial market platforms. After extraction, the data underwent a cleaning pipeline to remove any non-trading days (weekends/holidays) and to ensure that all numeric fields (prices and volume) were correctly parsed and free of anomalies.

---

## i. Biggest Problems and Challenges Facing This Project
1. **Handling Corporate Actions:** Stock prices can be artificially affected by stock splits, reverse splits, or dividend payouts. Ensuring the data is accurately "adjusted" for these events over a 6-year period is crucial for accurate analysis.
2. **Market Volatility & Exogenous Shocks:** The dataset begins in March 2020, right at the onset of the COVID-19 pandemic. Models trained on this data must account for extreme market anomalies and shifting healthcare regulations that heavily influenced investor behavior.
3. **Time Series Non-Stationarity:** Financial data is notoriously noisy and non-stationary. Building robust, predictive machine learning models that can generalize future stock movements without overfitting on past trends is a significant data science challenge.

---

## j. Dataset Source
* **Correct Source:** Saudi Stock Exchange (Tadawul) / Yahoo Finance Historical Data.
* **Source Link:** [Saudi Exchange - Company Profile (4013)](https://www.saudiexchange.sa/wps/portal/saudiexchange/hidden/company-profile-main/!ut/p/z1/04_Sj9CPykssy0xPLMnMz0vMAfIjo8ziTR3NDIw8LAz83d2NXA0C3SydAl1c3Q0NvE30I4EKzBEKDEJDnDICzbEKDHK2cDA0B1I_Sk_HqqI8KydVPz9cP1o_CrMivxR_H-N4_SjEKkE2BAA15E84/) | [Yahoo Finance (if applicable)](https://finance.yahoo.com/)

---

## k. How the Problem Developed (Step by Step)

1. **Initial Public Offering (IPO):** Dr. Sulaiman Al Habib Medical Services Group went public on the Saudi Exchange in March 2020. This generated the very first data points in our dataset.
2. **Daily Market Generation:** During every active trading session from 2020 to 2026, market forces (buyers and sellers) dictated the open, high, low, and close prices, alongside the total volume of shares exchanged.
3. **Data Aggregation:** Financial institutions and exchanges recorded these daily metrics, creating a continuous historical ledger.
4. **Data Science Application:** As the historical ledger grew, analysts identified a need to compile this unstructured or dispersed data into a single, clean CSV file. 
5. **Project Inception:** The need for comprehensive technical analysis, algorithmic trading backtesting, and healthcare sector performance evaluation led to the creation of this Kaggle dataset. It provides the structured foundation necessary to answer complex financial questions and forecast future market trends.
