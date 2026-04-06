#  Disaster Tweets Classification

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![ML](https://img.shields.io/badge/Machine%20Learning-Scikit--Learn-orange)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

---

##  Project Overview

This project performs **binary classification of disaster-related tweets** using multiple machine learning models.

The goal is to determine whether a tweet is about a real disaster or not.

### Models Used

* Logistic Regression
* Random Forest
* Neural Network (MLP)

###  Handling Class Imbalance

* Class Weighting
* SMOTE (Synthetic Minority Oversampling Technique)
* Threshold Tuning

---

##  Project Structure

AI_proj/
│── model_v3.ipynb       # Main notebook
│── tweets.csv           # Dataset
│── README.tex           # Original LaTeX README
│── requirements.txt     # Dependencies

---

##  Requirements

###  Run on Google Colab (Recommended)

No setup required.

###  Local Installation

pip install pandas numpy scikit-learn matplotlib imbalanced-learn tensorflow

---

##  Dataset

Dataset used:
https://www.kaggle.com/datasets/vstepanenko/disaster-tweets/data

### Steps:

1. Download dataset
2. Extract file
3. Place tweets.csv in project directory

---

##  How to Run

###  Option 1: Google Colab

1. Open: https://colab.research.google.com
2. Upload model_v3.ipynb
3. Upload tweets.csv
4. Click Runtime → Run All

---

###  Option 2: Local Execution

jupyter notebook model_v3.ipynb

---

##  Execution Pipeline

###  Data Processing

* Data loading
* Text preprocessing
* Train-test split
* Validation split

###  Feature Engineering

* TF-IDF Vectorization

---

###  Model Training

####  Logistic Regression

* GridSearchCV (hyperparameter tuning)
* Threshold tuning
* Class weighting
* SMOTE

####  Random Forest

* Hyperparameter tuning
* Threshold tuning
* Class weighting
* SMOTE

####  Neural Network (MLP)

* Activation function tuning
* Optimizer selection
* Learning rate tuning
* Weight initialization
* Threshold tuning
* Class weighting
* SMOTE

---

##  Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix
* ROC Curve
* Precision-Recall Curve

---

##  Outputs

The notebook generates:

* Detailed classification reports
* Performance comparison of models
* Visualizations (ROC & PR curves)

---

##  Important Notes

* TF-IDF is used for text feature extraction
* Validation set is used for threshold tuning
* Cross-validation applied in Logistic Regression
* SMOTE is applied only on training data to prevent data leakage

---

##  Results & Insights

* Logistic Regression performs best for sparse TF-IDF features
* Random Forest gives competitive results
* Neural Network underperforms due to sparse input representation
* SMOTE significantly improves recall and balance

---

##  Future Improvements

* Use word embeddings (Word2Vec, GloVe, BERT)
* Try deep learning models (LSTM, Transformers)
* Hyperparameter optimization with Bayesian methods
* Deploy as a web application

---

##  Contributing

Contributions are welcome!

1. Fork the repository
2. Create a new branch
3. Commit changes
4. Submit a Pull Request

---

##  License

This project is open-source and available.

---

##  Author

Koti Reddy,
Yangala Reddy Sekhar,
Venkat Subbaiah,
Abhiram,
Palla Rakesh
---

##  Acknowledgements

* Kaggle dataset contributors
* Scikit-learn & TensorFlow communities
