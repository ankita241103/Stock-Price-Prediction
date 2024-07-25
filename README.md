# Stock Price Prediction

The stock price prediction project employs the ARIMA (AutoRegressive Integrated Moving Average) model to forecast future stock prices. The project utilizes Python for comprehensive data analysis and prediction tasks. The dataset includes stock price information and is used to build, train, and evaluate the ARIMA model, with an emphasis on parameter optimization and the integration of exogenous variables.

## Dataset
The dataset consists of stock price data with the following columns:
- Date: The date of the stock price observation.
- Open: The opening price of the stock on the given date.
- High: The highest price of the stock on the given date.
- Low: The lowest price of the stock on the given date.
- Close: The closing price of the stock on the given date.
- Volume: The number of shares traded on the given date.
- Strategy: A column representing strategy to Hold, Buy or Sell stock.

## Project Structure

### 1. Data Loading and Preprocessing
- Data is loaded from a CSV file and preprocessed to extract relevant features and time series attributes.
- The dataset comprises columns such as Date, Open, Close, Volume, and additional exogenous variables.

### 2. Exploratory Data Analysis (EDA)
- Time series plots for stock prices (Open, Close) and trading volume are generated to understand trends and seasonal behaviors.
- Statistical summaries and distributions of numerical columns are analyzed.
- Correlation heatmaps are used to identify relationships between features.

### 3. Feature Engineering
- Lagged features and moving averages are created to enhance the model's ability to capture temporal dependencies.
- The dataset is augmented with lagged values and moving averages for Open and Volume to improve predictive performance.

### 4. Model Building and Training
- The ARIMA model is implemented to forecast stock prices based on historical data.
- The auto_arima function from the pmdarima library is used to optimize model parameters, including p, d, and q.
- Exogenous variables, including lagged values and moving averages, are integrated into the model to capture additional predictors.

### 5. Prediction and Evaluation
- Model predictions are compared against actual values using performance metrics such as Mean Squared Error (MSE) and Mean Absolute Error (MAE).
- A summary of the ARIMA model is provided, including parameter estimates and diagnostics.
- Results are visualized with plots comparing predicted and actual stock prices.

## Key Components

- Python Libraries: Pandas, NumPy, Matplotlib, Seaborn, Statsmodels, pmdarima
- Datasets: Historical stock price data, including features like Open, Close, Volume
- Models: ARIMA, optimized using auto_arima for parameter tuning
- Metrics: Mean Squared Error (MSE), Mean Absolute Error (MAE)

