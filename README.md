# Moving Average Crossover Strategy

## Code Overview

This project implements a Moving Average Crossover Strategy using historical stock data paired with Relative Strength Indexes. This project contains 2 inplementations using this strategy, one provides buy and sell signals for a single stock and another applies the same strategy to all SP500 stocks.

The main tasks performed by the code are:

1. **Installs necessary libraries**:
   - `pandas`
   - `numpy`
   - `matplotlib`
   - `yfinance`

2. **Imports necessary libraries**:
   - `pandas` for data manipulation
   - `numpy` for numerical operations
   - `matplotlib.pyplot` for plotting
   - `yfinance` for fetching historical stock data

3. **Loads stock tickers**:
   - Reads a list of stock tickers from a CSV file named `spx.csv`.

4. **Defines a date range**:
   - Start date: August 13, 2021
   - End date: August 13, 2024

5. **Fetches historical stock data**:
   - Defines a function `fetch_data` to retrieve historical stock data for each ticker using the `yfinance` library.
   - Calls the `fetch_data` function to retrieve and store the data in a dictionary.

6. **Implements the Moving Average Crossover Strategy**:
   - Calculates short-term and long-term moving averages for the stock prices.
   - Identifies buy and sell signals based on the crossover of these moving averages.

7. **Plots the results**:
   - Uses `matplotlib` to visualize the stock prices along with the moving averages and the buy/sell signals.
