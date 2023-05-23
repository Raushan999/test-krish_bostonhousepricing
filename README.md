## Test_BostonHousePredicition 
# In this machine learning model, we are predicting the price of house in Boston.
First I performed the Exploratory Data analysis on the dataset downloaded from Kaggle.
Next, I scaled the datapoint using MinMaxScaler/StandardScaler to scale them to same unit so that they converge quickly.
Checked the correlation of all the features wrt to the Medval. 
Used backward propagation to select the best features, --> it led to the removal of "indus", "nox", "age" features since they were having p-value greater than 0.05.
Finally implemnted various regression model to see the accuracy score ( R2-score ) .
Multiple Linear Regression didn't perform well (gave R2 score of 0.5 something)- with both the above mentioned scaling techniques.
The comparision of various models accuracy score is there in the test_bostonprice file.
It was observed that the Random forest performed quite well on the dataset.(R2 score of around 0.83 ) 

## Krish_bostonhousepricing: 
Here, simply we focused on assumptions of linear models, on how should be the behaviour of the scatterplot of the residual vs test and train output.
Finally converted the model to .pkl file and also checked it with new datapoint. 
Now this pkl file can be used to predict new point and is ready to be integrated into webisite/app for deployment.
