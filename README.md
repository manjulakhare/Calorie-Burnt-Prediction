Project Description
This project is focused on predicting calories burnt during exercise using machine learning regression models. It is built using Python in a Google Collab and demonstrates a complete ML pipeline — from data preprocessing to model evaluation — using real-world biometric and exercise data.
Objective:
To estimate the number of calories a person burns based on various features like gender, age, height, weight, heart rate, duration of exercise, and body temperature.
________________________________________
 Workflow Overview:
1. Data Collection & Merging
   •	Two datasets were used: one with exercise details and the other with calorie values.
   •	The datasets were merged using pd.concat() to create a single dataset containing all relevant features.
2. Data Exploration
   •	Displayed basic information about the dataset using .head(), .shape, .info(), and .describe().
   •	Checked for missing values using .isnull().sum().
3. Data Preprocessing
   •	Label Encoding was applied to convert the categorical Gender column into numerical form.
   •	Removed non-numeric columns when computing correlation to avoid errors.
   •	Checked correlations between input features and the target (Calories) using .corr().
4. Feature Selection & Target Definition
   •	Selected relevant features (Gender, Age, Height, Weight, Duration, Heart_Rate, Body_Temp) as X.
   •	Selected Calories as the target variable Y.
5. Train-Test Split
   •	The dataset was split into training and testing sets using an 80/20 ratio via train_test_split.
6. Model Training
   •	Used XGBoost Regressor (XGBRegressor) for regression modeling.
   •	Trained the model using the training data.
7. Model Evaluation
   •	Made predictions on the test set.
   •	Evaluated the model using:
      o	R² Score: To measure how well the predictions match the actual values.
      o	Mean Absolute Error (MAE): To measure prediction error in actual units.
8. Visualization
   •	Created scatter plots to compare actual vs. predicted calorie values for better visual understanding.
________________________________________
Key Libraries Used:
   •	pandas, numpy for data handling
   •	matplotlib, seaborn for visualization
   •	xgboost, sklearn for machine learning
________________________________________
