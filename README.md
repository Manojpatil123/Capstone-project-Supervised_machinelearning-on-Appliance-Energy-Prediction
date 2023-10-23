# Capstone-project-Supervised_machinelearning-on-Appliance-Energy-Prediction
Today's word usage of energy is increasing rapidly. Due to more usage of energy in some parts of the world, we are facing a lack of energy and it leads to environmental pollution. In some of the places, we are facing outrageous energy consumption in home appliances, so our main goal in this project is to analyse what the factors are affecting the increasing energy consumption of home appliances, how we can reduce the energy consumption of home appliances and predict energy consumption of appliances by using regression models

Problem statement:
________________________________________
The data set is at 10 min for about 4.5 months. The house temperature and humidity conditions were monitored with a ZigBee wireless sensor network. Each wireless node transmitted the temperature and humidity conditions around 3.3 min. Then, the wireless data was averaged for 10 minutes periods. The energy data was logged every 10 minutes with m-bus energy meters. Weather from the nearest airport weather station (Chievres Airport, Belgium) was downloaded from a public data set from Reliable Prognosis (rp5.ru) and merged together with the experimental data sets using the date and time column. Two random variables have been included in the data set for testing the regression models and to filter out non-predictive attributes (parameters).

Approach:

•	First, we load data set into Panda’s frame and initialize all the library which are required for doing EDA.

•	Then we did inspection of data on a basic level.

•	Then we did data cleaning by removing null values, duplicate values and outliers.

•	Then we used the matplotlib and seaborn to do Exploratory Data Analysis on sample data by plotting different graphs like count plot, pie chart, lmplot, bar plot, boxplot, subplot and heat map from this we got useful insights and correlation between target column and other features

•	In feature selection use variance threshold and F_Regression to select best features

•	In feature engineering check null values, removed outliers in the data set.

•	use multiple models to predict power consumption did hyper parameters tuning Random Forest regression is best model.

•	With model explain ability technique for knowing which features is important

Conclusion:         

•	Many columns in the dataset have not normally distributed and target column is also right skewed


•	Dataset has many outliers and no null values

•	We have hours column is high correlation with dependent variable and there are lot features have lesser than 0.1 correlation with dependent variable and its non-linear dataset.

•	Energy consumption in month of march is high and low in Jan month and increase in temp leads to more energy consumption

•	Decrease in Humidity leads increase in power consumption. Humidity is inversely proportional to dependent variable.

•	Hour of the Day is the most important influencing parameter for Energy consumption

•	High Electricity consumption of >140Wh is observed during evening hours 16:00 to 20:00. Weekends (Saturdays and Sundays) are observed to have high consumption of electricity. (> 25% than Weekdays)

•	lights are having very low importance as a feature

•	Random forest is the best model its performance is good compare to others have high r2 on test

•	Through model explain ability found which feature has high importance.
