# Heart Failure Prediction using Artificial Neural Networks (ANN)

This repository contains a Deep Learning project that predicts the mortality of patients with heart failure using clinical records. The model is built using a multi-layer **Artificial Neural Network (ANN)** implemented with Keras and TensorFlow.

## 📌 Project Overview
Heart failure is a common event caused by Cardiovascular Diseases (CVDs). This project aims to use machine learning to predict patient survival based on 12 clinical features, helping healthcare providers prioritize high-risk cases.

## 📊 Dataset
The project utilizes the [Heart Failure Clinical Records Dataset](https://www.kaggle.com/datasets/andrewmvd/heart-failure-clinical-data).
* **Samples:** 299
* **Features:** 13 (including age, anaemia, creatinine phosphokinase, ejection fraction, etc.)
* **Target:** `DEATH_EVENT` (1 if the patient deceased, 0 otherwise)

## 🛠️ Tech Stack
* **Language:** Python
* **Deep Learning:** TensorFlow, Keras
* **Data Analysis:** Pandas, NumPy
* **Visualization:** Seaborn, Matplotlib
* **Preprocessing:** Scikit-learn (StandardScaler, Train-Test Split)

## 🏗️ Model Architecture
The ANN is a sequential model designed with regularization to prevent overfitting:
1. **Input Layer:** 16 units, ReLU activation.
2. **Hidden Layer 1:** 8 units, ReLU activation.
3. **Dropout Layer:** 25% (Regularization).
4. **Hidden Layer 2:** 4 units, ReLU activation.
5. **Dropout Layer:** 50% (Regularization).
6. **Output Layer:** 1 unit, Sigmoid activation (for binary classification).

**Compilation Settings:**
* **Optimizer:** Adam
* **Loss Function:** Binary Crossentropy
* **Callbacks:** Early Stopping (Patience = 20)

## 📈 Performance Results
The model achieved the following results on the test set:

| Metric | Score |
| :--- | :--- |
| **Accuracy** | 81% |
| **Validation Accuracy (Avg)** | 77.59% |

### Classification Report:
* **Precision (Survived):** 0.88
* **Recall (Survived):** 0.88
* **F1-Score (Deceased):** 0.61

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone [https://github.com/yourusername/heart-failure-prediction.git](https://github.com/yourusername/heart-failure-prediction.git)
