# Time Series Forecasting with ARIMAX

In this project, we demonstrate how to perform time series forecasting using the ARIMAX model from the `statsmodels` library on the TSLA stock dataset.

## Dataset

The dataset (`TSLA_cleaned_v2.csv`) contains daily stock prices for Tesla from 2010 onwards with the following columns:

- **Date**: The date of the stock data.
- **Open**: Opening stock price.
- **High**: Highest stock price of the day.
- **Low**: Lowest stock price of the day.
- **Close**: Closing stock price.
- **Adj Close**: Adjusted closing stock price.
- **Volume**: Number of shares traded.

## Libraries Used

- [pandas](https://pandas.pydata.org/): For data manipulation and analysis.
- [statsmodels](https://www.statsmodels.org/stable/index.html): For statistical models, including the ARIMAX time series model.
- [sklearn](https://scikit-learn.org/): For evaluation metrics such as MAE, MSE, and RMSE.

## Process

1. **Data Preprocessing**:
   - Loaded the dataset into a pandas DataFrame.
   - Set the 'Date' column as the index and sorted the data chronologically.
   
2. **Data Splitting**:
   - Split the data into a training set (80%) and a test set (20%).
   
3. **Model Training**:
   - Used the ARIMAX model from `statsmodels` with 'Close' as the target variable and 'Open', 'High', 'Low', and 'Volume' as exogenous variables.
   
4. **Forecasting**:
   - Made forecasts for the test set.
   
5. **Evaluation**:
   - Calculated evaluation metrics (MAE, MSE, RMSE) to assess the accuracy of the forecasts.

## Results

The ARIMAX model provided forecasts for the test set, which were then compared with the actual values to evaluate the model's performance. Evaluation metrics such as MAE, MSE, and RMSE were computed to quantify the accuracy of the predictions.
