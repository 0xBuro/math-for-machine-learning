# Applied Mathematics for Engineers

This repository contains my solutions, mathematical derivations, and numerical implementations for **Applied Mathematics in Data Science**

Aims to bridge the gap between theoretical linear algebra and its practical application in **Machine Learning Engineering**.

## Structure and Key-Learnings

#### exercise_1/ - Linear Algebra Foundations
*Focus: The geometry of vector spaces and high-dimensional planes.*
- **Vector Norms & Geometry:** Proofs regarding the triangle inequality and collinearity conditions in R^n.
- **Linear Systems:** Solving 4x4 systems using Gaussian Elimination and LU Decomposition.
- **Hyperplanes:** Deriving the Hessian Normal Form (HNF) in R^4 — a fundamental concept for understanding decision boundaries in Support Vector Machines (SVM).

#### exercise_2/ - Matrix Calculus & Computational Efficiency
*Focus: Matrix operations, rank analysis, and algorithmic complexity.*
- **Dimensions & Compatibility:** Analyzing matrix-matrix and matrix-vector products to prevent dimension mismatches in neural network layers.
- **Computational Efficiency:** Mathematical proof of why x(yᵀz) is superior to (xyᵀ)z (O(n) vs O(n²) complexity).
- **Rank & Singularity:** Using rank determination to identify redundant features and multicollinearity in datasets.
- **Matrix Inversion:** Inverting matrices via Gauss-Jordan and identifying singular matrices where det(A) = 0.
- 
## Stack

- **Mathematics:** Linear Algebra, Vector Calculus, Optimization.
- **Typesetting:** LaTeX (Local TeX Live environment).
- **Programming:** Python 3.x (NumPy for numerical verification).
- **Editor:** VSCodium with LaTeX Workshop.
- **Version Control:** Git & GitHub.

## Reference & Literature

The problems and theoretical foundations are based on the textbook:

- **Burg, K., Haf, H., Wille, F., & Meister, A.** _Höhere Mathematik für Ingenieure, Band II: Lineare Algebra._ Springer Vieweg. [Link to Springer](https://link.springer.com/book/10.1007/978-3-8348-2267-3)

This book provides a rigorous approach to vector spaces, which serves as the mathematical backbone for studies in Data Science.

## ML Notes & Roadmap for me

Integrating these mathematical concepts into the ML workflow:

* **Support Vector Machines (SVM):** The Hessian Normal Form is the mathematical basis for defining decision boundaries and calculating the margin between classes.
* **Numerical Stability:** Utilizing optimized solvers (like LAPACK/BLAS) via NumPy is crucial for large-scale training to avoid floating-point errors common in manual Gaussian elimination.
* **Computational Complexity:** Understanding matrix associativity (O(n) vs O(n²)) is essential for optimizing custom layers in Deep Learning and handling High-Dimensional data.
* **Feature Engineering:** Matrix Rank analysis helps identify redundant features (multicollinearity). Techniques like SVD utilize Low-Rank Approximation for data compression and noise reduction.
* **Regularization:** When matrices are singular (det = 0), models become unstable. This necessitates the use of the Moore-Penrose Pseudoinverse or Regularization (Ridge/Lasso) to ensure convergence.
