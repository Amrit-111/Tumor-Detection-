
# 🧪 Tumor Detection using Random Forest

This project aims to detect whether a tumor is **malignant** or **benign** using diagnostic data and a machine learning model. It includes **exploratory data analysis (EDA)**, **feature engineering**, **data preprocessing**, and building a **Random Forest classifier** for prediction.

---

## 📁 Dataset

The dataset contains diagnostic measurements for various tumors, including:
- Statistical summaries like `mean`, `standard error`, and `worst` values
- Target column: `diagnosis` (`M` = Malignant, `B` = Benign)

---

## 📊 Exploratory Data Analysis

- Count plot of malignant vs benign tumor cases
- Descriptive statistics of diagnostic features
- Correlation heatmap for feature relationships
- Grouped feature sets: `_mean`, `_se`, `_worst`

---

## 🛠️ Preprocessing Steps

- Removed the `id` column as it's not relevant for prediction
- Converted categorical `diagnosis` into numeric (1 = Malignant, 0 = Benign)
- Standardized features using `StandardScaler` to normalize input data

---

## 🤖 Model Building

- **Model Used**: Random Forest Classifier (`sklearn.ensemble`)
- **Train-Test Split**: 70% for training, 30% for testing
- **Evaluation Metric**: Accuracy

---

## 📈 Model Performance

✅ **Achieved Accuracy**:  
🎯 **~95%+** (depending on train-test split randomness)

The model was evaluated using `accuracy_score` from `sklearn.metrics`, and the result shows that the Random Forest Classifier performs reliably in predicting whether a tumor is malignant or benign.

```python
from sklearn.metrics import accuracy_score
print("Accuracy:", accuracy_score(y_test, y_pred))


## 📦 Libraries Used

The following Python libraries were used in this project:

- 📊 **pandas** – For data manipulation and analysis  
- 🧮 **numpy** – For numerical computations  
- 📈 **matplotlib** – For creating static plots and visualizations  
- 🎨 **seaborn** – For advanced data visualization (heatmaps, count plots)  
- 🤖 **scikit-learn** – For machine learning models and preprocessing




