# Heart Disease Prediction 🫀

A machine learning project that predicts whether a patient has heart disease based on clinical measurements, using Logistic Regression.

## 📌 Problem Statement

To predict the presence of heart disease in a patient (1 = disease, 0 = no disease) using 13 clinical features such as age, sex, chest pain type, blood pressure, cholesterol, and more.

## 📂 Dataset

- **Source:** UCI Heart Disease Dataset
- **Samples:** 303 patients
- **Features:** 13 clinical attributes
- **Target:** `target` column (0 = No Disease, 1 = Disease)

| Feature | Description |
|---|---|
| age | Age of the patient |
| sex | 0 = female, 1 = male |
| cp | Chest pain type |
| trestbps | Resting blood pressure (mm Hg) |
| chol | Serum cholesterol (mg/dl) |
| fbs | Fasting blood sugar > 120 mg/dl |
| restecg | Resting electrocardiographic results |
| thalach | Maximum heart rate achieved |
| exang | Exercise-induced angina |
| oldpeak | ST depression induced by exercise |
| slope | Slope of the peak exercise ST segment |
| ca | Number of major vessels colored by flourosopy |
| thal | Thalassemia type |

## 🛠️ Tools & Libraries

- Python 3
- Jupyter Notebook
- pandas, numpy
- matplotlib, seaborn
- scikit-learn (`train_test_split`, `LogisticRegression`, `accuracy_score`, `confusion_matrix`, `classification_report`)

## 🔍 Approach

1. Load and explore the dataset (EDA)
2. Check for missing values and class distribution
3. Split data into training (70%) and testing (30%) sets
4. Train a Logistic Regression model on all 13 features
5. Predict on the test set
6. Evaluate using accuracy, classification report, and a confusion matrix

## 📊 Results

- **Accuracy:** ~78%
- Evaluated using precision, recall, and F1-score for both classes
- Confusion matrix visualized as a heatmap

## 🚀 How to Run

1. Clone this repository
```bash
git clone <your-repo-url>
cd heart-disease-prediction
```
2. Install dependencies
```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```
3. Open the notebook
```bash
jupyter notebook Heart_Disease_Prediction_Classification.ipynb
```

## 📁 Project Structure

```
heart-disease-prediction/
├── README.md
├── Heart_Disease_Prediction_Classification.ipynb
└── heart.csv
```

## 🔮 Future Improvements

- Feature scaling (StandardScaler)
- Cross-validation for more reliable accuracy estimates
- Try other models (Random Forest, KNN, SVM) and compare
- ROC curve and AUC score
- Hyperparameter tuning with GridSearchCV
