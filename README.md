# 📦 Heart Disease Prediction System
This project is a machine learning-based system that predicts the likelihood of heart disease in an individual based on their medical data. The system uses Logistic Regression for model training and demonstrates how to save and load the trained model using pickle.

## 📊 Dataset
The dataset used is heart.csv, which contains various medical measurements of individuals, with the target variable (target) indicating whether the individual has heart disease (1) or not (0).
[Heart Disease Dataset in Kaggle](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)

## Features:
- Age: Age of the individual
- Sex: Gender (1 = male, 0 = female)
- cp: Chest pain type (4 values)
- trestbps: Resting blood pressure (in mm Hg)
- chol: Serum cholesterol in mg/dl
- fbs: Fasting blood sugar > 120 mg/dl (1 = true, 0 = false)
- restecg: Resting electrocardiographic results (values 0, 1, 2)
- thalach: Maximum heart rate achieved
- exang: Exercise-induced angina (1 = yes, 0 = no)
- oldpeak: ST depression induced by exercise relative to rest
- slope: The slope of the peak exercise ST segment
- ca: Number of major vessels (0-3) colored by fluoroscopy
- thal: Thalassemia (3 = normal; 6 = fixed defect; 7 = reversible defect)


## 🛠️ Dependencies
The project uses the following libraries:

- numpy
- pandas
- scikit-learn
You can install the dependencies with:

```
pip install numpy pandas scikit-learn
```

## 🚀 Model Training Process
1. Data Collection and Preprocessing
Load the heart disease dataset (heart.csv) into a pandas DataFrame.
Perform exploratory data analysis (EDA) including checking the dataset structure, missing values, and statistical measures.
Split the data into features (X) and target labels (Y).
2. Model Training
Split the data into training (80%) and test sets (20%) using stratified sampling to maintain the distribution of the target variable.
Train a Logistic Regression model on the training data.
3. Model Evaluation
Evaluate the model's accuracy on both the training and test sets using accuracy_score.
4. Building a Predictive System
Build a system to classify new input data as either "Heart Disease" or "No Heart Disease" using the trained model.
5. Saving and Loading the Model
Save the trained Logistic Regression model to heart_disease_model.sav using pickle.
Load the saved model for future predictions without needing to retrain.

## 📂 Files in Repository
- heart_disease_prediction_system.ipynb: The main Jupyter notebook containing the code for training, evaluating, and saving the model.
- heart.csv: The dataset used for training and evaluating the model.
- heart_disease_model.sav: The saved trained model file.
  
