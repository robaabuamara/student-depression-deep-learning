# student-depression-deep-learning
# Student Depression Prediction Using Deep Learning

## Project Overview

This project applies a Deep Neural Network to predict student depression as a binary classification problem.

The goal of the project was to apply the concepts learned in Kaggle's Introduction to Deep Learning course to a complete real-world machine learning workflow.

## Dataset

The dataset contains 27,901 student records with academic, lifestyle, and personal features.

The target variable is:

- `Depression = 0`
- `Depression = 1`

Some of the features include:

- Gender
- Age
- Academic Pressure
- Work Pressure
- CGPA
- Study Satisfaction
- Job Satisfaction
- Sleep Duration
- Dietary Habits
- Degree
- Work/Study Hours
- Financial Stress
- Family History of Mental Illness

## Data Preprocessing

The preprocessing workflow included:

- Removing unnecessary columns
- Cleaning invalid values
- Handling missing values
- Encoding binary categorical variables
- One-Hot Encoding multi-class categorical variables
- Feature scaling using StandardScaler
- Splitting the dataset into training and validation sets

## Neural Network Architecture

The model was built using TensorFlow and Keras.

Architecture:

- Input Layer
- Dense Layer: 64 neurons with ReLU
- Dropout: 0.3
- Dense Layer: 32 neurons with ReLU
- Dropout: 0.2
- Output Layer: 1 neuron with Sigmoid

## Training Configuration

The model used:

- Optimizer: Adam
- Loss Function: Binary Crossentropy
- Metric: Binary Accuracy
- Early Stopping to reduce overfitting

## Results

Best Validation Accuracy:

**84.66%**

Minimum Validation Loss:

**0.3587**

### Classification Report

| Class | Precision | Recall | F1-score |
|------|------:|------:|------:|
| 0 | 0.82 | 0.79 | 0.81 |
| 1 | 0.86 | 0.88 | 0.87 |

Overall validation accuracy was approximately **84%**.

## Confusion Matrix

The model produced:

- 1826 correct predictions for class 0
- 2875 correct predictions for class 1
- 487 false positives
- 392 false negatives

## Sample Predictions

The model was also tested on individual validation samples.

Some predictions were correct with high confidence, while some high-confidence predictions were still incorrect.

This demonstrates that model probability should not be interpreted as certainty.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- TensorFlow
- Keras
- Matplotlib
- Joblib

## Learning Outcomes

Through this project, I practiced:

- Data cleaning
- Data preprocessing
- Categorical encoding
- Feature scaling
- Neural network architecture design
- Binary classification
- Dropout
- Early stopping
- Model evaluation
- Precision, Recall, and F1-score analysis

## Disclaimer

This project is for educational purposes only.

The dataset contains sensitive mental-health-related information, and the model should not be used for medical diagnosis or professional mental health assessment.
