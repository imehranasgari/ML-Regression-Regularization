# Regularization Regression

## Problem Statement
The project aims to explore and implement regularization techniques, specifically Ridge and Lasso Regression, to address potential issues like overfitting in linear regression models. The goal is to find optimal model parameters that balance model fit and complexity.

## Solution Approach
The solution involves applying Ridge and Lasso Regression, which are regularized versions of linear regression. These methods add a penalty term to the cost function to shrink model weights, thereby preventing overfitting.

**Key steps include:**
*   **Data Loading and Preprocessing:** Loading the `Advertising.csv` dataset and dropping the `Unnamed: 0` column.
*   **Exploratory Data Analysis:** Visualizing the relationship between advertising expenditures (TV, Radio, Newspaper) and Sales using scatter plots.
*   **Linear Regression Baseline:** Establishing a baseline performance using standard Linear Regression with 5-fold cross-validation to calculate the Mean Squared Error (MSE).
*   **Ridge Regression Implementation:**
    *   Utilizing `GridSearchCV` to find the optimal `alpha` (regularization strength) for Ridge Regression.
    *   Performing 5-fold cross-validation to evaluate different `alpha` values.
*   **Lasso Regression Implementation:**
    *   Similarly, employing `GridSearchCV` to determine the optimal `alpha` for Lasso Regression.
    *   Conducting 5-fold cross-validation for parameter tuning.

## Technologies & Libraries
*   **Python**
*   **NumPy**: For numerical operations.
*   **Pandas**: For data manipulation and analysis.
*   **Matplotlib**: For creating static, interactive, and animated visualizations.
*   **Seaborn**: For statistical data visualization.
*   **Scikit-learn**: For machine learning models and utilities, including:
    *   `LinearRegression`
    *   `Ridge`
    *   `Lasso`
    *   `GridSearchCV`
    *   `cross_val_score`

## Installation & Execution Guide

1.  **Clone the repository:**
    ```bash
    git clone <repository_url>
    cd Regularization_Regression
    ```

2.  **Install dependencies:**
    ```bash
    pip install numpy pandas matplotlib seaborn scikit-learn
    ```

3.  **Run the Jupyter Notebook:**
    ```bash
    jupyter notebook Regularization_Regression.ipynb
    ```
    Execute the cells sequentially within the notebook to perform data loading, visualization, model training, and evaluation.

## Key Results / Performance

**Linear Regression (Baseline):**
*   Mean Negative Mean Squared Error (MSE): \$-3.07294659710021\$

**Ridge Regression:**
*   Optimal `alpha` parameter: \$$20\$
*   Best Mean Negative Mean Squared Error (MSE): \$-3.072671338341143\$

**Lasso Regression:**
*   Optimal `alpha` parameter: \$$1\$
*   Best Mean Negative Mean Squared Error (MSE): \$-3.041405896751369\$

# **Author:** mehran Asgari
## **Email:** [imehranasgari@gmail.com](mailto:imehranasgari@gmail.com).
## **GitHub:** [https://github.com/imehranasgari](https://github.com/imehranasgari).

---

## 📄 License

This project is licensed under the MIT License – see the `LICENSE` file for details.