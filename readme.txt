# Coordinate Descent Experiments(continuous optimization)

All experiments are implemented in Jupyter notebooks.
The core optimization and loss functions are shared across notebooks; each notebook differs only in the dataset and regularization setting.

---

## Experiment Setup

The experiments compare the following optimization algorithms:

- Gradient Descent (GD)
- Randomized Coordinate Descent (RCD)
- Accelerated Coordinate Descent (ACD, convex case only)

All methods are applied to logistic regression under:
- Strongly convex (L2 regularization)
- Nonconvex (smooth nonconvex regularization)

Two public datasets are used:
- A9a (sparse, high-dimensional)
- Covtype (dense, large-scale)


## Notebooks Overview

### `a9a-cd-convex.ipynb`
- Dataset: A9a
- Loss: Logistic loss with L2 regularization (strongly convex)
- Algorithms: GD, RCD, ACD
- Purpose: Study convergence and performance on sparse data in the convex setting

### `a9a-cd-nonconvex.ipynb`
- Dataset: A9a
- Loss: Logistic loss with smooth nonconvex regularization
- Algorithms: GD, RCD
- Purpose: Analyze the effect of coordinate sampling in nonconvex optimization

### `covtype-cd-convex.ipynb`
- Dataset: Covtype
- Loss: Logistic loss with L2 regularization (strongly convex)
- Algorithms: GD, RCD, ACD
- Purpose: Evaluate accelerated coordinate descent on dense, large-scale data

### `covtype-cd-nonconvex.ipynb`
- Dataset: Covtype
- Loss: Logistic loss with smooth nonconvex regularization
- Algorithms: GD, RCD
- Purpose: Test stability and convergence behavior of RCD under nonconvex settings

