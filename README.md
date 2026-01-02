# ML Classification Project: Riyadh Metro Station Type Prediction

**Complete end-to-end Machine Learning pipeline** for predicting whether a metro station is **Deep Underground** or another type.

## Dataset
- **Source:** Official Riyadh Metro Authority (Public Data 2024)
- **File:** `metro-stations-in-riyadh-by-metro-line-and-station-type-2024 (1).csv`
- **Samples:** 104 metro stations across 6 lines
- **Problem:** Binary Classification (Imbalanced: ~33% Deep Underground, ~67% Other)
- **Features:** Latitude, Longitude, Line Number, Metro Line Name, Station Name

## Project Structure

```
ML_WEEK3/
├── ML_classification_project.ipynb    # Main notebook (all code & explanations)
├── metro-stations-in-riyadh-...csv    # Dataset (real public data)
├── requirements.txt                   # Python dependencies
└── README.md                          # This file
```

## What's Included

✓ **Problem Definition** — Why ML is suitable for this problem  
✓ **Data Loading & Inspection** — Loading CSV and initial exploration  
✓ **Data Cleaning** — Handling missing values, feature engineering  
✓ **EDA** — Class imbalance visualization, statistics  
✓ **Preprocessing Pipeline** — StandardScaler + OneHotEncoder with ColumnTransformer  
✓ **Baseline Model** — DummyClassifier for reference  
✓ **Model Selection** — 4 models (Logistic Regression, Decision Tree, Random Forest, SVM)  
✓ **Cross-Validation** — 5-fold stratified CV with F1-scoring  
✓ **Hyperparameter Tuning** — GridSearchCV optimization  
✓ **Final Evaluation** — Confusion matrix, precision/recall/F1, ROC-AUC  
✓ **Discussion** — Imbalance handling, overfitting/underfitting analysis  

## How to Run

### 1. Install dependencies
```bash
pip install -r requirements.txt
```

### 2. Run the notebook
```bash
jupyter notebook ML_classification_project.ipynb
```

### 3. Execute cells in order
- Start from the top and run each section sequentially
- All data loading and model training will run automatically

## Key Results

- **Best Model:** Decision Tree (Stratified K-Fold CV F1=0.9110)
- **Test Accuracy:** 94.74%
- **Test F1-Score:** 0.9412
- **ROC-AUC:** 0.9545

## Deliverables (Course Requirements)

✅ Completed Jupyter Notebook with full ML pipeline  
✅ README.md with clear instructions  
✅ Real dataset (CSV file)  
✅ All code, analysis, and discussion in one notebook  
✅ Ready for GitHub repository  

## Technologies

- **Python 3.x**
- **Libraries:** pandas, numpy, scikit-learn, matplotlib, seaborn
- **Notebook:** Jupyter
