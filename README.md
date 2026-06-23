# Applied Numerical Methods

> Numerical methods applied to Instacart grocery order data in Python

![Python](https://img.shields.io/badge/Python-0a7?style=flat-square) ![pandas](https://img.shields.io/badge/pandas-0a7?style=flat-square) ![NumPy](https://img.shields.io/badge/NumPy-0a7?style=flat-square) ![statsmodels](https://img.shields.io/badge/statsmodels-0a7?style=flat-square) ![scikit-learn](https://img.shields.io/badge/scikit--learn-0a7?style=flat-square) ![SciPy](https://img.shields.io/badge/SciPy-0a7?style=flat-square) ![SymPy](https://img.shields.io/badge/SymPy-0a7?style=flat-square) ![seaborn](https://img.shields.io/badge/seaborn-0a7?style=flat-square) ![matplotlib](https://img.shields.io/badge/matplotlib-0a7?style=flat-square) ![Jupyter Notebook](https://img.shields.io/badge/Jupyter_Notebook-0a7?style=flat-square) 

### 🌐 Live project page → **https://selsaady1.github.io/mat421-numerical-methods/**

## Overview
A MAT 421 (Applied Computational Methods) course project analyzing the Instacart Market Basket dataset with numerical and statistical methods in Python. Delivered as a Jupyter notebook (exported to HTML) plus a written project plan, it cleans and merges the relational order files, builds linear regression models relating reorders to products, and inspects model assumptions through residual and distribution diagnostics. A symbolic differentiation step is used to analyze the rate of change of a published prediction equation.

**Highlight:** OLS regression R-squared = 0.742

## Key Achievements
- Merged and aggregated the multi-file Instacart relational dataset (orders, prior order-products, products, departments, aisles) with pandas, computing per-order product counts and per-product reorder totals across roughly 3.2 million order-product rows
- Fit an OLS linear regression of products on reorders using statsmodels and a 500-user training sample, achieving an R-squared of 0.742 with a fitted slope of 1.093 and intercept of 3.589
- Reproduced the regression coefficients by hand using NumPy (least-squares slope/intercept formulas) to confirm the statsmodels output
- Diagnosed the fit with residual analysis, a QQ plot, a kernel-density residual distribution against a fitted normal, and fit plots, concluding the data is right-skewed
- Applied symbolic differentiation with SymPy to a published quadratic prediction equation to obtain its derivative (rate of change)
- Visualized data distributions with seaborn/matplotlib (product-frequency histogram, days-since-prior-order histogram)

## Approach
The notebook works through four stated problems: data preparation/visualization, linear regression and linear equations, residual and distribution analysis, and differentiation/optimization. It uses pandas to merge and reshape the relational files, statsmodels and scikit-learn for OLS regression, scipy/statsmodels for diagnostic plots, and SymPy for symbolic differentiation. Conclusions are drawn from the regression fit statistics and the diagnostic graphics.

## Tools & Technologies
- Python
- pandas
- NumPy
- statsmodels
- scikit-learn
- SciPy
- SymPy
- seaborn
- matplotlib
- Jupyter Notebook

## Repository Structure
```
.gitignore
LICENSE
README.md
docs/Elsaady_MAT421_PROJECT_1_.html
docs/Elsaady_Projectplan.pdf
images/preview.png
```

## Results
The OLS model relating reorders to products reached R-squared = 0.742 (slope 1.093, intercept 3.589) on the 500-user sample, indicating a strong positive linear relationship, with residual diagnostics showing a right-skewed distribution; full analysis is in docs/Elsaady_MAT421_PROJECT_1_.html.

## Deliverable
See [`docs/Elsaady_MAT421_PROJECT_1_.html`](docs/Elsaady_MAT421_PROJECT_1_.html).

## License
MIT — see [`LICENSE`](LICENSE).

---
_Part of [Saif Elsaady's engineering portfolio](https://selsaady1.github.io/portfolio/). Deliverables only — routine homework/quizzes/exams excluded._