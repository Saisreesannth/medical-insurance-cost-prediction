# medical-insurance-cost-prediction
A machine learning project that analyzes medical insurance data and predicts insurance costs using linear regression.
# Medical Insurance Cost Prediction — Linear Regression

**Repository:** medical-insurance-cost-with-linear-regression

---

## Project Overview

This project predicts medical insurance charges using a linear regression model. It demonstrates the typical supervised‑learning workflow: data loading, exploratory data analysis (EDA), preprocessing, model training, evaluation, and visualization — all implemented in a Jupyter notebook.

**Notebook (source):** `/mnt/data/medical-insurance-cost-with-linear-regression.ipynb`

---

## Contents

* `medical-insurance-cost-with-linear-regression.ipynb` — Jupyter notebook with full code, explanations, and plots.
* `requirements.txt` *(recommended)* — Python dependencies used for the project.

---

## Dataset

The notebook expects the medical insurance dataset (commonly available as `insurance.csv`) which contains columns such as:

* `age` — age of primary beneficiary
* `sex` — gender
* `bmi` — body mass index
* `children` — number of children covered by health insurance
* `smoker` — whether the person smokes
* `region` — residential area
* `charges` — individual medical costs billed by health insurance

If the notebook already includes the dataset or loads it from a path, follow the code in the notebook. Otherwise, place `insurance.csv` in the same folder as the notebook or update the path in the notebook.

---

## Main Steps (in notebook)

1. **Load data** — read CSV into a pandas DataFrame.
2. **Exploratory Data Analysis (EDA)** — inspect distributions, correlations, and relationships between features and the target (`charges`).
3. **Preprocessing** — handle categorical features (one‑hot encoding or label encoding), scale numerical features if required, and split into train/test sets.
4. **Modeling** — build and train a linear regression model (scikit‑learn `LinearRegression`) and potentially compare with baseline models.
5. **Evaluation** — compute metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), Root MSE (RMSE), and R² score. Visualize predicted vs actual charges.
6. **Conclusion & Next steps** — summarize findings and suggest improvements (feature engineering, regularization, alternate models such as Ridge/Lasso/Tree‑based models).

---

## How to run locally

1. Clone this repository:

```bash
git clone <your-repo-url>
cd medical-insurance-cost-with-linear-regression
```

2. (Optional) Create and activate a virtual environment:

```bash
python -m venv venv
# Windows
venv\Scripts\activate
# macOS / Linux
source venv/bin/activate
```

3. Install dependencies (create `requirements.txt` with required packages if not present):

```bash
pip install -r requirements.txt
```

**Suggested `requirements.txt`**

```
pandas
numpy
matplotlib
scikit-learn
seaborn
jupyter
```

4. Open and run the notebook:

```bash
jupyter notebook medical-insurance-cost-with-linear-regression.ipynb
```

Or execute the notebook headlessly:

```bash
jupyter nbconvert --to notebook --execute medical-insurance-cost-with-linear-regression.ipynb --output executed_notebook.ipynb
```

---

## Results & Interpretation

The notebook contains model performance metrics and plots. Look for the evaluation section (MAE, RMSE, R²) and visualizations such as predicted vs actual scatter plots to understand model quality. Linear regression provides a simple, interpretable baseline — review residuals and consider more complex models if performance is insufficient.

---

## Suggestions for improvement

* Try regularized linear models (Ridge, Lasso) to reduce overfitting.
* Engineer interaction terms (e.g., `bmi * smoker`) or polynomial features for non‑linear effects.
* Evaluate tree‑based models (Decision Tree, Random Forest, Gradient Boosting) for potentially better performance.
* Use cross‑validation for more robust performance estimates.
* Add unit tests / data validation steps to safeguard data quality.

---

## License

This repository is released under the MIT License. Update as appropriate for your project.

---

## Contact

If you have questions or suggestions, open an issue or contact the project owner.

*Generated README — feel free to edit this file in the notebook or on GitHub.*
