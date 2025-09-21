# Milestone Assignment 2: Principal Component Analysis (PCA)

## Project Description

This project is a data analysis assignment for the Anderson Cancer Center, where the goal is to develop a predictive model to address the growing number of referrals. The first step involves using **Principal Component Analysis (PCA)** to identify essential variables for securing donor funding. The project demonstrates how PCA can effectively reduce data dimensionality while retaining critical information, and it utilizes a logistic regression model for prediction on the reduced data.

---

## Assignment Tasks

1.  **PCA Implementation:** Apply PCA to the breast cancer dataset from `sklearn.datasets` to identify essential variables.
2.  **Dimensionality Reduction:** Reduce the dataset's dimensionality to two principal components (PC1 and PC2).
3.  **Logistic Regression (Bonus):** Implement a logistic regression model on the PCA-reduced data to perform a classification task.

---

## Analysis and Results

### 1. PCA Implementation
PCA was successfully performed on the breast cancer dataset. The analysis revealed that the first two principal components capture **63.24% of the total variance**, making them highly effective representations of the original 30 features.

-   **PC1:** The most influential variables are `mean concave points`, `mean concavity`, and `worst concave points`.
-   **PC2:** The most influential variables are `mean fractal dimension`, `fractal dimension error`, and `worst fractal dimension`.

### 2. Dimensionality Reduction
The dataset was successfully reduced from its original shape of `(569, 30)` to `(569, 2)`. The 2D projection shown in the plot below illustrates the clear separation of the two target classes, `malignant` and `benign`, in the new feature space. 

### 3. Logistic Regression
A logistic regression model was trained on the PCA-reduced data. This model achieved an impressive **accuracy of 94.74%** on the test set, demonstrating that even with a significant reduction in dimensionality, a predictive model can still perform exceptionally well.

A decision boundary plot visually confirms the model's ability to classify the data points effectively. 

---

## How to Run the Code

1.  Make sure you have all the necessary Python libraries installed.
    ```bash
    pip install numpy pandas scikit-learn matplotlib
    ```
2.  Open and run the `Milestone Assignment 2.ipynb` notebook in a Jupyter environment.
3.  Execute each cell sequentially. The output and plots will be generated in the notebook.
