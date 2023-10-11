Observations and explanations from our assignment:


--There is an increase in the bike rental count in spring and summer season , and then decrease in the bike rental count in fall and winter season.

--The bike rental count distribution is higher in 2019 than in 2018.

--During no holidays, the bike rental counts is the highest, compared to during holidays for different seasons.

--There is no significant change in bike demand with working days and non working days.

--During clear, partly cloudy weather, the bike rental count is the highest, second-highest during misty cloudy weather, and followed by 3rd highest, during light snow and light rain weather.

Outlier analysis:
(i) No outliers are present in total_count variable.<br>
(ii) No outliers are present in normalized temp but few outliers are present in normalized windspeed and humidity variables.

For modelling the datset, we split the dataset into train and test in the ratio of 70:30.

Training dataset:
(i) While fitting Linear regression to our trained dataset, Accuracy of the model: 82.4 %<br>
(ii) Cross validation prediction plot tells about finite variance between actual target value and predicted target value. In our Cross validation prediction plot for training dataset, some data points are have same finite variance between them and some are not having it
(iii) Model Evaluation metrics: R-Squared (R² or the coefficient of determination) is a statistical measure in a regression model that determines the proportion of variance in the dependent variable that can be explained by the independent variable.The R-squared or coefficient of determination for our model is 0.81 on average , it means that predictor is only able to predict 81% of the variance in the target variable which is contributed by independent variables.

Testing dataset:
(i) Model Evaluation metrics: Root Mean Square Error (RMSE) is the standard deviation of the residuals, and The mean absolute error of a model with respect to a test set is the mean of the absolute values of the individual prediction errors on over all instances in the test set.

For our model, 
Root mean square error : 802.4291866599553
Mean absolute error : 595.2441391283483
=========================================
Dataset characteristics
=========================================	
day.csv have the following fields:
	
	- instant: record index
	- dteday : date
	- season : season (1:spring, 2:summer, 3:fall, 4:winter)
	- yr : year (0: 2018, 1:2019)
	- mnth : month ( 1 to 12)
	- holiday : weather day is a holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)
	- weekday : day of the week
	- workingday : if day is neither weekend nor holiday is 1, otherwise is 0.
	+ weathersit : 
		- 1: Clear, Few clouds, Partly cloudy, Partly cloudy
		- 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
		- 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
		- 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
	- temp : temperature in Celsius
	- atemp: feeling temperature in Celsius
	- hum: humidity
	- windspeed: wind speed
	- casual: count of casual users
	- registered: count of registered users
	- cnt: count of total rental bikes including both casual and registered
	
=========================================
License
=========================================
Use of this dataset in publications must be cited to the following publication:

[1] Fanaee-T, Hadi, and Gama, Joao, "Event labeling combining ensemble detectors and background knowledge", Progress in Artificial Intelligence (2013): pp. 1-15, Springer Berlin Heidelberg, doi:10.1007/s13748-013-0040-3.

@article{
	year={2013},
	issn={2192-6352},
	journal={Progress in Artificial Intelligence},
	doi={10.1007/s13748-013-0040-3},
	title={Event labeling combining ensemble detectors and background knowledge},
	url={http://dx.doi.org/10.1007/s13748-013-0040-3},
	publisher={Springer Berlin Heidelberg},
	keywords={Event labeling; Event detection; Ensemble learning; Background knowledge},
	author={Fanaee-T, Hadi and Gama, Joao},
	pages={1-15}
}

=========================================
Contact
=========================================
	
For further information about this dataset please contact Hadi Fanaee-T (hadi.fanaee@fe.up.pt)
