# Arbitrage Opportunity Detector

This Python script is designed to identify potential arbitrage opportunities between a stock index (e.g., S&P 500) and its corresponding futures contract. The script utilizes historical price data to calculate volatility, identify spreads, and highlight potential long or short arbitrage opportunities.

## Prerequisites

Before running the script, make sure you have the following libraries installed:

- pandas
- yfinance
- matplotlib

You can install these dependencies using the following:

```bash
pip install pandas yfinance matplotlib
```

## Usage

1. Import the necessary libraries:

```python
import pandas as pd
import yfinance as yf
import matplotlib.pyplot as plt
from datetime import datetime, timedelta
```

2. Define the fee structure for each asset in the `fees` dictionary. This includes the minimum spread and margin percentage.

3. Adjust the `threshold_multiplier` based on your risk tolerance.

4. Run the script.

```python
python arbitrage_opportunity_detector.py
```

The script will fetch historical data, calculate volatility, identify arbitrage opportunities, and display a plot highlighting potential opportunities. Descriptive output includes the number of opportunities and the dynamic historical window.

## Output

The script provides a visual representation of the index and futures prices along with markers indicating long or short arbitrage opportunities. Additionally, it outputs the number of opportunities and the current arbitrage situation.

Feel free to customize the script based on your specific needs and risk preferences.