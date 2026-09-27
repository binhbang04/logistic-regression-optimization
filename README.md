# Logistic Regression Optimization: Gradient Descent vs Newton's Method

## Overview
This project implements and compares two optimization algorithms for **Logistic Regression** — **Gradient Descent** and **Newton's Method** — applied to a heart disease classification task.

## Dataset
- **Heart Disease Dataset** (`heart.csv`) — 303 samples with 13 clinical features
- **Target**: Binary classification (presence/absence of heart disease)

## Methodology

### 1. Data Preprocessing
- Feature-target separation
- Train/test split (80/20)
- Feature standardization using `StandardScaler`

### 2. Logistic Regression from Scratch
- Sigmoid activation function
- Binary Cross-Entropy loss function
- Gradient and Hessian computation

### 3. Optimization Algorithms
| Algorithm | Description | Iterations |
|-----------|-------------|------------|
| **Gradient Descent** | First-order method using gradient of loss function | 1,000 |
| **Newton's Method** | Second-order method using Hessian matrix | 20 |

### 4. Evaluation & Visualization
- Loss convergence comparison
- Classification accuracy on test set
- 3D surface plot of loss landscape with optimization trajectory

## Key Results
- Newton's Method converges significantly faster (fewer iterations) than Gradient Descent
- Both methods achieve comparable final accuracy
- Visual demonstration of convergence behavior on convex loss surface

## Tech Stack
- Python, NumPy, Pandas
- Scikit-learn (preprocessing & splitting)
- Matplotlib, Seaborn (visualization)

## Project Structure
```
├── code_optimization.ipynb    # Main analysis notebook
├── heart.csv                  # Dataset
├── report_optimization.pdf    # Detailed report
├── .gitignore
└── README.md
```

## How to Run
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
jupyter notebook code_optimization.ipynb
```
