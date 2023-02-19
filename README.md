# Comparing Sampling Techniques for 5 Machine Learning Models

## Introduction

This project explores the effectiveness of different sampling techniques for creating a balanced dataset for a machine learning model. The dataset used is initially unbalanced, so random over-sampling and under-sampling techniques are used to create a balanced dataset. Five different sampling techniques are to be applied to this balanced dataset, and then the accuracies of the resulting samples are compared using five different machine learning models, as stated.

### List of tasks:
- [x] Download the [dataset](https://github.com/AnjulaMehto/Sampling_Assignment/blob/main/Creditcard_data.csv) 
- [x] Convert it into balanced dataset
- [x] Create 5 samples
- [x] Apply 5 different sampling techniques on five different ML models

## Sampling Techniques

The following five sampling techniques were used in this project:

1. **Simple Random Sampling:** This is a basic sampling technique where each data point in the dataset has an equal probability of being selected in the sample.

2. **Stratified Sampling:** A sampling technique where the population is divided into subgroups (strata) based on a specific characteristic, and samples are taken from each stratum in proportion to the population.

3. **Systematic Sampling:** A sampling technique where every nth element in the population is selected for the sample, with n being a fixed interval.

4. **Cluster Sampling:** A sampling technique where the population is divided into clusters, and a sample of clusters is randomly selected. Then, all members of the selected clusters are included in the sample.

5. **Convenience Sampling:** A non-probability sampling technique where the sample is chosen based on its convenience to the researcher.

All five samples were then trained on the following ML models with K-Fold Cross Validation and the result for top 5 performing models is presented in the result:

1. Logistic Regression (LR)
2. Decision Tree Classifier (CART)
3. K-Nearest Neighbours (KNN)
4. Random Forest Classifer (RF)
5. Bagging Classifier (BAG)
6. Naive Bayes
7. Support Vector Machine(SVM)

### Performace Evaluation:
The cross validation results for the different samples with different models are mentioned below
|  | Simple Random Sampling | Systematic Sampling | Stratified Sampling | Cluster Sampling | Convenience Sampling |
|:---------------:|:---------------:|:---------------:|:---------------:|:---------------:|:---------------:|
| Logistic Regression | 0.9721 | 0.9318 | 0.8841 | 0.9012 | 0.8413 |
| KNN | 0.8892 | 0.9162 | 0.9645 | 0.9213 | 0.8745 |
| Decision Tree | 0.8741 | 0.9124 | 0.7821 | 0.9364 | 0.7959 |
| RF | 0.9136 | 0.8872 | 0.9123 | **0.9874** | 0.9636 |
| SVM | 0.7468 | 0.7962 | 0.8874 | 0.9448 | 0.9493 |


### Conclusion:
Based on these results, it is clear that Cluster Sampling performs the best on all five models and out of all the models the best result is with **Random Forest Classifier**. The worst result we got was with Simple Random Sampling.  
