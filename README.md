# Crop Recommendation System using Machine Learning

## Overview

This repository contains an implementation of a Crop Recommendation System that utilizes machine learning techniques. The system recommends suitable crops based on environmental conditions such as nutrients, temperature, humidity, pH, and rainfall.

## Dataset

- The dataset (`Crop_recommendation.csv`) includes information about various crops, with features like **`Nitrogen (N), Phosphorus (P), Potassium (K), temperature, humidity, pH, rainfall,`** and corresponding crop labels.
- The dataset consists of **`2200`** entries with no missing values.

### Key Terms

- **N, P, K:** Essential nutrients representing Nitrogen, Phosphorus, and Potassium.
- **Temperature, Humidity, pH, Rainfall:** Environmental conditions affecting crop growth.
- **Label:** Categorical crop types **`(e.g., rice, wheat)`**.

## Exploratory Data Analysis (EDA)

Exploring the dataset provides insights into the characteristics of different crops and their dependencies on environmental factors.

### Rainy Season Insights

During the rainy season, there is a significant increase in average rainfall, impacting soil moisture levels and pH. Specific crops like rice and coconut thrive under these conditions.

## Data Preprocessing

The data is preprocessed to handle categorical labels, explore correlations, and ensure compatibility for machine learning models.

### Feature Scaling

**`MinMaxScaler`** is applied to Gaussian-distributed features like temperature and pH to scale them between 0 and 1.

## Model Selection

Several machine learning models are explored and evaluated for crop prediction.

### KNN Classifier

The K-Nearest Neighbors (KNN) classifier is tuned using GridSearchCV, achieving a training accuracy of **`98%`** and a test accuracy of **`97%`**.

### SVM Classifier

Support Vector Classifier (SVC) is applied with different kernels (linear, RBF, poly). GridSearchCV is used to tune hyperparameters, resulting in a tuned accuracy of **`98.4%`** for the linear kernel.

### Decision Tree

A Decision Tree Classifier achieves an accuracy of **`98.6%`** on the test set. Feature importance is visualized.

### Random Forest

Random Forest Classifier with max depth **`4`** and **`100`** estimators achieves **`95%`** accuracy on the training set and **`92%`** on the test set.

### Gradient Boosting Tree

Gradient Boosting Classifier achieves an accuracy of **`98.18%.`**

## Crop Prediction for Custom Input

A sample input representing environmental conditions is used to predict the recommended crop using the Random Forest Classifier.

## Usage

Clone the repository and run the provided Jupyter Notebook (`Crop_Recommendation_System.ipynb`) to explore the code and experiment with different inputs.

Feel free to contribute or adapt the code for your specific needs!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

