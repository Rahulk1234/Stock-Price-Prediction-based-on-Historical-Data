# Stock-Price-Prediction-based-on-Historical-Data!


**Predictive Analysis of Stock based on Historical Data in Python
The models used are LSTM Model and ARIMA.**

Data is dynamically taken from _Yahoo Finance. _

The program ask you to enter the Stock Ticker, Start Date and End Date for analysis. Based on your input it will download the historical data from Yahoo Finance.

At first, the program will split the data as 70%-train and 30%-test. I have trained the LSTM model by adding dense=1(1 layer) and lookback is 60. While fitting the epocs are set as 50. Loss function value initially is high but it reduces down and as set epoch 50 to get a better loss function value.


Plotly graphs are used for plotting the time series. You can see




Close values plotted:

![image](https://user-images.githubusercontent.com/26666702/149738808-0a7c2490-be19-4353-bcdc-82a5052076e4.png)


Results of LSTM Model: 
The red line are the predictions and green is the original close. As we can see from the graph, the predictions are closer to the original close values.

![image](https://user-images.githubusercontent.com/26666702/149738994-5d9597f9-dd50-401e-bcae-97f79c364f3f.png)



Root Mean Square Error and R2 Score values for the LSTM Model.

![image](https://user-images.githubusercontent.com/26666702/149739243-fdf6a966-d527-4bb2-9bbf-56b44f0ab750.png)




**ARIMA Model**

I have used ARIMA(4,1,2) Model for forecasting the future values.

These are ARIMA predictions
![image](https://user-images.githubusercontent.com/26666702/149740454-68153ddd-bdeb-41e9-9b4f-0520ff8ad09b.png)


Forecasting using ARIMA
![image](https://user-images.githubusercontent.com/26666702/149740604-73780fd0-3b61-4d0f-9c0a-7030a5784fe8.png)


Results Summary for ARIMA 
![image](https://user-images.githubusercontent.com/26666702/149740735-6f16dd50-7be5-4ed6-abd2-8c689e819a96.png)


Forecasting plotted using plotly graph after taking inverse trasform of the predictions from the results of ARIMA Model

![image](https://user-images.githubusercontent.com/26666702/149741034-3d108e80-35c3-4ada-a698-7f24fe14c954.png)



You can compare both and check LSTM and ARIMA. In this scenario I have used Tesla Stock but as I said the program will ask you initially which stock do you want to consider, you can enter the stock ticker value of your desired stock.


_**Thankyou**_
