# News-Article-Source-Prediction

Predict cost on media campaigns in food mart of usa on the basis of 60k customers income, product, promotion and store features.

## Dataset

- The Data set is selected from Kaggle.com
- It has 40 columns and 60058 rows.

## Preprocessing

- Checking and removal of Null values.
- Encoding of categorical predictors.
- Removal of redundant columns on the basis of correlation matrix.
- Removal of column with no relation with target variable.

## Predictive Modeling

The dataset is rich has both numerical and categorical, we tried both Ordinal and One hot encoding techniques and trained below models.
- Linear Regression
- Decision Tree Regressor
- KNN
- Random Forest Regressor
- Random Forest Boosting
- Random Forest XGBoosting
- Neural Network

## Performance Analysis

![image](https://user-images.githubusercontent.com/57527313/218596665-371b3ab7-5128-41dc-b00a-2afd008a1728.png)

## References

- https://www.kaggle.com/datasets/ramjasmaurya/medias-cost-prediction-in-foodmart
