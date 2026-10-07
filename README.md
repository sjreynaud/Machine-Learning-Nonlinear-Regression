**Project Overview**

This repository contains coursework for DDS8555 Predictive Analysis focused on exploring nonlinear machine learning methods for regression problems. The project combines theoretical concepts from Introduction to Statistical Learning with Applications in Python (ISLR) with practical implementation using real-world datasets and a Kaggle competition.

The analysis investigates how nonlinear techniques improve predictive performance compared to traditional linear models. Methods examined include polynomial regression, Random Forest Regression, and Gradient Boosting Regression. Model performance is evaluated through R² and Root Mean Squared Logarithmic Error (RMSLE) metrics, supported by exploratory data analysis, visualizations, residual diagnostics, and Kaggle leaderboard results.

**Learning Objectives**

  - Apply nonlinear regression methods to real datasets.
  - Examine basis functions and piecewise regression concepts.
  - Compare linear and polynomial regression models.
  - Implement ensemble machine learning algorithms.
  - Evaluate predictive performance using appropriate metrics.
  - Interpret model diagnostics and assumptions.
  - Participate in a Kaggle machine learning competition.
  - Document results using APA 7 academic standards.
    
**Repository Structure**

Machine-Learning-Nonlinear-Regression
│
├── README.md
├── LICENSE
├── .gitignore
│
├── reports
│ ├── Assignment4_Report.pdf
│ └── Assignment4_Report.docx
│
├── notebooks
│ ├── 01_Conceptual_Question_3.ipynb
│ ├── 02_Applied_Question_8_Auto_Dataset.ipynb
│ ├── 03_Random_Forest_Abalone.ipynb
│ └── 04_Gradient_Boosting_Abalone.ipynb
│
├── src
│ ├── auto_polynomial_regression.py
│ ├── random_forest_regression.py
│ ├── gradient_boosting_regression.py
│ └── utils.py
│
├── data
│ ├── raw
│ └── processed
│
├── figures
│ ├── nonlinear_relationships/
│ ├── residual_diagnostics/
│ └── kaggle_results/
│
├── submissions
│ ├── submission_random_forest.csv
│ └── submission_gradient_boosting.csv
│
├── results
│ ├── model_metrics.csv
│ └── kaggle_scores.csv
│
├── documentation
│ ├── assignment_instructions.pdf
│ ├── model_reports/
│ └── supporting_materials/
│
└── references
└── references.md

**Conceptual Question #3: Basis Functions**

A piecewise nonlinear regression model was constructed using basis functions:

b1(X)=Xb_1(X)=Xb1​(X)=X b2(X)=(X−1)2I(X≥1)b_2(X)=(X-1)^2I(X\ge1)b2​(X)=(X−1)2I(X≥1)

The resulting fitted curve demonstrates how basis functions can introduce nonlinearity while maintaining continuity. The model behaves linearly for values below the knot point and transitions into a downward-opening quadratic function for values greater than or equal to one.

**Key Concepts**

Basis Functions
Piecewise Regression
Spline Foundations
Nonlinear Transformations
Model Interpretation

**Applied Question #8: Auto Dataset**

**Objective**

Investigate whether nonlinear relationships exist between automobile characteristics and fuel efficiency (MPG).

**Models Evaluated**

**Model	                         R² Score**
Linear Regression	0.6059
Polynomial Regression (Degree 2)	0.6876
Polynomial Regression (Degree 3)	0.6882

**Findings**

Polynomial regression substantially improved model performance relative to simple linear regression. Scatterplots and residual diagnostics indicated nonlinear relationships between horsepower and MPG, supporting the use of nonlinear modeling approaches.

**Conclusion**

The Degree 3 Polynomial Regression model provided the strongest fit, explaining approximately 68.8% of the variability in fuel efficiency.

**Kaggle Competition: Regression with Abalone Dataset**
**Competition**

Playground Series S4E4: Regression with an Abalone Dataset

**Model 1: Random Forest Regression**

**Model Parameters**

  - 500 Trees
  - Minimum Samples Leaf = 2
  - Random State = 42

**Validation Performance**

RMSLE = 0.15395

**Strengths**
  - Handles nonlinear relationships naturally
  - Captures complex feature interactions
  - Robust against overfitting

**Model 2: Gradient Boosting Regression**

**Model Parameters**

  - 600 Estimators
  - Learning Rate = 0.05
  - Maximum Depth = 3
  - Subsample = 0.90

**Validation Performance**

RMSLE = 0.14936

**Strengths**

  - Sequential error correction
  - High predictive accuracy
  - Effective for structured tabular datasets
    
**Kaggle Submission Results**

Two nonlinear machine learning models were successfully submitted to the Kaggle competition. The Gradient Boosting Regression model produced the strongest leaderboard performance, achieving a Public Score of 0.14964 and a Private Score of 0.14911. The Random Forest Regression model achieved a Public Score of 0.15643 and a Private Score of 0.15754. These results demonstrate that Gradient Boosting captured the underlying nonlinear relationships more effectively and provided the highest level of predictive accuracy among the evaluated models.

<img width="587" height="156" alt="image" src="https://github.com/user-attachments/assets/2b59bc55-84e2-41a5-8a00-c6399fd94b2e" />


**🏆 Best Performing Model: Gradient Boosting Regression**

Technologies Used
Python
Pandas
NumPy
Scikit-learn
Matplotlib
Seaborn
ISLP Package
Jupyter Notebook
Kaggle
Key Machine Learning Concepts
Exploratory Data Analysis (EDA)
Feature Engineering
Label Encoding
Polynomial Regression
Ensemble Learning
Random Forests
Gradient Boosting
Residual Diagnostics
Model Validation
RMSLE Evaluation Metric

**References**

James, G., Witten, D., Hastie, T., & Tibshirani, R. (2023). An Introduction to Statistical Learning with Applications in Python (2nd ed.). Springer.

Little, R. J. A., & Rubin, D. B. (2019). Statistical Analysis with Missing Data (3rd ed.). Wiley.

Tukey, J. W. (1977). Exploratory Data Analysis. Addison-Wesley.

**Author**

Sidney Reynaud
 M.S. Data Analytics (AWS Cloud Computing)
 Ph.D. Data Science Researcher
 Clinical Analytics • Predictive Modeling • Machine Learning • Data Governance
