# Breast Cancer Prediction Using Machine Learning

## Overview

This project focuses on predicting the presence of breast cancer using machine learning models. We experiment with four different algorithms to achieve this task and utilize the breast cancer dataset from Kaggle.

## Dataset

The dataset used in this project is the `Breast Cancer Wisconsin Data` which is available on Kaggle.

- **Dataset Source**: [Breast Cancer Wisconsin Data](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data?resource=download)

## Implemented Models

- **Decision Tree Classifier (CART)**
- **Support Vector Machines (SVM)**
- **Naive Bayes (NB)**
- **K-Nearest Neighbors (KNN)**

## Code Structure

1. **Imports**: Necessary libraries and modules.
2. **Exploratory Analysis**: Basic checks on the dataset's shape, attributes, etc.
3. **Data Visualization and Preprocessing**:
   - Convert diagnosis into a binary format.
   - Remove unnecessary columns.
   - Plot attribute correlations.
4. **Dataset Splitting**: Splitting the data into training and testing sets.
5. **Model Evaluation**:
   - **Raw Data**: Each model's performance is evaluated on the raw data.
   - **Standardized Data**: Each model's performance is also assessed after standardizing the dataset.
6. **Algorithm Tuning**: Using GridSearchCV for tuning hyperparameters of the SVM model.
7. **Model Preparation and Prediction**: Using the best parameters, the SVM model is trained and evaluated on the test dataset.

## How to Run

1. Download the dataset from the provided Kaggle link and place it in the same directory as this script.
2. Run the Python script to perform the predictions and evaluate the models' performances.
   ```bash
   python <script_name>.py
   ```

## Results

The results, including accuracy, precision, recall, etc., are printed on the terminal after the script is executed. The script evaluates the models' performances on both raw and standardized data.

## Dependencies

To run this project, the following libraries are required:

- numpy
- pandas
- matplotlib
- sklearn

## Notes

- Several parts of the code, such as data visualization (density plots, heatmaps, etc.) and SVM algorithm tuning, are commented out. Uncomment if you wish to execute these sections.
- Ensure you have the required libraries installed. Use pip to install any missing dependencies.
- Adjust the dataset path in the `pd.read_csv()` method if you place the dataset in a different directory.

## Contributions

Feel free to fork this project, contribute, and raise any issues or suggestions. We're always looking to improve and collaborate.
