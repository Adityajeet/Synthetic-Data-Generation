# Synthetic-Data-Generation
Generate realistic synthetic datasets while preserving the statistical essence of your original data.
## Introduction
This project focuses on generating synthetic data from the training dataset provided in the "Data" sheet. The goal is to ensure that the synthetic dataset accurately reflects key statistical properties of the original data, including mean, variance, distribution patterns, and inter-variable relationships. A comparative analysis of synthetic data, actual data, and the combined (actual + synthetic) dataset is also done.
## Methods Used for Comparative Analysis
### Gaussian Approximation- 
- It is simple and efficient for datasets following a normal distribution.
- It captures key statistical properties such as mean and variance accurately.
- It works well when relationships between variables are mostly linear.
#### Process Flow Diagram -
<img width="495" height="218" alt="image" src="https://github.com/user-attachments/assets/dc98224a-92bb-44e3-8a9b-b7f7e1020440" />

### Gaussian Copula-
- It preserves complex dependencies between variables beyond linear correlation.
- It produces more realistic synthetic data when the dataset is not perfectly Gaussian.
#### Process Flow Diagram -
<img width="1007" height="216" alt="image" src="https://github.com/user-attachments/assets/e848d83c-3972-44e6-b1bf-e4c54dcc67b2" />
















