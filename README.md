# Movie-Rating-Predictor-Project
## Introduction

The movie industry relies on informed decisions to ensure success, from casting to production choices. In this project, we predict movie ratings using features such as genres, keywords, cast, crew, and production metadata. We preprocess these features into numerical representations and train Machine Learning (ML) and Deep Learning (DL) models.

Our results show that attention-based DL models achieve the best performance, with an MSE of 0.43 and an $R^2$ score of 0.743. However, ML models like Random Forest Regression are competitive, achieving an MSE of 0.45 and an $R^2$ score of 0.732. This highlights the potential of both ML and DL approaches for guiding decisions in film production.

---

## Models Implemented

1. Bayesian Ridge Regression (Benchmark)
2. Support Vector Regression (SVR)
3. Random Forest Regression
4. PCA-Based Multi-Layer Perceptron (MLP)
5. PCA-Based Attention Model
6. Multi-Layer Perceptron (MLP)
7. Attention-Based Deep Learning Model

---
## File Description
1. EE 541 Model Card.pdf: Summarize the Model and provide key information about our model.
2. EE541_data_creater.ipynb: Import the dataset from Kaggle, and create the files needed for the movie predictors.
3. EE541_project_rating_movies_5000Version_ablation_study.ipynb: Movie Rating Predictors, ablation study.
5. EE541_project_rating_movies_full_dataset.ipynb: Movie Rating Predictors, trained on the entire movie dataset.

---

## Usage
Use data_creater.ipynb to create and split the dataset into training/validation/test. Then run the movie_rating ipynb files accordingly to generate results. 

---

## Results from Training on 50,000 Movies

| **Model**                 | **MSE**  | **R²**   |
|---------------------------|----------|----------|
| Bayesian Ridge            | 0.5501   | 0.6728   |
| Support Vector Regression | 0.4523   | 0.7309   |
| Random Forest Regression  | 0.4497   | 0.7325   |
| PCA-MLP                   | 0.4638   | 0.7241   |
| PCA-Attention             | 0.4380   | 0.7395   |
| MLP                       | 0.4375   | 0.7398   |
| Attention                 | 0.4313   | 0.7434   |

---

## Key Findings

- **Best Model**: Attention-based DL model with an MSE of 0.43 and $R^2$ of 0.743.
- **Competitive ML Model**: Random Forest Regression with an MSE of 0.45 and $R^2$ of 0.732.
- **Scalability**: PCA-based models provide efficient alternatives for large datasets.

---

## Team Members

- **Frank Yan**  
  *University of Southern California*  
  yanfrank@usc.edu

- **Timing Yang**  
  *University of Southern California*  
  timingya@usc.edu

---

## Author Contributions and Attribution

This project was completed as part of the EE541 Machine Learning course at the University of Southern California.

### Contributions by Frank Yan

Frank Yan implemented the following components of the project:

- Data preprocessing and feature engineering pipeline
- Parsing and transforming categorical movie metadata (genres, keywords, cast, crew, production data) into numerical representations
- Feature compression strategy for high-dimensional categorical features
- Implementation of Machine Learning models:
  - Bayesian Ridge Regression
  - Support Vector Regression (SVR)
  - Random Forest Regression

### Contributions by Timing Yang

Timing Yang contributed to the overall project design and collaborated on experimentation and evaluation of the models.

- Experimentation with different dataset sizes and ablation studies
- Implementation of Deep Learning models in PyTorch:
  - Multi-Layer Perceptron (MLP)
  - Attention-based neural network
  - PCA-based model variants
  
### External Libraries and Tools

This project uses several open-source libraries:

- **Python**
- **NumPy**
- **Pandas**
- **Scikit-learn**
- **PyTorch**
- **Matplotlib**

All model implementations build upon these libraries' standard APIs.

### Dataset Attribution

The dataset used in this project is the **The Movies Dataset** available on Kaggle:

https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset

This dataset contains metadata for approximately 50,000 movies including genres, keywords, cast, crew, production information, and user ratings.

All data used in this project is publicly available.

---
