# Python-Multiple-linear-regression-omitted-variable-bias-multicollinearity-and-hypothesis-testing
This repository contains a Python-based econometric analysis demonstrating multiple linear regression, omitted variable bias, multicollinearity, and hypothesis testing using synthetic data. All computations and interpretations are contained in the notebook
Overview

The project replicates an exam-style econometrics workflow:

Build and interpret OLS regression models.

Examine the effects of omitting relevant variables.

Detect multicollinearity using correlation matrices and VIF.

Perform t-tests and construct confidence intervals.

Tools Used

Python 3.9+

pandas – data handling

statsmodels – regression estimation

matplotlib / seaborn – plotting and visualization

scipy.stats – statistical inference

Analysis Summary
1. Baseline Model

Model:

- Education coefficient ≈ **15.83** → Each extra year of education raises the dependent variable by ~15.83, holding other factors constant. --- ### **2. Omitted Variable Bias** Removing Age reduces the Education coefficient to **≈ 2.98**, showing that **Age and Education are positively correlated**. This demonstrates **omitted variable bias** — excluding relevant variables distorts the estimated effects. --- ### **3. Multicollinearity Check** - **Correlations:** 0.96–0.99 among predictors - **VIF values:** Education = 452, Experience = 2299, Age = 767 → Severe **multicollinearity**, meaning these regressors overlap heavily in explaining variation in \(Y\). Coefficient estimates become unstable and standard errors inflate. --- ### **4. Hypothesis Testing** t = 3.125, p = 0.197 → **Fail to reject H₀** Education is **not statistically significant** at the 5% level. --- ### **5. Confidence Interval** 95% CI for Education’s effect: **(-7.67, 12.67)** Since 0 lies within this range, Education remains **insignificant** at 5%. --- ## File Structure ``` . ├── Econometrics Exam 2 code.pdf # Main notebook with results ├── README.md # Project documentation └── (optional folders for future data/figures) ``` --- ## Key Takeaways - Demonstrated full regression workflow with `statsmodels`. - Illustrated how **multicollinearity** and **omitted variables** affect inference. - Applied **t-tests** and **confidence intervals** for coefficient significance. - Reinforced reproducible econometric analysis using Python. --- ## Author **Qudus Bawa-Allah** Undergraduate | Applied Mathematics & Econometrics SUNY Brockport *Aiming toward quantitative finance & research applications.* --- Would you like me to generate a **formatted Markdown file (`README.md`)** that you can directly upload to GitHub (with proper headings, spacing, and emoji support)?
