# Cancer Antigen Regression

## Overview
Predict cancer antigen level (log scale) from clinical features using linear models. This repository compares Ordinary Least Squares (OLS), Ridge, and Lasso regressions. Manual cross-validation is implemented for hyperparameter selection and model comparison.

## Dataset
The dataset contains clinical measurements such as:
- logCancerVol, logCancerWeight, age, logBenignHP, svi, logCP, gleasonScore, gleasonS45, levelCancerAntigen

A train/test split is provided in the dataset.

## Methodology
1. Data import and exploratory data analysis  
2. Preprocessing and normalization (documented in the notebook)  
3. Manual cross-validation for Ridge and Lasso hyperparameters  
4. Model evaluation using RMSE, MAE, and R²  
5. Interpretation of the most influential features via coefficients

## How to run
1. Create and activate a Python virtual environment (recommended).  
2. Install dependencies:
```
pip install -r requirements.txt
```
3. Open and run the notebook:
`cancer-antigen-regression.ipynb`

## Notes & Recommendations
- Do not upload any patient-identifiable data.  
- If model artifacts are large, exclude them and include code to retrain models.  
- Cite any external code or libraries used.

## Repository structure
- `cancer-antigen-regression.ipynb` — main notebook  
- `requirements.txt` — dependencies
