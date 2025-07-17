## Green Hydrogen Evolution: Predictive Modeling of Membrane Reactor Efficiency

This repository contains the full implementation and report of a data science research project titled:

**“Green Hydrogen Evolution: Predictive and Comparative Modeling of Membrane Reactor Efficiency Using Advanced Artificial Neural Networks”**

The project was submitted as part of the M.Tech in Data Science and Analytics at Cochin University of Science and Technology (CUSAT), 2025.

---

##  Project Overview

The goal of this project is to develop and compare various machine learning and deep learning models to predict the **efficiency of membrane reactors** used in **green hydrogen production**.

##  Objective

- Develop predictive models to estimate system efficiency of membrane reactors for hydrogen production.
- Compare traditional machine learning models with ANN architectures.
- Optimize models using hyperparameter tuning, clustering methods, and performance evaluation metrics.

---

### Models Used:
### 🔹 Traditional Machine Learning
- **Support Vector Regression (SVR)**
- **Random Forest**
- **XGBoost**
## 🔹 Artificial Neural Networks
- **Multilayer Perceptron (MLP)**
  - Multiple activation functions (ReLU, tansig, logsig)
  - Training algorithms (GD, GDM, GDX)
- **Radial Basis Function (RBF) Neural Network**
  - ✅ **Standard K-Means Clustering**
  - ✅ **Moving K-Means Clustering**
  - Tuned hyperparameters: spread values, number of centers

> ✅ **RBF network achieved the best generalization with R² = 0.9981 using Moving K-Means.**


##  Project Files

| File | Description |
|------|-------------|
| `data_set.csv` | Input dataset used for training and testing models |
| `Hyperparameter_tuning_ML.ipynb` | Machine Learning model development with hyperparameter tuning |
| `MLP.ipynb` | Implementation and tuning of Multilayer Perceptron model |
| `RBF.ipynb` | Implementation of RBF model with K-Means and Moving K-Means clustering |
| `Project_Report_SNEHA.pdf` | Final research report detailing methodology, results, and conclusions |

---

##  Dataset Description

**Input Features:**
- Membrane Area
- Mass Flow of Feed
- Lower Heating Value (LHV) of feed
- CH₄, CO₂, N₂, O₂ mole fractions
- Reactor Pressure
- Reactor Diameter

**Target Output:**
- System Efficiency (%)


##  Evaluation Metrics

- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score


##  Key Results

| Model            | RMSE    | MSE     | R² Score |
|------------------|---------|---------|----------|
| SVR              | 0.3889  | 0.1512  | 0.9870   |
| Random Forest    | 0.3889  | 0.0373  | 0.9968   |
| XGBoost          | 0.2260  | 0.0511  | 0.9887   |
| MLP (Best Model) | 0.0355  | 0.0018  | 0.9974   |
| RBF (Enhanced)   | 0.1454  | 0.0216  | 0.9981   |


##  How to Run the Project

### Step 1: Clone this Repository

```bash
git clone https://github.com/snehakp1/green-hydrogen-modeling.git
