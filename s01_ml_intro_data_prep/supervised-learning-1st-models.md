# Supervised Learning & First Models

## Table of Contents

1. [What is Supervised Learning?](#1-what-is-supervised-learning)
2. [Supervised Learning Workflow](#2-supervised-learning-workflow)
3. [ML Models Exercises](#3-ml-models-exercises)

## 1. What is Supervised Learning?

In **Supervised Learning** the model is trained using labeled data:

- **Inputs (features):** the data used to make predictions
- **Outputs (target/label):** the known value we want the model to predict

### The Model's Goal

Learn the mapping between features (X) and target (y).

### Types of Tasks

- **Classification** predicts categories
- **Regression** predicts numbers

[(back to top)](#table-of-contents)

## 2. Supervised Learning Workflow

### Step 1 | Split Features (X) and Target (y)

| Features (X) | Input variables used to predict |
|:--- |:--- |
| **Target (y)** | Output you want to predict |
| **Why** | Prevents data leakage |

### Step 2 | Split into Train/Test

| Train | Data model learns on |
|:--- |:--- |
| **Test** | Unseen data used to judge model |
| **Why** | Mimics real-life and prevents optimistic, misleading score |

### Step 3 | Choose an Algorithm

| Classification | Logistic Regression, Decision Tree, Random Forest, Gradient Boosting, SVM |
|:--- |:--- |
| **Regression** | Linear Regression, Decision Tree/Random Forest, Gradient Boosting |
| **Why** | Models differ in assumptions and trade-offs |

### Step 4 | Fit the Model

- `.fit(X_train, y_train)` learn parameters for the models
- Only training data should inform the model to void leakage

### Step 5 | Predict with Test Data

| `.predict(X_test)` | Get class/number predictions |
|:--- |:--- |
| **`.predict_proba(X_test)`** | For classification probabilities (threshold tuning) |
| **Why** | Shows how model generalizes to new data |

### Step 6 | Evaluate

Classification metrics:

- **Accuracy** (overall correctness)
- **Precision/Recall & F1** (class-imbalance aware)
- **ROC AUC / PR AUC** (ranking quality)
- **Confusion matrix** (types of errors)

Regression metrics:

- **MAE** (average absolute error)
- **RMSE** (penalizes large errors)
- **R²** (variance explained)

>**Golden Rule:**
>
> - _Train:_ Fit only
> - _Test:_ Transform, Predict, Evaluate

[(back to top)](#table-of-contents)

## 3. ML Models Exercises

1. [Guided: Regression Data](/notebooks/03_ml_model_regression.ipynb)
2. [Guided: Titanic Dataset](/notebooks/04_ml_model_titanic.ipynb)
3. [Unguided: Adult Income](/notebooks/05_ml_model_adult_income.ipynb)

---

Proceed to next section:

[(back to top)](#table-of-contents)  
[(back to README)](/README.md)
