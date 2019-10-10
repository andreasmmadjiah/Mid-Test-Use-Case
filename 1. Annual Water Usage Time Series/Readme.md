# Time Series Model ARIMA
<br>
<br>
We are using **ARIMA** model to forecast Baltimore's Annual Water. Our data has annual water in Baltimore ranging from 1885-1963. We divide this data into 2, dataset and validation. dataset will be further divided into train and test. validation for further analyze our performance. We EDA this data by plot it in time, and plot it by each decade. In this data, there are no null values and duplicate but it's not stationer in mean, and in variance. We use differencing to make it stationer in mean. We also plot ACF and PACF to determine order in ARIMA, and also search manualy by finding which order produce best Mean squared error for our test data. In the end, we forecast and compare our prediction to validation.csv
<br><br>
We are valdiate our model performance by using iteration, that is for example there are 50 train, and 50 test. First we train ARIMA model to 50 train and forecast 1 year ahead it. Then we store the prediction in other variable. Then we train 51 train, to predict one year ahead it. Iterate until we train 100 train.
<br><br>
Using ARIMA model, we find decent result to predict our dataset. This could be caused by there are random outlier or fluctuation in our data, probably caused by seasonal. 
