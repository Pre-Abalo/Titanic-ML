# 🚢 Titanic — Machine Learning Starter Project

Beginner-friendly ML project using the classic Titanic dataset (Kaggle).
Goal: predict passenger survival from tabular features (age, sex, class, etc.), with a clear, step-by-step workflow.

## 📂 Structure
```
Titanic-ML/
├── data/            # CSV files (not committed)
├── notebooks/       # Jupyter notebooks (detailed & step-by-step)
├── src/             # Reusable Python modules (optional)
├── models/          # Saved models (not committed)
└── outputs/         # Figures & predictions
```

## ⚙️ Setup
```bash
git clone <your_repo_url>
cd Titanic-ML
pip install -r requirements.txt
```

## 🧪 Run
1) Put `train.csv` and `test.csv` into `data/` (download from Kaggle: https://www.kaggle.com/c/titanic).
2) Launch Jupyter:
```bash
jupyter notebook
```
3) Open the notebooks in order:
   - `01_setup_data.ipynb`
   - `02_exploration_eda.ipynb`
   - `03_baseline_logistic.ipynb`

## 🛠️ Technical Stack

- **Python 3** → flexible, widely used in ML.
- **Pandas / NumPy** → data loading, cleaning, and manipulation.
- **Matplotlib** → simple, reliable visualization (EDA, distributions, correlations).
- **Scikit-learn** → machine learning pipeline:
    - Imputation: median (numeric) / mode (categorical) for missing values.
    - One-Hot Encoding: categorical variables → numeric features.
    - Logistic Regression: simple, interpretable baseline model.
    - Cross-validation: robust performance estimation.
- **Joblib** → save and reload trained models.
- **Jupyter Notebook** → step-by-step workflow, mixing code and explanations.

### Why this stack?

- It’s lightweight, beginner-friendly, and widely used in the ML community.
- Scikit-learn provides a clean, modular pipeline API to avoid data leakage.
- Logistic Regression is a strong baseline: interpretable, fast, and establishes a reference before trying advanced models.

## ✅ Baseline
The baseline uses a simple preprocessing pipeline (median/mode imputation + one-hot encoding) and a Logistic Regression classifier, evaluated with stratified cross-validation.

## 📜 License
MIT (feel free to reuse).
