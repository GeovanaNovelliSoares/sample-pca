# Student Disciplines' Grades: Factorial Analysis & Dimensionality Reduction (PCA)

This repository presents a comprehensive case study on the application of **Factor Analysis (FA)** using the **Principal Component Analysis (PCA)** method. The goal is to transform a dataset of academic grades into independent latent dimensions, allowing for a deeper analysis of student profiles.

## 📖 Use Case Scenario

In this scenario, we analyze students' grades in four disciplines (features). Instead of a traditional clustering analysis (where we group similar observations), we apply Factor Analysis to:

1. **Consolidate Features:** Merge correlated disciplines into orthogonal components (independent axes).
2. **Dimensionality Reduction:** Minimize the number of analytical axes (from 4 to 2 or 3) while maintaining the maximum original variance.
3. **Identify Latent Constructs:** Reveal hidden affinities between disciplines that are not obvious through simple averages alone.

---

## 🧬 Mathematical Foundation and Pipeline

The project follows a rigorous statistical pipeline based on standardized data (**Z-score**):

* **Pearson Correlation Matrix:** The basis for calculating the determinant and the characteristic polynomial equation.
* **Eigenvalues:** Extracted as roots of the polynomial equation, they represent the absolute variance intrinsic to each component. The retention criterion is based on relative variance (Explained/Total).
* **Eigenvectors:** Coefficients that determine the weight of each original variable in the composition of the new axis.
* **Loadings:** The product of the variable's weight and the square root of the component's eigenvalue, representing the correlation between the variable and the factor.
* **Communalities:** A measure of how much of the original variance of each discipline was preserved after discarding less representative components.

---

## 🛠️ Tech Stack

The project utilizes an advanced ecosystem of Python libraries for scientific computing and multivariate analysis:

* **Processing:** `Pandas`, `NumPy`, `SciPy`, `Scikit-learn`.
* **Advanced Statistics:** `Factor-Analyzer` (extraction and rotation), `Pingouin` (hypothesis testing and correlation).
* **Symbolic Algebra:** `SymPy` (calculation of characteristic polynomials).
* **Visualization:** `Matplotlib`, `Seaborn`, `Plotly`.

---



## 🚀 Main Utilities of this Technique

* **Feature Engineering:** Reducing multicollinearity for regression models.
* **Data Summarization:** Summarizing large volumes of variables into interpretable indices.
* **Ranking & Scoring:** Creating rankings based on the weighted sum of factor scores by relative variance.
* **Data Cleaning:** Identifying and discarding "noise" through uniqueness analysis.

---

## 📊 How to Interpret the Results

1.  **Loadings Matrix:** Identifies the "signature" of each factor (e.g., Factor 1 focused on STEM, Factor 2 on Humanities).
2.  **Scree Plot / Variance Table:** Determines the ideal cutoff point for factor retention.
3.  **Factor Scores:** The new coordinates for each student in the reduced multidimensional space.

---

**Project Status:** Completed ✅  
**Key Skills Demonstrated:** Linear Algebra, Multivariate Statistics, Unsupervised Machine Learning.
