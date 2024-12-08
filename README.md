# Air Quality Classification

![PCA Image](\assets\pca_visualization.png)

This project involves classifying air quality based on certain features using a multiclass classification approach. The goal is to predict the air quality category (Good, Moderate, Poor, or Hazardous) from given input features such as pollution levels, temperature, humidity, etc. 

## Dataset
The dataset used for this project is the [Air Quality Data Set](https://www.kaggle.com/api/v1/datasets/download/mujtabamatin/air-quality-and-pollution-assessment). The target variable is the Air Quality Index (AQI) which is a categorical variable with 4 classes: Good, Moderate, Poor, and Hazardous.

### Project Overview
The project follows a systematic process to predict the air quality based on the provided features. Here's an overview of steps done:

1. **Exploratory Data Analysis (EDA)**:
   - Analyzed the dataset to understand its structure, identify patterns, and detect outliers.
   - Visualized the data using various charts to explore relationships between features and target classes.
   
2. **Data Preprocessing**:
   - Handled missing values, standardized the features (StandardScaler), and label encoded categorical variables.
   - Split the dataset into training and test sets to evaluate model performance.
   
3. **Model Selection**:
   - Evaluated five different machine learning models for multiclass classification:
     - **Logistic Regression**
     - **K-Nearest Neighbors (KNN)**
     - **Decision Tree**
     - **Support Vector Classifier (SVC)**
     - **Random Forest**
     
4. **Cross-validation and Grid Search**:
   - Used **Cross-Validation** (10-fold) to evaluate the models' generalizability on unseen data.
   - Performed **Grid Search Cross-Validation** to find the best hyperparameters and estimators for each model.

5. **Model Training & Evaluation**:
   - After identifying the best model through cross-validation, I trained the final model on the entire training set.
   - Evaluated the trained model on the test data using various performance metrics:
     - **Accuracy**
     - **Confusion matrix**
     - **Precision**
     - **Recall**
     - **F1-score**