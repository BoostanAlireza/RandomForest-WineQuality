# 🍷 Wine Quality Prediction using Random Forest

This project uses a machine learning model (Random Forest Classifier) to predict the quality of red wine based on its physicochemical properties. The dataset is sourced from the UCI Machine Learning Repository.

## 📂 Dataset

- **Name**: Wine Quality Data Set (Red Wine)
- **Source**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Wine+Quality)
- **File**: `winequality-red.csv`
- **Features**: 11 chemical attributes (e.g., acidity, sugar, pH)
- **Target**: Wine quality (integer score between 3 and 8)

## 📊 Features Used

- `fixed acidity`
- `volatile acidity`
- `citric acid`
- `residual sugar`
- `chlorides`
- `free sulfur dioxide`
- `total sulfur dioxide`
- `density`
- `pH`
- `sulphates`
- `alcohol`

## 🧠 Model

- **Algorithm**: Random Forest Classifier
- **Train-Test Split**: 70% training / 30% testing
- **Evaluation Metrics**:
  - Confusion Matrix
  - Accuracy Score
  - Classification Report (Precision, Recall, F1-score)

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/wine-quality-prediction.git
cd wine-quality-prediction
