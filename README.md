# Pairs Trading Strategy Implementation

## Overview

This repository contains a Python implementation of a Pairs Trading Strategy using a statistical arbitrage approach based on cointegration. The strategy identifies pairs of stocks that move together and generates trading signals based on their price spread and z-score.

## Features

- **Data Fetching**: Automatically fetches historical stock data for Nifty 100 stocks using the `yfinance` and `niftystocks` libraries.
- **Correlation and Cointegration Analysis**: Identifies highly correlated and cointegrated pairs of stocks.
- **Hedge Ratio Calculation**: Computes the hedge ratio for the selected pairs to optimize trading positions.
- **Signal Generation**: Generates trading signals based on the z-score of the price spread.
- **Backtesting**: Simulates trading based on historical data to evaluate the strategy's performance.
- **Performance Metrics**: Calculates key performance metrics such as CAGR, Sharpe Ratio, Sortino Ratio, and Maximum Drawdown.
- **Visualization**: Provides comprehensive visualizations of price movements, spread, z-scores, portfolio value, and performance metrics.

## Requirements

To run this code, you need to have the following Python packages installed:

- `numpy`
- `pandas`
- `yfinance`
- `niftystocks`
- `statsmodels`
- `quantstats`
- `matplotlib`
- `seaborn`

You can install the required packages using pip:

## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/pairs-trading-strategy.git
   cd pairs-trading-strategy
   ```

2. Open the Python script (e.g., `pairs_trading.py`) in your preferred IDE or text editor.

3. Modify the `start_date` and `end_date` parameters in the `main()` function to set the desired backtesting period.

4. Run the script:

   ```bash
   python pairs_trading.py
   ```

5. The script will fetch market data, identify correlated and cointegrated pairs, generate trading signals, backtest the strategy, and display performance metrics along with visualizations.

## Code Structure

- **PairsTrading Class**: Contains methods for fetching data, finding correlated and cointegrated pairs, calculating hedge ratios, generating signals, backtesting, and plotting results.
- **Main Function**: Initializes the PairsTrading class and executes the strategy steps.

## Example Output

The script will output the following:

- Selected pairs of stocks
- Trading signals
- Performance metrics (CAGR, Sharpe Ratio, etc.)
- Visualizations of price movements, spread, z-scores, and portfolio performance

## Contributing

Contributions are welcome! If you have suggestions for improvements or new features, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [yfinance](https://pypi.org/project/yfinance/) for fetching stock data.
- [niftystocks](https://pypi.org/project/niftystocks/) for Nifty stock tickers.
- [statsmodels](https://www.statsmodels.org/stable/index.html) for statistical tests.
- [quantstats](https://github.com/enzoampil/quantstats) for performance metrics.
- [matplotlib](https://matplotlib.org/) and [seaborn](https://seaborn.pydata.org/) for data visualization.
