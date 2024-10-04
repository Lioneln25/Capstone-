# Financial Market Characteristics Analysis: Volatility, Liquidity, and Correlation

## Overview

This project analyzes key financial market characteristics—volatility, liquidity, and asset correlations—across major stock indices: NASDAQ, S&P 500, and Dow Jones Industrial Average (DJIA) from 2015 to 2024. By leveraging historical market data and Python-based data analysis tools, this project provides insights into the dynamics of financial markets, aiding investors, analysts, and policymakers in understanding market behavior during various economic periods.

## Features

- Volatility Analysis: Computes and visualizes the rolling 30-day volatility for each index.
- Liquidity Analysis: Analyzes trading volumes to approximate market liquidity.
- Correlation Analysis: Provides a correlation matrix to understand relationships between NASDAQ, S&P 500, and DJIA indices.
- Visualizations: Generates clear and informative charts to display volatility, liquidity, and correlation trends.
- Granger Causality Test: (Optional) Investigates whether changes in liquidity lead to changes in volatility.

## Table of Contents

1. [Project Setup](#project-setup)
2. [Data Sources](#data-sources)
3. [How to Use](#how-to-use)
4. [Dependencies](#dependencies)
5. [Key Concepts](#key-concepts)
6. [Future Improvements](#future-improvements)
7. [License](#license)

## Project Setup

### Clone the Repository

```
git clone https://github.com/your-username/financial-market-analysis.git
cd financial-market-analysis
```

### Install the Required Packages

Ensure Python is installed on your system. To install the necessary libraries, run the following command:

```
pip install -r requirements.txt
```

This will install all required dependencies listed in the `requirements.txt` file.

## Data Sources

This project uses financial data from Yahoo Finance. The data includes daily adjusted closing prices and trading volumes for the following indices:

- NASDAQ Composite (^IXIC)
- S&P 500 (^GSPC)
- Dow Jones Industrial Average (^DJI)

These indices represent major segments of the U.S. stock market, offering a broad view of market behavior from 2015 to 2024.

## How to Use

### Running the Analysis

1. Download Data: The script automatically fetches historical data using yfinance for the specified indices.
2. Perform Analysis:
   - Volatility: The script calculates rolling 30-day volatility for each index.
   - Liquidity: Approximates market liquidity using daily trading volume.
   - Correlation: Analyzes the relationships between the indices via a correlation matrix.
3. Generate Visualizations: Outputs charts for volatility, liquidity, and correlation.

To run the analysis, execute the following command:

```
python financial_market_analysis.py
```

### Output

The script generates three main outputs:
- Volatility Plot: Rolling 30-day volatility for each index.
- Liquidity Plot: Daily trading volumes as a proxy for liquidity.
- Correlation Heatmap: A heatmap displaying the correlation matrix between NASDAQ, S&P 500, and DJIA.

## Dependencies

This project uses the following Python libraries:
- yfinance: For retrieving historical market data from Yahoo Finance.
- pandas: For data manipulation and analysis.
- numpy: For numerical computations.
- matplotlib: For plotting charts.
- seaborn: For statistical data visualization and heatmaps.
- statsmodels: For advanced statistical tests, including Granger causality.

To install these dependencies manually, you can run:

```
pip install yfinance pandas numpy matplotlib seaborn statsmodels
```

## Key Concepts

- Volatility: Measures the degree of variation in stock prices over time. Higher volatility indicates more significant price fluctuations and higher risk.
- Liquidity: Refers to the ease of buying or selling an asset without causing significant price changes. Daily trading volume serves as a proxy for liquidity.
- Correlation: A statistical measure that indicates how two indices move in relation to each other. A positive correlation suggests that indices move in the same direction, while a negative correlation indicates opposite movements.
- Granger Causality Test: A statistical hypothesis test to determine whether one time series can predict another. This test helps understand the cause-effect relationships between liquidity and volatility.

## Future Improvements

There are several ways to extend this project:

- Incorporate Additional Indices: Add global stock market indices such as FTSE 100, DAX, or Nikkei to broaden the analysis.
- Sector-Specific Analysis: Break down the indices into individual sectors (e.g., technology, healthcare) to analyze sector-specific volatility and liquidity trends.
- Machine Learning Models: Implement machine learning algorithms (e.g., LSTM, Random Forest) to forecast volatility, liquidity, and correlation based on historical data.
- Event-Driven Volatility Analysis: Analyze how specific macroeconomic events (e.g., interest rate hikes, economic crises) impact the volatility and liquidity of the markets.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.
