# Wine Quality Classification
This project aims to predict the quality of wines based on their chemical properties. The dataset used in this project is the "Wine Quality" dataset from the UCI Machine Learning Repository.

# Data
The dataset consists of 11 input variables and 1 output variable (quality), as follows:

Fixed acidity

Volatile acidity

Citric acid

Residual sugar

Chlorides

Free sulfur dioxide

Total sulfur dioxide

Density

pH

Sulphates

Alcohol

Quality (score between 0 and 10)

The dataset contains 1599 samples.

# Approach
The first step in this project was to perform exploratory data analysis to get an idea of the data and its properties. The EDA involved analyzing the distribution of each variable, as well as correlations between variables. The data was visualized using various plotting techniques, such as heatmaps and pairplots.

After the EDA, some preprocessing steps were performed on the data. Highly correlated features were dropped, as well as samples with very high density and residual sugar. The remaining features were then scaled using the StandardScaler.

Two different classifiers were used to predict the quality of wines: Logistic Regression and Random Forest. The models were trained on 80% of the data and tested on the remaining 20%. To address the class imbalance in the data, SMOTE was used to oversample the minority classes.

# Results
The best performing model was the Random Forest classifier, which achieved an F1-score of 0.78 on the test set. The Logistic Regression classifier achieved an F1-score of 0.56 on the test set.

# Conclusion
In this project, we were able to predict the quality of wines based on their chemical properties with a decent level of accuracy. Random Forest outperformed Logistic Regression in this task. Future work could involve trying other classification algorithms, as well as experimenting with different preprocessing techniques.
