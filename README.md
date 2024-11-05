
# Options Analysis Project

This project is an in-depth study on Vanilla, Non-Vanilla, and Exotic options, conducted to model and visualize the payoffs, profit, and risk associated with each option style across multiple stocks and global exchange markets. We select three stocks from different sectors to diversify the analysis and implement various quantitative models in Python, including the Black-Scholes formula, Monte Carlo simulations, and sensitivity analysis through the Greeks, to evaluate and compare options under differen...

## Project Overview

### 1. **Data Collection**
   - Using `yfinance`, we fetch real-time stock and options chain data for three specified tickers (Tesla, Apple, and Johnson & Johnson) from different sectors and a common expiration date.
   - This data provides key inputs like the underlying asset price, strike price, historical volatility, and current option prices.

### 2. **Options Pricing Models**
   - **Vanilla Options**:
     - The Black-Scholes model is used to calculate theoretical prices for European call and put options.
   - **Exotic Option (Asian Option)**:
     - A Monte Carlo simulation is employed to model an Asian option, where the payoff is based on the average price of the underlying asset over time. This simulation generates multiple paths to compute the expected payoff.

### 3. **Greeks Calculation**
   - The Greeks (Delta, Gamma, Vega) are calculated to assess the sensitivity of option prices to changes in factors such as asset price, volatility, and time. This provides insights into risk management and the impact of market movements on option values.

### 4. **Payoff Tables and Visualizations**
   - **Vanilla Payoffs**: Payoff tables and plots are created for Vanilla call and put options for each selected stock, showing how profits or losses vary across different underlying prices.
   - **Exotic Payoffs**: The project also models the payoff for an Asian option, adding a comparison to showcase the differences in profit structures.
   - **Comparative Plot**: The code visualizes the payoffs for both Vanilla and Exotic options, highlighting their unique profit-risk characteristics.


### 5. **Risk-Return Analysis**
   - Using the Sharpe Ratio, the project evaluates the risk-adjusted return for holding each option, providing a quantitative measure of profitability against market volatility.

### 6. **Global Market Comparison**
   - The project compares Exotic option prices across global markets (e.g., US, Europe, Asia) by adjusting the volatility for each market and running separate simulations. This section highlights how geographic and economic factors influence option pricing.

### 7. **Advanced Visualizations**
   - **3D Surface Plot**: The code includes a 3D plot to show how Greeks like Delta vary with the underlying price and time to maturity.
   - **Probability Distribution of Returns**: A histogram with a probability density function (PDF) illustrates the distribution of expected returns, providing an intuitive view of risk.

## How to Run the Code

1. Clone the repository or download the `.ipynb` file.
2. Install necessary packages:
   ```bash
   pip install yfinance matplotlib numpy scipy pandas
   ```
3. Open the notebook in Google Colab or Jupyter and run each cell sequentially.


## Key Takeaways

This project provides a comprehensive view of options pricing and risk modeling by:
   - Comparing traditional and exotic options using different payoff and pricing models.
   - Using Monte Carlo simulations to account for stochastic behaviors in exotic options.
   - Visualizing how market conditions, risk factors, and geographic locations impact option values.

This project can be expanded further by including additional exotic options (like barrier or lookback options), implementing more sophisticated models (e.g., Heston or GARCH), and exploring machine learning techniques for predictive pricing.
