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

![image](https://github.com/SVJLucas/ApprAuto2023/assets/60625769/8940f410-71f4-46cb-9ece-54acc905a6a6)



## Modeling

Multiple machine learning models were evaluated with Extreme Gradient Boosting (xgboost) showing the most promising results. An ensemble model was also developed for better performance.

## Results

The ensemble model achieved an \( R^2 \) score of 0.8414 on the test set, indicating strong predictive performance. However, the neural network used for predicting the causes of delays showed room for improvement.
![results_tgv_delay](https://github.com/SVJLucas/ApprAuto2023/assets/60625769/8b9a7258-542a-4fca-bff6-a7a4da4b8e59)

## Conclusion

The study suggests that incorporating more granular data could significantly enhance the model's predictive capability. It lays a solid foundation for future research aimed at optimizing TGV train delay predictions.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
