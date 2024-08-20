Diabetes Prediction
Overview
This repository contains the complete project files for predicting diabetes using machine learning. The project is aimed at early detection and management of diabetes, which is crucial in preventing complications and improving the quality of life for individuals at risk. The model is deployed using a user-friendly Streamlit application, enabling real-time predictions.

Project Structure
The repository includes the following files and directories:

Diabetes_Prediction_Project_Report.pdf: Detailed project report covering the entire development process, from data exploration to model deployment.
User_Guide_for_Streamlit_App.pdf: A guide for users to navigate and use the Streamlit application for diabetes prediction.
Data_Preprocessing_and_Model_Training.ipynb: Jupyter Notebook for data exploration, preprocessing, feature selection, and model training.
Diabetes_Prediction_Streamlit_App.py: The Streamlit application that deploys the trained machine learning model for real-time predictions.
Datasets/: Directory containing the datasets used for training and testing the model.
Diabetes_Prediction.pkl: Trained Random Forest model saved as a pickle file for deployment.
Project Description
1. Introduction
Diabetes is a chronic condition that affects millions globally. This project aims to develop a machine learning model that can predict whether an individual is diabetic based on various health attributes.

2. Dataset Description
The dataset consists of 100,000 records with 9 features, including both numerical and categorical variables. The target variable indicates whether an individual is diabetic (1) or not (0).

3. Data Exploration and Preprocessing
Data Exploration: The dataset was inspected for structure, types of variables, and missing values. Summary statistics were generated to understand the distribution of numerical variables.
Data Preprocessing: Involves categorical encoding, feature scaling, and saving the preprocessed data for model training.
4. Feature Selection
Feature selection was performed using correlation analysis, feature importance from the Random Forest model, and a variance threshold method. All features were retained as they contributed to the model's predictive power.

5. Model Building and Evaluation
Model Selection: A Random Forest classifier was chosen for its robustness and effectiveness.
Class Imbalance Handling: SMOTE was used to balance the training set, addressing the class imbalance.
Model Evaluation: The model was evaluated using accuracy, precision, recall, F1-score, and a confusion matrix. The decision threshold was adjusted to improve recall for diabetic cases.
Final Model: The trained model was saved as a .pkl file for deployment.
6. Model Deployment Using Streamlit
The trained model was deployed using a Streamlit application, allowing users to input data and receive real-time predictions. The application is designed to be intuitive and easy to use.

How to Run the Project
1. Set Up the Environment
Ensure that you have Python installed along with the required libraries:

pip install -r requirements.txt

2. Run the Streamlit Application
Navigate to the directory containing the Streamlit app file and run the following command:

streamlit run Diabetes_Prediction_Streamlit_App.py

This will launch the application in your default web browser.

3. Use the Application
Follow the User Guide provided in the repository to interact with the application and make predictions based on your input data.

Conclusion
This project successfully developed a machine learning model for predicting diabetes, with a strong focus on accuracy and user accessibility. Future improvements could focus on enhancing the model's ability to predict diabetic cases more accurately and deploying the application on a cloud platform for broader reach
