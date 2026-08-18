# CodeAlpha_SalesPrediction

##  Task
Predict product sales based on advertising spend across TV, Radio, and Newspaper channels, and analyze how each channel impacts sales outcomes. This project is part of the **CodeAlpha Data Science Internship** (Task 4).

##  Dataset
- **Advertising.csv** — 200 records with advertising spend on TV, Radio, and Newspaper, along with resulting Sales.
- No missing values, no duplicate rows.

##  Tools & Libraries
- Python
- Pandas, NumPy
- Matplotlib, Seaborn (visualization)
- Scikit-learn (model building & evaluation)

##  Approach
1. **Data Cleaning** — checked for nulls and duplicates; dropped the unnecessary index column.
2. **Exploratory Data Analysis (EDA)** — visualized relationships between each advertising channel and sales; correlation heatmap to identify strongest predictors.
3. **Model Building** — split data (80/20) and trained a **Linear Regression** model.
4. **Evaluation** — assessed performance using MAE, MSE, and R² score; visualized actual vs predicted sales.
5. **Business Impact Analysis** — extracted regression coefficients to quantify each channel's effect on sales and tested the model on a new sample budget.

##  Results
| Metric | Score |
|---|---|
| R² Score | 0.899 |
| MAE | 1.46 |
| MSE | 3.17 |

**Feature Coefficients:**
| Channel | Coefficient |
|---|---|
| TV | 0.045 |
| Radio | 0.189 |
| Newspaper | 0.003 |

## Business Insights
- Advertising expenditure has a positive relationship with sales.
- **Radio and TV** are the strongest contributors to sales, while Newspaper has minimal impact.
- Marketing budgets should be prioritized toward TV and Radio for better returns.
- The model can estimate expected sales for a proposed advertising budget, helping businesses plan campaigns more effectively.

## How to Run
1. Clone this repository
2. Install dependencies: `pip install pandas numpy matplotlib seaborn scikit-learn`
3. Open `Advertising.ipynb` in Jupyter Notebook and run all cells

## Conclusion
A Linear Regression model was built to predict sales from advertising spend across three channels. The model explained ~90% of the variance in sales (R² = 0.899), with TV and Radio emerging as the most influential channels. These insights can guide businesses in allocating advertising budgets more effectively.

## About
This project was completed as part of the **CodeAlpha Data Science Internship**.
