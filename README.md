# Financial-Forecasting-with-ARIMA-Model
Financial Forecasting - ARIMA Model

Introduction
This code is designed to help forecast future sales data using the ARIMA (AutoRegressive Integrated Moving Average) time series model. It uses the pmdarima library to automatically determine the optimal parameters for the ARIMA model and then fits the model to the provided sales data. Finally, it generates a forecast for future sales data.

Requirements
To run this code, you need to have the following libraries installed:

pandas
matplotlib
statsmodels
pmdarima
You also need to have a CSV file containing your sales data with the following columns:

Month: the date of each monthly sales data point
Sales: the sales data for each month
Usage
Install the required libraries.
Save your sales data as a CSV file with the correct format.
Update the path to your CSV file in the sales_data variable.
Run the code.
The code will generate two plots:

The first plot shows the original sales data over time.
The second plot shows the original sales data and the forecasted sales data for the next 12 months.
Output
The code outputs the following:

A summary of the optimal ARIMA parameters determined by the auto_arima function.
The forecasted sales data for the next 12 months.
Disclaimer
Please note that forecasting future sales data is not an exact science and there are many factors that can affect sales. Therefore, the forecasted sales data should be used as a guide only and not as a guarantee of future sales.
