# Pokémon Type Prediction (R)

This repository contains an analysis and predictive modeling project that classifies Pokémon types based on various numeric and categorical features. Though implemented in a `.ipynb` Jupyter notebook, all code is written in R using the IRKernel.

## 🧪 Project Overview

The objective of this project is to predict a Pokémon's primary type (e.g., Water, Fire, Grass) using features such as stats, generation, and resistance against other types. The dataset includes 801 Pokémon entries with 41 features.

Two machine learning models were used:
- **CART (Classification and Regression Trees)** for interpretability.
- **Random Forest** for better accuracy and generalization.

The models achieved the following:
- **CART Accuracy**: ~83.1%
- **Random Forest Accuracy**: ~93.1%

## 📊 Features & Methods

- **Data Cleaning**: Removed high-cardinality or low-informative features (e.g., names, abilities), handled missing values via imputation.
- **Exploratory Data Analysis**: Assessed feature correlation, distribution by generation/type, and legendary status.
- **Modeling**: Applied decision trees and ensemble techniques to handle outliers and feature noise.
- **Evaluation**: Compared accuracy and interpretability between CART and Random Forest using confusion matrices and OOB error.

## 📁 File Structure

- `pokemon_model.ipynb` – Jupyter Notebook with R kernel code and analysis
- `pokemon.csv` – Pokemon Dataset

## 📌 Requirements

- R (>= 4.0)
- IRKernel (for running R in Jupyter)
- Packages: `rpart`, `randomForest`, `ggplot2`, `dplyr`, `tidyr`, etc.

## 🧠 Insights

- Random Forest outperformed CART in accuracy.
- High cardinality categorical features were excluded to prevent model bloat.
- Further improvements possible via feature engineering of excluded columns.
