# Synthetic-Data-Generation 
Generate realistic synthetic datasets while preserving the statistical essence of your original data.
### Code
https://colab.research.google.com/drive/1xzSm3cCDHfDcyKXIGVRe_bFETnb7XvXW?usp=sharing
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

## Results - 
#### This image shows the Gaussian Copula result for the column “Meaningfully Different Index.” The synthetic distribution closely overlaps with the original and the combined distribution, showing minimal deviation in both central tendency and spread.

 <img width="776" height="577" alt="image" src="https://github.com/user-attachments/assets/29b20c55-eba0-4097-827e-0e6eee1cad8b" />

#### This image shows the Gaussian Approximation result for the same column. Here, the synthetic distribution deviates more from the original, especially around the peak, and the combined distribution shows noticeable differences in shape as well.
 <img width="746" height="596" alt="image" src="https://github.com/user-attachments/assets/3f72a91d-bceb-4fe8-b142-0898e9d53841" />

#### Same pattern is seen for all the columns. Hence Gaussian Copula Method is preferred.

## Conclusion - 
Gaussian Copulas give better results because they capture relationships between variables more accurately, even if each variable’s distribution is different.
They separate the dependency structure from the marginal distributions, allowing more flexibility. This means you can model complex, real-world correlations that normal methods (like assuming everything is Gaussian) might miss

















