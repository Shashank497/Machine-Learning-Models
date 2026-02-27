# Diabetes Prediction using Machine Learning

This project builds a Machine Learning model to predict whether a person is diabetic or not based on medical attributes. The complete workflow is implemented in a Jupyter Notebook.

---

## 📌 Project Overview

The notebook performs:

- Importing required libraries
- Loading the diabetes dataset
- Data preprocessing
- Splitting data into training and testing sets
- Training a classification model
- Evaluating model performance
- Building a predictive system

---

## 📂 Project File

- `Diabetes.ipynb` → Complete ML workflow (data loading, training, evaluation, prediction)

---

## 📊 Dataset Features

The dataset contains the following medical attributes:

- Pregnancies
- Glucose
- BloodPressure
- SkinThickness
- Insulin
- BMI
- DiabetesPedigreeFunction
- Age
- Outcome (0 = Non-Diabetic, 1 = Diabetic)

---

## ⚙️ Technologies Used

- Python
- NumPy
- pandas
- Scikit-Learn
- Jupyter Notebook

---

## 🚀 How to Run

1. Clone the repository:

```bash
git clone https://github.com/Shashank497/ML-DL-Models.git
cd "ML-DL-Models/Diabetes Prediction"
```

2. Install required libraries (if needed):

```bash
pip install numpy pandas scikit-learn
```

3. Run the notebook:

```bash
jupyter notebook
```

Open `Diabetes.ipynb` and run all cells.

---

## 🧪 Sample Prediction Code (from notebook)

```python
input_data = (6,148,72,35,0,33.6,0.627,50)

import numpy as np
input_data_as_numpy_array = np.asarray(input_data)
input_data_reshaped = input_data_as_numpy_array.reshape(1,-1)

prediction = model.predict(input_data_reshaped)

if prediction[0] == 0:
    print("The person is not diabetic")
else:
    print("The person is diabetic")
```

---

## 📈 Model Evaluation

The model is evaluated using accuracy score on both training and test data.

---

⭐ If you found this project useful, consider giving it a star!
