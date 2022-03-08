# Mobile-Price-Range-Prediction

Problem Statement: In the competitive mobile phone market companies want to understand sales data of mobile phones and factors which drive the prices. The objective is to find out some relation between features of a mobile phone (e.g.: - RAM, Internal Memory, etc.) and its selling price. In this problem, we do not have to predict the actual price but a price range indicating how high the price is.
Further based on different features of mobile phones, develop a model that would classify each mobile into different categories of price range, i.e., into categorical value of 0 (low), 1 (Medium), 2 (High) and 3 (Very High).

Data Structure: We are provided with Mobile Price Range Prediction Dataset. The dataset contains around 2000 observations and 21 columns. Dataset having categorical and numerical features with any null values and unwanted columns were removed which were of less importance.

Data Analysis: Mobile price range prediction dataset contains features like battery_power, ram, four_g, three_g, wifi, etc. Here our dependent variable was price range which is divided into 4 categories: 0(Low cost), 1(Medium cost), 2(High cost) and 3(Very high cost). We divided features into 3 categories: continuous features, discrete features and binary features.
With various visualization techniques, we got to understand the relationship of different feature types with our dependent variable. Using correlation heatmap, we found multi-collinearity among variables. Some feature engineering done to reduce the number of features.
Various regression models like XGBoost, SVM, etc. were used to fit the data. Classification report of both train and test set gave insight into the model performance. Variance and bias tradeoff played major role in determining the efficiency one model. Shap package was used for model explainability. Summary plot was used to explain various features important to our model prediction.


Conclusion:

•	Features like RAM, battery power and pixels are most important in model predictability. This can also be seen while doing data visualization.

•	Logistic Regression performs better than tree-based models because important features change linearly with price changes and logistic regression has linear decision boundary, so it gives better results.

•	XGBoost performs better than other tree-based models because while generating tree, the leaves are penalized which doesn't improve the model predictability.

•	SVM performed much better than all other models because it has more accurate results and also able to generalize the features much better than others. The classification report also shows good prediction score for each class (0, 1, 2 and 3).
