# Riding request Prediction for Rapido
Each time a customer has requested a ride,her/his pickup and drop location is recorded with exact date and time.Now based on this we want to predict the number of ride request for future.

1.Used google colab for GPU computation and make the runtime very fast as the size of the data is around 550Mb,which is pretty large.

2.Firstly,made a nice looking map using folium library inorder to get an idea that what are the key areas where riding requests was given.

3.Secondly,some feature engineering is done.Using kmean clustering(the number of cluster was decided on the basis of the webmap),we differentiates different positions where riding request was given by customers.

4.After making clusters,for each cluster the exploratory data analysis was done.Decomposed the time series into trend,seasonal and stationary part.Then checked for the stationarity.After doing all this we have used deep learning model LSTM for the forecasting purpose.
