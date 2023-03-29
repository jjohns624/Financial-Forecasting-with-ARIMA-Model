# Time Series forecasting with ARIMA
This project demonstrates time series forecasting with ARIMA (Autoregressive Integrated Moving Average) using Python. The steps for building the ARIMA model are as follows:

# Step 1: Read the Data
The first step is to read the historical sales data into a pandas DataFrame. The data is read from a CSV file and parsed as dates, with the date column set as the index.

# Step 2: Resample the Data
The data is resampled to a monthly frequency by aggregating daily sales. This is necessary for ARIMA modeling as the model requires a stationary series.

# Step 3: Stationarity Check
The stationarity of the data is checked using the augmented Dickey-Fuller (ADF) test and seasonal decomposition of time series. The data is found to be seasonal and requires seasonal ARIMA modeling.

# Step 4: Train Test Split
The data is split into training and testing sets for model evaluation. The first 64 months are used for training and the remaining data is used for testing.

# Step 5: Hyperparameters of ARIMA model - p d q
The hyperparameters for the ARIMA model are selected using three different methods: ACF (Autocorrelation Function) and PACF (Partial Autocorrelation Function) plots, AUTO_ARIMA function, and for loop.

# Step 6: Build ARIMA model
The ARIMA model is built using the selected hyperparameters and trained on the training data.

# Step 7: Predict test dataset
The model is used to forecast sales for the testing period.

# Step 8: Model Evaluation
The model's performance is evaluated by calculating the root mean squared error (RMSE) between the actual and predicted sales. The RMSE is compared to the mean and standard deviation of the testing set. The predictions and actual values are also plotted for visual evaluation.
