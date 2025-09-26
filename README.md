# House-Prices---Advanced-Regression-Techniques

The primary objective is to develop a robust regression model capable of predicting the sale price (SalePrice) of houses with high accuracy. 
This involves extensive data exploration, feature engineering, model selection, and hyperparameter tuning.

 1.Techniques and Methodologies:-
   - Handling Missing Data: Strategically imputing missing values using methods like mean/median for numerical features and          None'/'mode' for categorical features, or dropping columns with excessive missingness.

   - Outlier Detection: Identifying and handling influential outliers in features like GrLivArea and SalePrice.

   - Target Transformation: Applying log-transformation to the SalePrice target variable to address its right-skewness and         achieve a distribution closer to normal, which improves model performance (the evaluation metric is
     Root Mean Squared Logarithmic Error (RMSLE)).

2. Feature Engineering :-
   - Handling Categorical Data: One-hot encoding for nominal variables (e.g., $MSSubClass, $ Neighborhood) and                     label/ordinal encoding for ordinal variables (e.g., $ExterQual, $ KitchenQual). 

   - Creating New Features: Deriving meaningful features from existing ones, such as TotalSF (Total Square Footage from            1stFlrSF, 2ndFlrSF, and BsmtSF), or simplifying  year/month features. 

   - Skewness Correction: Applying Box-Cox or log transformations to highly skewed numerical features to make them more            normally distributed.

3. Modeling:-
   - Base Models: Linear Models: Lasso, Ridge, ElasticNet (effective for regularizing features).
  
4. Data:- The dataset consists of:-
   - Training Data: 1460 instances and 81 features (including SalePrice).

   - Test Data: 1459 instances and 80 features.

   - The target variable is SalePrice, and the evaluation metric is RMSLE.
  
5. Key Insights & Results:-
   - Correlation: Features like OverallQual (Overall material and finish quality), GrLivArea (Above grade (ground) living          area square feet), and GarageCars show the strongest positive correlation with SalePrice.
