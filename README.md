# Parkinson's Disease Prediction

This project aims to predict Parkinson's disease based on various biomedical voice measurements. Parkinson's disease is a progressive nervous system disorder that affects movement and can cause tremors, stiffness, and difficulty with balance and coordination.

## Dataset

The dataset used in this project contains biomedical voice measurements from individuals with and without Parkinson's disease. It consists of the following features:

1. Fundamental frequency measures
2. Frequency perturbation measures
3. Amplitude perturbation measures
4. Nonlinear dynamic measures
5. Tonality measures
6. Acoustic measures

The target variable is the presence or absence of Parkinson's disease, encoded as 0 for absence and 1 for presence.

## Preprocessing

Before training the predictive model, the dataset undergoes the following preprocessing steps:

1. Data cleaning: Handle missing values, if any, and remove any outliers.
2. Feature scaling: Standardize the features to have mean 0 and standard deviation 1.
3. Train-test split: Split the dataset into training and testing sets for model evaluation.

## Model Training

The predictive model is trained using a Support Vector Classifier (SVC) with a radial basis function (RBF) kernel. The choice of model and kernel is based on experimentation and performance evaluation.

## Evaluation

The trained model's performance is evaluated using various metrics, including accuracy, precision, recall, and F1-score. The evaluation metrics provide insights into how well the model generalizes to unseen data and its ability to correctly classify individuals with and without Parkinson's disease.

## Prediction

Once the model is trained and evaluated, it can be used to predict Parkinson's disease in new individuals based on their biomedical voice measurements. The prediction process involves preprocessing the input data, making predictions using the trained model, and interpreting the prediction results.

## Dependencies

- Python 3.x
- scikit-learn
- NumPy
- pandas
