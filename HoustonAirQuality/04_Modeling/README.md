![cover](https://github.com/Aurenkeelin18/For_You_Thorough_Recruiter/blob/a35e4f5f2c3fae011ffc7f84abc9145cf48ae13d/HoustonAirQuality/06_Images/HAQ_MOD_Title.png)

## Choosing the Appropriate Model
The following models were tested:
* Linear Regression with sklearn linear_model.
* Linear Regression with statsmodel OLS.
* Multilinear Regresssion with statsmodel OLS.
* Support Vector Regression using RBF kernel with sklearn SVR.
* Support Vector Machine using RBF kernel with sklearn SVM.
* Multiclass Logistic Regression with sklearn LogisticRegression.
* K Nearest Neighbor with sklearn KNeighborsClassifier.
* Extreme Gradient Boosting with XGBoost [https://xgboost.readthedocs.io/en/latest/]

![mod](https://github.com/Aurenkeelin18/For_You_Thorough_Recruiter/blob/c4fcfd18aff3805de5a68b3f7afe187bd43f6746/HoustonAirQuality/06_Images/HAQ_MOD_slide1.png)

The model could be built focusing on ozone concentration values or AQI labels:
* In practice the dataset was too imbalanced to allow the detection of the rarer labels “Unhealthy” and “Very Unhealthy” by algorithms like Logistic Regression, SVM, KNN and XGB Classifier. Applying SMOTE to the dataset did not help the classification models because it forced the model to overfit the minority classes. 
* Linear and multi-linear regression do not fit the problem. 
* SVR with RBF kernel was performing well with the training set but performed poorly with the testing test.  
* XGB Regressor provided the best cross-validation results.

The XGB Regressor was tuned using the following parameters: 
* reg:Squarrederror objective with gbtree booster,
* colsample_bytree and subsample set to 1,
* Eta at 1.3 and 20 for maxdepth.

MAE is the primary metric because the aim of the model is to show trends rather than predicting daily data. RMSE is used to keep an eye on the distance between daily data and predicted data. 
**The metrics of the final model are: MAE = 4.3 and RMSE = 6.2.**

## Model Results
The features of importance show that maximum temperature, wind speed and daily precipitation are the main drivers behind ozone concentrations in the air. Being  near an industrial zone seems to play a role thought minor. Population and traffic have little influence.
The model shows that the hypothesis “More people, more traffic, more pollution” is likely incorrect.  The graph ozone daily measurement vs. predictions shows that the model is not built for daily predictions.
The major features of importance of the ozone model are not surprising:
- the first feature is the maximum temperature, which is a catalyst in the formation of ozone.
- the second and third features are the wind, which transports the ozone away from its source and  is the reason why ozone can be found in remote country areas.
- the fourth feature is the amount of rain precipitation, which is interesting because rainy days tend to be less polluted because the pollutants are washed away by the rain. This phenomenon is called 'wet deposition'. Here the influence of rain will have to be determined: is it washing away pollution or washing it in?
- the fifth feature is industrial activity. Note that the pollution is not in the industrial zone, but 'near' it, which story works well with the influence of the  wind and the rain on ozone formation.


![mod2](https://github.com/Aurenkeelin18/For_You_Thorough_Recruiter/blob/c4fcfd18aff3805de5a68b3f7afe187bd43f6746/HoustonAirQuality/06_Images/HAQ_MOD_slide2.png)

This outcome is not surprising because temperature is a catalyst in the formation of ozone. Regarding the wind, it may play a role of transportation, concentration or dispersion of ozone or of the chemicals leading its formation. The model can be used to see how this works in practice.
![ozoneformation](https://github.com/Aurenkeelin18/For_You_Thorough_Recruiter/blob/2812db2978ba95c3f1d4ff4e7470cd6468a13491/HoustonAirQuality/06_Images/HAQ_OzoneFormation.jpg)



picture in the title banner from https://taniere-de-kyban.fr/2019/des-modeles-en-pate-a-modeler
