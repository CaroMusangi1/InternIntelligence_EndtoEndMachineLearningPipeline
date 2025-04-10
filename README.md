# InternIntelligence_EndtoEndMachineLearningPipeline
Project Title: End-to-End Machine Learning Pipeline
Description:
This project implements a complete machine learning pipeline that includes the steps of data ingestion, preprocessing, model training, evaluation, and saving. The Titanic dataset is used to build a pipeline where the features are processed, the model is trained, and the final model is saved for later use.

Key Concepts:
Pipeline: A streamlined process where each step of the workflow (data preprocessing, training, etc.) is linked together, allowing for easier maintenance and automation.

ColumnTransformer: Used to apply different preprocessing steps to different columns of the dataset.

Joblib: Used to save the trained model to a file so that it can be reused without retraining.

Steps:
Load Titanic dataset:

The Titanic dataset is loaded using pandas.read_csv().

The dataset contains features like age, sex, class, etc., and the target variable is whether the passenger survived.

Clean and preprocess features:

Missing values in the dataset are handled.

Categorical features are encoded, and continuous features are scaled.

Build the pipeline:

A Pipeline is constructed that first applies preprocessing steps like scaling and encoding, followed by training the model.

The preprocessing steps are handled using ColumnTransformer.

Train a Logistic Regression model:

A Logistic Regression model is used for classification.

The model is trained on the processed features of the dataset.

Evaluate model performance:

The model’s performance is evaluated using metrics such as accuracy, precision, recall, and F1-score.

Save trained model using joblib:

The trained model is saved using joblib.dump() so that it can be loaded and used in future applications without retraining.

Libraries Used:
scikit-learn: For building the machine learning pipeline and training the Logistic Regression model.

pandas: For loading and manipulating the dataset.

numpy: For numerical operations.

seaborn: For data visualization (optional).

joblib: For saving the trained model.

How to Use:
Open the notebook in Google Colab.

Run all cells in sequence.

Adjust preprocessing steps or model hyperparameters as needed.

Save the final trained model for future use by calling joblib.load() on the saved model file.

Example Output:
The final output will include the model's accuracy and performance metrics, and a saved .pkl model file for future predictions.
