# Online Food Delivery Customer Analysis and Prediction

## Project Description
A complete data analytics and machine-learning project for analyzing online food delivery customers and predicting the `Output` field (`Yes`/`No`).

## Dataset
The CSV used for this submission was provided with the project. A matching public dataset source is:
https://www.kaggle.com/datasets/srisyra02/online-food-ordering-dataset

Local filename required by the notebook:
`online food delivery dataset.csv`

## Dataset Summary
- Original records: 388
- Original columns: 14
- Exact duplicate rows: 103
- Clean records used: 285
- Target: `Output`

## Technologies
Python, Pandas, NumPy, Matplotlib, Scikit-learn, Jupyter Notebook, python-docx.

## Machine Learning
- Logistic Regression
- Random Forest Classifier
- One-Hot Encoding for categorical variables
- StandardScaler for numerical variables
- 80/20 stratified train-test split
- 5-fold stratified cross-validation
- Metrics: Accuracy, Precision, Recall, F1-score, ROC-AUC

## Leakage Prevention
`Unnamed: 13` is removed because it duplicates `Output`. `Feedback` is excluded from model features because it is outcome-related and may not be known at prediction time.

## Test Results From the Supplied Dataset
| Model | Accuracy | Precision | Recall | F1 | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Random Forest | 0.789 | 0.830 | 0.907 | 0.867 | 0.744 |
| Logistic Regression | 0.737 | 0.780 | 0.907 | 0.839 | 0.698 |

## Setup
1. Install Python 3.10+.
2. Put the CSV beside the notebook.
3. Run `pip install -r requirements.txt`.
4. Start Jupyter with `jupyter notebook`.
5. Open `KotiShiva_OnlineFoodDeliveryCustomerAnalysis.ipynb`.
6. Run all cells.

## Files
- `KotiShiva_OnlineFoodDeliveryCustomerAnalysis.ipynb` — complete code
- `requirements.txt` — dependencies
- `KotiShiva_ProjectReport.docx` — documentation
- `README.md` — project overview
