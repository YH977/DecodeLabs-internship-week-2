# Iris Species Classification

A basic machine learning project to demonstrate supervised learning classification using the Iris dataset.

## 🎯 Project Goal
The objective of this project is to build a classification model that can accurately predict the species of an iris flower based on four physical measurements: sepal length, sepal width, petal length, and petal width.

## 📊 Dataset Overview
The project uses the **Iris Dataset**, a staple in the data science community.
- **Features:** Sepal Length, Sepal Width, Petal Length, Petal Width.
- **Target:** `Species` (Setosa, Versicolor, Virginica).
- **Size:** 150 samples (small, clean dataset).

## 🛠️ Key Skills Demonstrated
- **Data Handling:** Loading and inspecting data with `pandas`.
- **Pre-processing:** Categorical encoding with `LabelEncoder` and feature scaling with `StandardScaler`.
- **Supervised Learning:** Implementing a **K-Nearest Neighbors (KNN)** algorithm.
- **Evaluation:** Using `accuracy_score`, `confusion_matrix`, and `classification_report`.

## 🚀 The Machine Learning Pipeline
1. **Load Data:** Imported the dataset and checked for missing values.
2. **Feature Engineering:** Removed unnecessary columns (e.g., `Id`).
3. **Encoding:** Converted the categorical target labels into numerical format.
4. **Data Splitting:** Divided the data into **Training (80%)** and **Testing (20%)** sets.
5. **Scaling:** Applied `StandardScaler` to ensure the distance-based KNN algorithm isn't biased by different measurement scales. *(Note: Scaling was applied after the split to prevent data leakage).*
6. **Training:** Initialized and fit the KNN model ($k=3$).
7. **Testing:** Predicted species for the test set and evaluated the results.

## 📈 Results
The model achieved high performance metrics:
- **Accuracy:** 1.0 (100%)
- **Precision:** 1.0
- **Recall:** 1.0

*Note: While 100% accuracy is often a sign of errors in complex data, it is a common and expected result for the Iris dataset due to the clear separation between species classes.*

## 📂 File Structure
- `Iris.csv`: The raw dataset.
- `project_2.py`: The Python script containing the code.
- `README.md`: This documentation.

## 🔧 Installation & Usage
1. Clone this repository.
2. Install required libraries:
   ```bash
   pip install pandas scikit-learn
