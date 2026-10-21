# 🩺 AI-Powered Multi-Disease Prediction System

A machine learning web application built with Python and Streamlit to demonstrate predictions for five diseases through a single interactive dashboard.

## 🚀 Overview

This project integrates pretrained machine learning models into one application. Users can select a disease module, enter the requested health-related features, and view the model's prediction.

### Supported Disease Modules

| Disease | Machine Learning Model | Reported Accuracy |
|---|---|---:|
| Diabetes | Support Vector Machine (SVM) | ~77% |
| Heart Disease | Random Forest Classifier | ~85% |
| Liver Disease | Gradient Boosting Classifier | ~87% |
| Kidney Disease | Random Forest Classifier | 100% |
| Breast Cancer | Random Forest Classifier | ~95% |

*Note: These accuracy figures are reported by the original project documentation and have not been independently verified. Model performance depends on the dataset, evaluation procedure, and input data.*

## ✨ Features

- **Multi-disease prediction:** Five disease prediction modules in one application.
- **Interactive dashboard:** Navigate between disease modules using the sidebar.
- **Pretrained models:** Load saved machine learning models from the `models/` directory.
- **Data preprocessing:** Apply the preprocessing implemented for each model.
- **Prediction results:** Display the model's output through the Streamlit interface.
- **Modular structure:** Separate training scripts are provided for selected disease models.

## 🛠️ Technology Stack

- **Language:** Python
- **Web framework:** Streamlit
- **Machine learning:** Scikit-learn, XGBoost
- **Data processing:** NumPy, Pandas
- **Model persistence:** Pickle
- **Version control:** Git and GitHub

## 🏗️ System Architecture

```text
User
  |
  v
Streamlit Dashboard
  |
  v
Select Disease Module
  |
  v
Enter Input Features
  |
  v
Data Preprocessing
  |
  v
Load Trained ML Model
  |
  v
Generate Prediction
  |
  v
Display Result
```

## 📂 Project Structure

```text
disease-prediction/
├── app.py
├── README.md
├── requirements.txt
├── .gitignore
├── datasets/
├── models/
├── train_breast_cancer_model.py
├── train_heart_model.py
├── train_kidney_model.py
├── train_liver_model.py
└── train_models.py
```

The `datasets/` directory contains the available datasets, while `models/` contains saved model files used by the application.

## 💻 Installation and Setup

### Prerequisites

- Python 3.10 or a compatible Python version
- Git
- Internet access for installing dependencies

### 1. Clone the repository

```bash
git clone https://github.com/spandey009/disease-prediction.git
cd disease-prediction
```

### 2. Create a virtual environment

**Windows PowerShell:**

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

### 3. Install dependencies

Upgrade pip:

```powershell
python -m pip install --upgrade pip
```

The supplied `requirements.txt` may need to be decoded if it is saved in UTF-16 encoding. To create a temporary UTF-8 copy on Windows PowerShell without
