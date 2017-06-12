# Predicting-Age-of-Abalones
The goal is to predict the age of abalones using machine learning models. Instead of predicting raw age in years, the final goal will be to predict "young","medium","old"-defined as grouping ring classes 1-8, 9-10, and 11 on.




Classification of Abalones Data
Goal: Predicting age of abalones
Input variables: Sex, Length, Diameter, Height, Whole weight, Shucked weight, Viscera weight, Shell weight, Rings
•	Sex is either Male ("M"), Female ("F") or Infant ("I"), this is not suitable for regression algorithms, so I created a numeric feature: 1:Male, 2: Female, 3:Infant	
•	There are no missing/null values in dataset. At 2 places height is 0mm , but considering it in mm we can ignore it considering 4000 rows
•	Added age column in the dataframe for classification. Age is classified based on the number of rings.
Rings 1-8 -->Age 1, denoting young
Rings 9-10 -->Age 2, denoting middle
Rings 11-29 -->Age 3, denoting old
 

I used 4 classification algorithms and their respective accuracy is as follows:

Models	
1. Neural Network
Accuracy : 64.6889952153
Root mean square error(RMSE): 0.6777389936698861
Mean Absolute error(MAE): 0.388516746411

2. Logistic Regression	
Accuracy : 65.2631578947
Root mean square error(RMSE):	0.6903296487356203
Mean Absolute error(MAE): 0.39043062201

3. Random Forest	
Accuracy : 62.5837320574
Root mean square error(RMSE):	0.7254762501100116
Mean Absolute error(MAE):	0.424880382775

4. KNN Classifier	
Accuracy : 61.8181818182
Root mean square error(RMSE):	0.7228333405962345
Mean Absolute error(MAE):	0.428708133971

Conclusion: Neural network gives highest accuracy for classification of age data among all the 4 models, depending on rmse value of 0.677 which is lowest.

