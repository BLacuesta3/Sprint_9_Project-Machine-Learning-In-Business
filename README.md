Project Title: Sprint 9 Project/ Machine Learning In Business 

Project Description: I will be using Machine Learning in order to create a machine learning model in order to help the OilyGiant mining company (hypothetical company) 
find the best well. This project contains information for Regions 0, 1, and 2 for the OilyGiant mining company. In this project, I will be using a Linear Regression model 
in order to find which of the 3 regions listed is the most profitable for the OilyGiant mining company. This project involves calculating the estimated profit for each region 
using a Linear Regression Model and then using the bootstrapping to revaluate the average estimed profit once again from a dataset of 1000 bootstrapped samples with replacement. 
This project is a regression task.

Task Presented For The Project: 

You work for the OilyGiant mining company. 

Your task is to find the best place for a new well.

Steps to choose the location:

Collect the oil well parameters in the selected region: oil quality and volume of reserves;

Build a model for predicting the volume of reserves in the new wells;

Pick the oil wells with the highest estimated values;

Pick the region with the highest total profit for the selected oil wells.

You have data on oil samples from three regions. Parameters of each oil well in the region are already known. 
Build a model that will help to pick the region with the highest profit margin. Analyze potential profit and risks using the Bootstrapping technique.
You have data on oil samples from three regions. Parameters of each oil well in the region are already known. Build a model that will help to pick the region 
with the highest profit margin. Analyze potential profit and risks using the Bootstrapping technique. 

Project Model Evaluation Metric: RMSE

Project Dataframes: 

* 'geo_data_0.csv'
* 'geo_data_1.csv'
* 'geo_data_2.csv'

Model Used For The Project:

* Linear Regression

Libraries And Tools Used For The Project:

* pandas 

* sklearn.model_selection (function: train_test_split())

* sklearn.linear_model (function: LinearRegression())

* sklearn.model_selection (functions: RandomizedSearchCV(), cross_val_score())

* sklearn.pipeline (function: Pipeline())

* sklearn.preprocessing (function: StandardScaler())

* sklearn.metrics (functions: mean_squared_error(), mean_absolute_error(), r2_score())

* numpy 

* seaborn

* matplotlib.pyplot

Project Methodology: 

1) Importing The Necessary Libraries

2) Reading/ Uploading The Dataframes

3) Data Cleaning/ Data Preprocessing

4) Exploratory Data Analysis (EDA) For Regions: 0, 1, And 2

5) Data Splitting

6) Linear Regression Model Training And Predictions For Regions: 0, 1, And 2
   (Reserve Calculations Per Region Included In Each Model Training Section)

   Best Region Chosen:
   
   According to the results, Region 2 has the highest average amount of predicted reserves with an average predicted amount of: approximately 94.86 K barrels and a
   Linear Regresion model RMSE of: approximately 40.05. Region 0 has the 2nd highest average amount of predicted reserves with an average predicted amount of: 92.78 K
   barrels and a Linear Regression Model RMSE of: approximately 37.64. Region 1 has the lowest average amount of predicted reserves with an average predicted akount of:
   69.17 K barrels and a Linear Regression model RMSE of: approximately 0.88.

8) Calculating Sufficient Volume Of Reserves Amount For Developing A New Well Without Losses For Each Region
   
  Best Region Choice Result: 

   According to the results analysis, it appears that Region 2 would be the best choice when it comes to comparing average predicted reserves to the calculated break 
   even volume of suffient reserves needed for developing a new well without losses. Region 2 had the least difference when subtracting average predicted reserves from the 
   sufficient calculated break even volume of reserves needed for developing a new well without losses. 

   Region 2 Results: 

   It appears that Region 2 has 94.86 K barrels of reserves, which is 16.25 K less reserves than the calculated break even volume of reserves which is 111.11 K barrels. 

9) Calculating Estimated Profit And Estimated Volume Of Reserves For Each Region Using Model Predictions

    Best Region Choice Result:

   According to the results, Region 0 had the highest estimated profit at: $25,012,838.53 and an estimated volume of reserves of: approximately 5558.41 K barrels.

10) Calculating The Risk And Profit For Each Region Using Bootstrapping Technique:

    Bootstrapping Task Directions:

     Calculate risks and profit for each region:
    
    1) Use the bootstrapping technique with 1000 samples to find the distribution of profit.

    2)  Find average profit, 95% confidence interval and risk of losses. Loss is negative profit, calculate it as a probability and then express as a percentage.
   
    Bootstrapping Risk And Profit Task Result:

    According to the boostrapped data, although the Region 1 was the best choice for a deveplopment of oil wells because the region had the highest bootstrap average profit of: 
$4,624,024.33) which was higher than Region 0 and Region 2. Although Regions 0 and 2 had significantly notable amounts for their estimated average bootstrap profits, both these regions' risk of loss were too high with Region 1 having a 7.5% risk of loss and Region 0 having an approximately 11.89% risk of loss. Both Regions 0 and 2 did not satisfy the project's maximum risk of loss threshold of 2.5%, thus making Region 1 the best and only qualified region to suggest a development of oil wells with a low risk of loss of 0.2%.
