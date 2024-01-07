# Crop Recommendation System using Machine Learning

### Overview

This repository presents the implementation of a Crop Recommendation System that leverages machine learning techniques. The system suggests suitable crops based on environmental conditions such as nutrients, temperature, humidity, pH, and rainfall.

### Dataset

- The dataset (`Crop_recommendation.csv`) contains information about various crops, featuring **`Nitrogen (N), Phosphorus (P), Potassium (K), temperature, humidity, pH, rainfall,`** and corresponding crop labels.
- With **`2200`** entries and no missing values, the dataset is comprehensive.

#### Key Terms

- **N, P, K:** Essential nutrients denoting Nitrogen, Phosphorus, and Potassium.
- **Temperature, Humidity, pH, Rainfall:** Environmental conditions influencing crop growth.
- **Label:** Categorical crop types **`(e.g., rice, wheat)`**.

### Exploratory Data Analysis (EDA)

Exploring the dataset provides insights into the characteristics of different crops and their dependencies on environmental factors.

#### Rainy Season Insights

The rainy season witnesses a substantial increase in average rainfall, impacting soil moisture levels and pH. Certain crops, such as rice and coconut, flourish under these conditions.

### Data Preprocessing

The data undergoes preprocessing to handle categorical labels, explore correlations, and ensure compatibility with machine learning models.

#### Feature Scaling

The **`MinMaxScaler`** is applied to Gaussian-distributed features like temperature and pH to scale them between 0 and 1.

### Model Selection

Various machine-learning models are explored and evaluated for crop prediction.

#### KNN Classifier

The K-Nearest Neighbors (KNN) classifier is tuned using GridSearchCV, achieving a training accuracy of **`98%`** and a test accuracy of **`97%`**.

#### SVM Classifier

Support Vector Classifier (SVC) is applied with different kernels (linear, RBF, poly). GridSearchCV is used to tune hyperparameters, resulting in a tuned accuracy of **`98.4%`** for the linear kernel.

#### Decision Tree

A Decision Tree Classifier achieves an accuracy of **`98.6%`** on the test set. Feature importance is visualized.

#### Random Forest

The Random Forest Classifier with a max depth of **`4`** and **`100`** estimators achieves **`95%`** accuracy on the training set and **`92%`** on the test set.

#### Gradient Boosting Tree

The Gradient Boosting Classifier attains an accuracy of **`98.18%`**.

### Crop Prediction for Custom Input

A sample input representing environmental conditions is utilized to predict the recommended crop using the Random Forest Classifier.

### Usage

Clone the repository and execute the provided Jupyter Notebook (`Crop_Recommendation_System.ipynb`) to explore the code and experiment with different inputs.

Feel free to contribute or adapt the code for your specific needs!

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
