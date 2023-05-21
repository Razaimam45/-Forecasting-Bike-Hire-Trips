# Forecasting-Bike-Hire-Trips

The workflow of this project: Initaly loads ride data from a set of CSV files from 2014-2017, creates a Cartesian product of dates, start station, and end station, filters for the most connected station pairs, and groups the data by station pair and date to compute the number of rides and median ride duration per day. Then I select a specific station pair and fits a Prophet model to forecast the number of rides for the next seven days. The model is then cross-validated using a rolling window approach with a horizon of seven days and a period of five days. Performance metrics including RMSE and MSE are then computed based on the cross-validation results. Finally, for visualization the forecast is plotted. The approach I used in this project is basically a standard workflow for time series forecasting using the Prophet library, including data preparation, model fitting, and evaluation.
