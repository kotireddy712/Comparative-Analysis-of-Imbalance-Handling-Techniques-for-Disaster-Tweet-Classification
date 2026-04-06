

README: Execution Instructions

## 1  Project Overview
This project implements binary classification of disaster tweets using:
## •  Logistic Regression
## •  Random Forest
-  Neural Network (MLP)
Imbalance handling techniques used:
## •  Class Weighting
## •  SMOTE
## •  Threshold Tuning
## 2  Project Structure
AI_proj/
model_v3.ipynb
tweets.csv
README.tex
requirements.txt
## 3  Requirements
If using Google Colab, no installation is required.
Otherwise install manually:
pip install pandas numpy scikit-learn matplotlib imbalanced-learn tensorflow
## 1

## 4  Dataset
Download dataset from:
https://www.kaggle.com/datasets/vstepanenko/disaster-tweets/data
Upload tweets.csv into the working environment.
5  How to Run (Google Colab)
## 5.1  Step 1: Open Google Colab
Go to:
https://colab.research.google.com
## 5.2  Step 2: Upload Notebook
-  Click on Upload Notebook
-  Upload model
v
## 3.ipynb
## 5.3  Step 3: Upload Dataset
-  Open Files panel (left side)
-  Upload tweets.csv
5.4  Step 4: Run the Notebook
## •  Click Runtime→ Run All
-  Wait until execution completes
## 6  Execution Flow
The notebook follows this order:
-  Data loading and preprocessing
-  Train-test split and validation split
-  TF-IDF vectorization
## 4.  Logistic Regression
-  Hyperparameter tuning (GridSearchCV)
## 2

-  Threshold tuning
-  Class weighting
## •  SMOTE
## 5.  Random Forest
-  Hyperparameter tuning
-  Threshold tuning
-  Class weighting
## •  SMOTE
-  Neural Network (MLP)
-  Parameter tuning (activation, optimizer, learning rate, initialization)
-  Threshold tuning
-  Class weighting
## •  SMOTE
-  Evaluation metrics and plots
## 7  Outputs
The notebook generates:
-  Classification reports
## •  Accuracy, Precision, Recall, F1-score
-  Confusion matrices
-  ROC curves
-  Precision-Recall curves
## 8  Important Notes
## •  Use Google Colab (recommended).
-  TF-IDF is used for feature extraction.
-  Validation set is used for threshold tuning.
-  Cross-validation is used in Logistic Regression.
-  SMOTE is applied only on training data to avoid data leakage.
## 3

## 9  Final Outcome
-  Logistic Regression performs best for TF-IDF based text classification.
-  Random Forest provides competitive performance.
-  Neural Network performs comparatively lower due to sparse input features.
-  SMOTE provides the best balance between precision and recall.
## 4