# 🐄 Predicting Livestock Feeding Expenses from Species Inventory

## Author: Christian Amaro – INEGI

## 📊 Project Overview

This project demonstrates how to predict livestock feeding expenses (CG111_01) using species inventory data. The workflow includes data cleaning, outlier detection, regression modeling using training and testing datasets, and species-specific analyses to improve predictive accuracy.

Key goals:

- Predict feeding expenses based on livestock species and inventory.

- Identify and handle outliers to reduce bias and improve reliability.

- Apply transformations to improve normality and reduce skewness.

- Build and optimize multiple linear regression models.

- Implement species-specific models to account for behavioral differences.

Note: Initial model results did not meet expected predictive performance, highlighting the need to develop more robust models for accurate predictions.

## 🔍 Workflow

Data Loading & Preprocessing

Import Excel datasets and clean missing values.

Rename variables for clarity.

Create subsets for specific livestock species.

Exploratory Data Analysis (EDA)

Correlation matrices and boxplots to analyze distributions.

Logarithmic transformations for skewed variables.

Outlier Detection

K-means clustering with ±3 standard deviations.

Interquartile range (IQR) criterion.

Visualizations and optional removal for cleaner datasets.

Regression Modeling

Multiple linear regression on training (80%) and test (20%) data.

Residual analysis for linearity, normality, and homoscedasticity.

Model Optimization

Stepwise selection using Akaike Information Criterion (AIC).

Bidirectional and backward methods to select relevant variables.

Prediction & Evaluation

Generate predictions on test data and compare with actual values.

Evaluate performance visually and statistically.

Species-Specific Modeling

Build separate models for bovine, ovine, and other species.

Select variables relevant to each species to improve predictive accuracy.

## 💡 Key Skills & Techniques

- Data cleaning, preprocessing, and handling missing values in R.

- Exploratory data analysis and visualization (ggplot2, corrplot).

- Outlier detection using clustering and IQR methods.

- Logarithmic transformations for normalization.

- Multiple linear regression, residual analysis, and assumption checking.

- Stepwise model optimization using AIC.

- Train-test splitting and predictive evaluation.

- Species-specific modeling for better accuracy.

- Reproducible workflow with RMarkdown documentation.

## 🛠 Technologies

Language: R

Packages: dplyr, tidyverse, readxl, ggplot2, caTools, cluster, KMEANS.KNN, corrplot, quantreg, rpart, rpart.plot, randomForest, factoextra, patchwork, writexl, MASS

## 📁 Repository Structure

data/ – raw and simulated Excel datasets

scripts/ – RMarkdown scripts with full workflow

- modelos.Rmd – analysis and results in Spanish

- models_eng.Rmd – analysis and results in English

outputs/ – visualizations, tables, and model summaries

- modelos.html
  
- modelos-eng.html

README.md – project overview and methodology

## ✅ Conclusion

This project demonstrates how to predict livestock feeding expenses using inventory data, handle outliers, optimize models, and apply species-specific analyses. While initial model results did not achieve the expected performance, the workflow sets the foundation for developing more robust models to improve predictive accuracy. 

Note: Two versions of the workflow are included in the repository: modelos.Rmd in Spanish and models_eng.Rmd in English, allowing users to review results in their preferred language.
