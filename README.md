# ML Sampling Project

## Introduction

This project investigates the impact of different sampling techniques on the performance of machine learning models. Sampling plays a crucial role in handling imbalanced datasets and ensuring model generalization. In this project, we explore five common sampling techniques and evaluate their effects on five popular machine learning models.

## Sampling Techniques

1. **Simple Random Sampling**

   Definition: Randomly selecting data points from a dataset without any specific criteria.
   Purpose: Basic and commonly used to create a representative subset.
2. **Stratified Sampling**

   Definition: Ensures the proportion of each class in the sample reflects the proportion in the entire dataset.
   Purpose: Particularly useful when dealing with imbalanced datasets.

3. **Systematic Sampling**

   Definition: Involves selecting every k-th element from the dataset after a random starting point.
   Purpose: A deterministic method providing a representative sample.

4. **Bootstrap Sampling**

   Definition: Involves repeatedly sampling with replacement from the dataset.
   Purpose: Often used for estimating the distribution of a statistic.

5. **Cluster Sampling**

   Definition: Divides the dataset into clusters and randomly selects entire clusters to form the sample.
   Purpose: Useful when the dataset has a natural grouping.
   
## Machine Learning Models

1. **Random Forest**

   Definition: An ensemble learning method that constructs a multitude of decision trees during training.
   Purpose: Used for classification problems, outputting the mode of the classes.
   
3. **K-Nearest Neighbors**

   Definition: A non-parametric classification algorithm that classifies new data points based on the majority class of their k-nearest neighbors.
   Purpose: Useful for both classification and regression tasks.

4. **Naive Bayes**

   Definition: A probabilistic classification algorithm based on Bayes' theorem, assuming independence between features.
   Purpose: Efficient and commonly used for text classification.

5. **Neural Network**

   Definition: A machine learning model inspired by the human brain, consisting of interconnected nodes (neurons) organized in layers.
   Purpose: Suitable for complex tasks such as image recognition and natural language processing.
6. **Support Vector Machines**

   Definition: A powerful classification algorithm that finds the hyperplane that best separates the data into different classes.
   Purpose: Effective for both linear and non-linear classification tasks.

## Results and Analysis

The table below shows the accuracy of each model under different sampling techniques:

| Sampling Technique      | Random Forest | K-Nearest Neighbors | Naive Bayes | Neural Network | Support Vector Machines |
|--------------------------|---------------|----------------------|-------------|-----------------|--------------------------|
| Simple Random Sampling   | 1.0000        | 0.8701               | 0.9610      | 0.9870          | 0.8831                   |
| Stratified Sampling      | 1.0000        | 0.9871               | 0.9806      | 0.9871          | 0.9871                   |
| Systematic Sampling      | 1.0000        | 0.9329               | 0.7450      | 0.9732          | 0.9664                   |
| Bootstrap Sampling       | 1.0000        | 0.9250               | 0.9625      | 1.0000          | 0.9750                   |
| Cluster Sampling         | 1.0000        | 0.9932               | 0.9658      | 0.9932          | 1.0000                   |

## Box Plot

![Unknown-2](https://github.com/cheshtabiala/Sampling_Assignment/assets/94442128/bdd2c9bb-dbdd-4f6e-a894-94634b28dff8)

## Line Plot
![Unknown](https://github.com/cheshtabiala/Sampling_Assignment/assets/94442128/a3ca170a-a9e0-4d92-8433-a183e928f2eb)

## Conclusion

After analyzing the performance of machine learning models under different sampling techniques, the following observations can be made:

1. **Random Forest:**
   - All sampling techniques except Stratified Sampling have the same accuracy.

2. **Logistic Regression:**
   - Systematic Sampling gives the highest accuracy.

3. **Decision Trees:**
   - Both Stratified Sampling and Bootstrap Sampling give the highest accuracy.

4. **Gradient Boosting:**
   - All sampling techniques except Simple Random Sampling give the same accuracy.

5. **Support Vector Machines:**
   - All sampling techniques except Simple Random Sampling give the same accuracy, with Bootstrap Sampling having the highest.

In summary, the choice of the best sampling technique varies depending on the machine learning model. While some models perform consistently across different sampling methods, others show sensitivity to specific sampling strategies. Consideration of these observations is crucial when selecting the appropriate model and sampling technique for a given dataset and problem domain.


