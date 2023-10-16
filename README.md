# Python_guided_project
This repository hosts a breast cancer prediction project using machine learning. It includes code, a Jupyter Notebook, and a dataset for building and evaluating a predictive model that classifies breast tumors as malignant (M) or benign (B) based on tumor characteristics.

#Key freatures and actions

Importing Libraries: The project starts by importing essential Python libraries for data analysis and visualization.

Downloading Dataset from Kaggle: The Kaggle API is used to download the breast cancer dataset. The dataset contains information on various tumor characteristics.

Load & Explore Data: The dataset is loaded into a Pandas DataFrame, and its structure is explored. This includes checking for missing values, which are removed.

Label Encoding: The 'diagnosis' column in the dataset is label-encoded, converting the categorical values ('M' for malignant and 'B' for benign) into numerical values for model training.

Split Dataset & Feature Scaling: The dataset is split into independent (X) and dependent (Y) datasets. It is further divided into training and testing sets. Feature scaling is applied to standardize the data.

Build a Logistic Regression Model: A logistic regression classifier is constructed using the training data, and the model is then used to make predictions on the test data.

Performance Evaluation: The performance of the model is evaluated by creating a confusion matrix and calculating accuracy. The accuracy score is used to assess the model's effectiveness in predicting breast cancer diagnoses.

# Instructions to download the dataset directly from kaggle
1. Open a Jupyter Notebook or script in your preferred development environment.

2. Import the `os` library to set up Kaggle API credentials as environment variables.

3. Use the following Python code to set your Kaggle username and API key as environment variables:
   
   import os
   os.environ['KAGGLE_USERNAME'] = 'your_kaggle_username'
   os.environ['KAGGLE_KEY'] = 'your_kaggle_api_key'
   
   Replace `'your_kaggle_username'` and `'your_kaggle_api_key'` with your Kaggle credentials.

4. Execute the following command to download the dataset from Kaggle:
   
   !kaggle datasets download -d uciml/breast-cancer-wisconsin-data
   
   This command will fetch the dataset associated with the specified Kaggle dataset name (`uciml/breast-cancer-wisconsin-data`).

5. After the dataset is downloaded, execute the following command to unzip the dataset:
   
   !unzip /content/breast-cancer-wisconsin-data.zip
   
