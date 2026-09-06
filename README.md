# Breast Cancer Classification

## 📌 Project Overview

This project builds and evaluates a **Machine Learning Classification Model** to predict whether a breast tumor is **malignant or benign**.

A **Logistic Regression** model is used for classification, and its performance is evaluated using:

* Accuracy
* Precision
* Recall
* Confusion Matrix
* Classification Report

The project demonstrates the complete machine learning workflow, including data loading, preprocessing, feature scaling, model training, prediction, and evaluation.

---

## 📊 Dataset

The dataset used in this project is the **Breast Cancer Wisconsin (Diagnostic) Dataset**, downloaded from **Kaggle**.

🔗 **Kaggle Dataset:**
https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data

The dataset contains features computed from digitized images of breast mass cell nuclei. The target variable indicates whether the tumor is **malignant (M)** or **benign (B)**.

### ⚠️ Dataset Not Included in This Repository

The dataset is **not uploaded to GitHub**.

To run this project:

1. Download the dataset from the Kaggle link above.
2. Extract the downloaded file.
3. Place the CSV file inside the `data/` folder.
4. Make sure the dataset filename matches the filename used in the notebook.

---

## 📁 Project Structure

```text
breast-cancer-classification/
│
├── data/
│   └── breast_cancer.csv
│
├── classification_model.ipynb
│
├── requirements.txt
│
├── README.md
│
└── .gitignore
```

### Folder and File Description

| File/Folder                  | Description                                                     |
| ---------------------------- | --------------------------------------------------------------- |
| `data/`                      | Contains the downloaded dataset                                 |
| `data/breast_cancer.csv`     | Kaggle dataset — **not pushed to GitHub**                       |
| `classification_model.ipynb` | Jupyter Notebook containing the complete ML workflow            |
| `requirements.txt`           | Python dependencies required to run the project                 |
| `README.md`                  | Project documentation                                           |
| `.gitignore`                 | Prevents the dataset and unnecessary files from being committed |

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## 🤖 Machine Learning Model

### Logistic Regression

Logistic Regression is used as the classification algorithm to predict the tumor class.

Before training the model, the numerical features are standardized using `StandardScaler`.

### Workflow

```text
Dataset
   ↓
Data Loading
   ↓
Data Cleaning & Preprocessing
   ↓
Train-Test Split
   ↓
Feature Scaling
   ↓
Logistic Regression
   ↓
Predictions
   ↓
Model Evaluation
```

---

## 📈 Model Evaluation

The model is evaluated using the following metrics:

### Accuracy

Measures the overall percentage of correctly classified observations.

### Precision

Measures how many of the observations predicted as positive are actually positive.

### Recall

Measures how many of the actual positive observations were correctly identified by the model.

The notebook displays the calculated:

```text
Accuracy
Precision
Recall
```

along with a **confusion matrix** and **classification report**.

> Note: The exact metric values may vary depending on the train-test split and preprocessing.

---

## 🚀 How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/cp1928/breast-cancer-classification.git
```

### 2. Navigate to the project folder

```bash
cd breast-cancer-classification
```

### 3. Create a virtual environment

```bash
python -m venv .venv
```

### 4. Activate the virtual environment

**Windows:**

```powershell
.venv\Scripts\activate
```

**Mac/Linux:**

```bash
source .venv/bin/activate
```

### 5. Install dependencies

```bash
pip install -r requirements.txt
```

### 6. Download the dataset

Download the dataset from Kaggle:

https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data

Place the CSV file inside:

```text
data/
```

### 7. Start Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
classification_model.ipynb
```

and run the cells.

---

## 📌 Results

The Logistic Regression model provides strong classification performance on the test dataset.

The following metrics are reported in the notebook:

* **Accuracy:** ~97%
* **Precision:** ~97%
* **Recall:** ~99%

The exact values can vary based on the dataset and train-test split.

---

## 👩‍💻 Author

**Chitra P**

GitHub:
https://github.com/cp1928

---

## 📄 License

This project is created for educational and machine learning practice purposes.
