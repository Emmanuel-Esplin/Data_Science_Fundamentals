# Data Science Fundamentals

Jupyter notebooks covering the foundations of data science in Python: core Python, NumPy,
pandas and an introduction to machine learning with scikit-learn. They are learning projects
based on textbooks, online courses and practical experimentation.

## Notebooks

| # | Notebook | Topics |
|---|----------|--------|
| 01 | [NumPy Fundamentals](notebooks/01_numpy_fundamentals.ipynb) | Lists vs arrays, array creation, vectorised maths, ufuncs, indexing/slicing, reshaping, coin-flip and random-walk simulations |
| 02 | [pandas: HR Employee Attrition](notebooks/02_pandas_hr_attrition.ipynb) | `Series` and `DataFrame`, `.loc`/`.iloc`, summary statistics, recoding, boolean filtering, `groupby` comparisons |
| 03 | [Intro to Machine Learning](notebooks/03_intro_to_machine_learning.ipynb) | k-NN on iris, logistic regression and random forest classification, linear regression of house prices, train/test evaluation against baselines |
| 04 | [Python Basics and Arrays](notebooks/04_python_basics_and_arrays.ipynb) | Expressions and precedence, `int`/`float` limits, growth rates, strings, comparisons, NumPy arrays, approximating π |

Notebook 04 contains a few **intentional** errors and numeric edge cases (for example a
`SyntaxError` and float overflow). They are labelled in the notebook and demonstrate what
Python does in those situations.

## Getting started

Requires Python 3.10+.

```bash
git clone https://github.com/Emmanuel-Esplin/Data_Science_Fundamentals.git
cd Data_Science_Fundamentals
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter lab
```

Open the notebooks from the `notebooks/` folder. They read their datasets from `../data/`.
Random processes are seeded, so a fresh **Restart & Run All** reproduces the saved outputs.

## Data

| File | Used in | Source |
|------|---------|--------|
| `data/hr_employee_attrition.xlsx` | 02 | IBM HR Analytics Employee Attrition & Performance (fictional data created by IBM data scientists) |
| `data/student.csv` | 03 | [UCI Student Performance](https://archive.ics.uci.edu/dataset/320/student+performance) (Portuguese course), CC BY 4.0 |
| `data/house_train.csv` | 03 | [Kaggle House Prices: Advanced Regression Techniques](https://www.kaggle.com/c/house-prices-advanced-regression-techniques) (Ames, Iowa) |

The iris dataset in notebook 03 ships with scikit-learn.

## Related

More Python projects, including the matplotlib, housing EDA, student statistics and literary
text analysis work, are in [Python_Projects](https://github.com/Emmanuel-Esplin/Python_Projects).

## License

[MIT](LICENSE)
