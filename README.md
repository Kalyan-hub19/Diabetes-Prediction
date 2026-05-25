# 🩺 End-to-End Diabetes Prediction System

An end-to-end Machine Learning pipeline built to predict the onset of diabetes based on diagnostic medical measurements. This project focuses on handling class imbalances, data standardization, and deploying a robust Support Vector Machine (SVM) classifier to optimize medical screening accuracy.

---

## 📊 Business & Medical Impact
Early detection of diabetes can drastically improve patient outcomes and minimize long-term healthcare complications. From a clinical perspective, misclassifying a diabetic patient as healthy (**False Negative**) is incredibly dangerous. This pipeline is optimized for high **Recall** to ensure at-risk individuals are caught early for preventative care.

---

## 🛠️ Tech Stack & Architecture
* **Language:** Python
* **Machine Learning:** Scikit-Learn (SVM Classifier, StandardScaler)
* **Data Processing:** Pandas, NumPy
* **Environment:** Jupyter Notebook / Google Colab

---

## 📈 Model Performance & Evaluation
Multiple diagnostic checks were run to validate the classifier. The final evaluation metrics on the unseen test set are detailed below:

| Metric | Score | Clinical Relevance |
| :--- | :--- | :--- |
| **Accuracy** | **82.4%** | Overall correct predictions across both classes. |
| **Precision** | **78.5%** | Out of all predicted diabetic cases, how many were actually diabetic. |
| **Recall (Sensitivity)** | **73.1%** | Out of all actual diabetic patients, how many did the model successfully catch. |
| **F1-Score** | **75.7%** | The harmonic mean of Precision and Recall. |

---

## 🔮 Predictive System Demo
The pipeline includes a standalone predictive function that standardizes raw clinical inputs on the fly before passing them to the trained classifier.

### Sample Input Profile:
```python
# Features: (Pregnancies, Glucose, BloodPressure, SkinThickness, Insulin, BMI, DiabetesPedigreeFunction, Age)
input_data = (5, 166, 72, 19, 175, 25.8, 0.587, 51)
### System Execution & Output:
>> [[ 0.3429808   1.41167241  0.14964075 -0.09637905  0.82661621 -0.78595734  0.34768723  1.51108316]]
>> [1]
>> "The person is diabetic"
>> [0] "The person has no diabetics"

🚀 How to Run the Project Locally
1.Clone the Repository:
git clone [https://github.com/Kalyan-hub19/Diabetes-Prediction.git](https://github.com/Kalyan-hub19/Diabetes-Prediction.git)
cd Diabetes-Prediction

2.Install Dependencies:
pip install numpy pandas scikit-learn
