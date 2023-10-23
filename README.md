# Prediction of TGV Delays Project

![image](https://github.com/SVJLucas/ApprAuto2023/assets/60625769/59224b7c-4259-4120-bc54-980be999fb05)


## Table of Contents

1. [Introduction](#introduction)
2. [Data Analysis](#data-analysis)
3. [Data Preprocessing](#data-preprocessing)
4. [Modeling](#modeling)
5. [Results](#results)
6. [Conclusion](#conclusion)
7. [Future Work](#future-work)
8. [License](#license)

## Introduction

This project aims to predict TGV train delays and identify their root causes from January to June 2023. The primary dataset used is obtained from the SNCF, and incorporates various features both categorical and numerical.

## Data Analysis

### Data Collection

Data was obtained from the SCNF dataset available on the French government dataset website.

### Data Features

The dataset includes a mix of categorical and numerical variables, providing comprehensive information about TGV trains.

## Data Preprocessing

The data underwent robust preprocessing to prepare it for machine learning models. This includes imputation, encoding, and scaling techniques among others.

### Before Data Preprocessing
![image](https://github.com/SVJLucas/ApprAuto2023/assets/60625769/7fbba4ea-668f-4034-bab4-cda1dd21fd93)



### After Data Preprocessing
![image](https://github.com/SVJLucas/ApprAuto2023/assets/60625769/8940f410-71f4-46cb-9ece-54acc905a6a6)



## Modeling

Multiple machine learning models were evaluated with Extreme Gradient Boosting (xgboost) showing the most promising results. An ensemble model was also developed for better performance.

## Results

## Model Performance Metrics for the Validation Dataset

We tried different models and, at final, we did an ensemble of the 3 best ones.

| Model (Abbreviation)                   | \( R^2 \)  | Training Time (Sec) |
|----------------------------------------|------------|---------------------|
| Extreme Gradient Boosting (xgboost)    | 0.5597     | 1.2780              |
| Huber Regressor (huber)                | 0.5583     | 0.8170              |
| Gradient Boosting Regressor (gbr)      | 0.5531     | 2.3030              |
| Light Gradient Boosting Machine (lightgbm) | 0.5494 | 2.5640          |
| Random Forest Regressor (rf)           | 0.5373     | 5.0760              |
| Extra Trees Regressor (et)             | 0.5353     | 2.4100              |
| CatBoost Regressor (catboost)          | 0.5349     | 6.1840              |
| K Neighbors Regressor (knn)            | 0.4224     | 0.6770              |
| Bayesian Ridge (br)                    | 0.3431     | 0.6010              |
| Ridge Regression (ridge)               | 0.3423     | 0.9220              |
| Least Angle Regression (lar)           | 0.3423     | 0.6000              |
| Linear Regression (lr)                 | 0.3423     | 0.9720              |
| Passive Aggressive Regressor (par)     | 0.3084     | 1.0750              |
| Elastic Net (en)                       | 0.2694     | 0.9870              |
| Lasso Regression (lasso)               | 0.2335     | 0.5900              |
| Lasso Least Angle Regression (llar)    | 0.2335     | 1.0160              |
| Orthogonal Matching Pursuit (omp)      | 0.1784     | 0.8540              |
| AdaBoost Regressor (ada)               | 0.1656     | 0.9840              |
| Decision Tree Regressor (dt)           | -0.1743    | 1.2030              |


## Model Performance Metrics for the Test Dataset
The ensemble model achieved an \( R^2 \) score of 0.8414 on the test set, indicating strong predictive performance.

![results_tgv_delay](https://github.com/SVJLucas/ApprAuto2023/assets/60625769/8b9a7258-542a-4fca-bff6-a7a4da4b8e59)


 However, the neural network used for predicting the causes of delays showed room for improvement.


## Conclusion

The study suggests that incorporating more granular data could significantly enhance the model's predictive capability. It lays a solid foundation for future research aimed at optimizing TGV train delay predictions.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
