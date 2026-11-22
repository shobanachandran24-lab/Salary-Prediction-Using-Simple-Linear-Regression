# Salary Prediction Using Simple Linear Regression

A beginner-friendly machine learning project that predicts an employee's **salary** from their **years of experience** using simple linear regression.

## Dataset

`simple_linear_regression_dataset.csv` contains 10 records:

| Column | Description |
|---|---|
| `Experience_Years` | Years of work experience (feature) |
| `Salary` | Salary (target) |

Experience ranges from 1 to 10 years and salary from 22,000 to 65,000.

## Project Workflow

1. Import libraries (pandas, NumPy, Matplotlib, Seaborn, scikit-learn)
2. Load the dataset
3. Check the data (`head()`, `info()`, missing values)
4. Split into feature (`Experience_Years`) and target (`Salary`)
5. Scatter plot, correlation and heatmap to confirm a linear relationship
6. Train/test split (80/20, `random_state=42`)
7. Train a `LinearRegression` model
8. Predict salaries for the test set
9. Compare actual vs predicted values
10. Evaluate with MAE, MSE, RMSE and R²
11. Plot the best-fit line
12. Residual plot to check the quality of the fit
13. Predict salary for a new value

## Results

| Metric | Value |
|---|---|
| Correlation (Experience vs Salary) | 0.9993 |
| Mean Absolute Error (MAE) | ~633.62 |
| Mean Squared Error (MSE) | ~542,100.18 |
| Root Mean Squared Error (RMSE) | ~736.27 |
| R² Score | ~0.998 |

Fitted line: `Salary ≈ 4818.97 × Experience_Years + 16620.69`

Example: predicted salary for 5 years of experience is about **40,715**.

> Note: the dataset is very small (10 rows), so these scores are only illustrative.

## Tech Stack

- Python
- pandas, NumPy
- Matplotlib, Seaborn
- scikit-learn

## How to Run

```bash
git clone <your-repo-url>
cd <your-repo-folder>
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
jupyter notebook Simple_linear_regression.ipynb
```

Keep `simple_linear_regression_dataset.csv` in the same folder as the notebook.

## Files

- `Simple_linear_regression.ipynb`: the full notebook
- `simple_linear_regression_dataset.csv`: the dataset
- `README.md`: project documentation
