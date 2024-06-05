# crop-recommender
Sure! Here’s a comprehensive README for your crop recommendation system project:

---

# Crop Recommendation System

## Overview

The Crop Recommendation System is a machine learning-based project aimed at helping farmers determine the most suitable crops for their land. By analyzing various soil and environmental attributes, the system provides crop recommendations to optimize yield and promote sustainable farming practices.

## Table of Contents

1. [Introduction](#introduction)
2. [Dataset](#dataset)
3. [Preprocessing](#preprocessing)
4. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
5. [Feature Engineering](#feature-engineering)
6. [Modeling](#modeling)
7. [Evaluation](#evaluation)
8. [Installation](#installation)
9. [Usage](#usage)
10. [Results](#results)
11. [Contributing](#contributing)
12. [License](#license)
13. [Contact](#contact)

## Introduction

Agriculture plays a vital role in the global economy, and choosing the right crop for specific soil and environmental conditions can significantly impact productivity and sustainability. This project leverages machine learning to build a crop recommendation system that predicts the optimal crop for a given set of soil attributes.

## Dataset

The dataset used in this project is sourced from Kaggle and contains the following attributes:
- **Nitrogen** (N)
- **Phosphorus** (P)
- **Potassium** (K)
- **Temperature** (°C)
- **Humidity** (%)
- **pH Value**
- **Rainfall** (mm)
- **Crop** (Target variable)

The dataset includes 2200 samples, each representing a unique combination of soil and environmental attributes.

## Preprocessing

- **Handling Missing Values**: The dataset contains no missing values.
- **Handling Duplicates**: There are no duplicate rows in the dataset.
- **Outlier Detection**: Outliers are detected and capped at 1.5 times the interquartile range (IQR).
- **Standardization**: All numerical features are standardized using `StandardScaler`.
- **Encoding**: The target variable (crop) is label-encoded.

## Exploratory Data Analysis (EDA)

- **Univariate Analysis**: Distribution of individual features and detection of outliers.
- **Multivariate Analysis**: Correlation heatmap to identify relationships between features.

## Feature Engineering

- **Outlier Treatment**: Outliers are capped to reduce their impact on the model.
- **Standardization**: Features are standardized to have zero mean and unit variance.

## Modeling

- **Algorithm**: Logistic Regression is used for initial modeling.
- **Hyperparameter Tuning**: RandomizedSearchCV is used to find the optimal hyperparameters (`C` and `penalty`).

## Evaluation

- **Accuracy**: The model achieves 98.8% accuracy on both training and testing sets.
- **Classification Report**: Detailed performance metrics including precision, recall, and F1-score for each crop class.

## Installation

To run this project locally, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/ishola-faazele/crop-recommendation-system.git
   ```
2. **Navigate to the project directory**:
   ```bash
   cd crop-recommendation-system
   ```
3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. **Prepare the data**: Ensure the dataset is placed in the same directory as the .ipynb file.

## Results

The model provides accurate crop recommendations based on the input soil and environmental attributes. Key results include:
- High accuracy of 98.8%
- Effective handling of outliers and feature standardization
- Optimized hyperparameters for the logistic regression model

## Contributing

Contributions are welcome! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature-branch
   ```
3. Make your changes and commit them:
   ```bash
   git commit -m 'Add new feature'
   ```
4. Push to the branch:
   ```bash
   git push origin feature-branch
   ```
5. Create a pull request.

## Contact

For any questions or suggestions, please contact:

- Name: Ishola Faazele Adebiyi
- Email: faazeleishola2030@gmail.com
- LinkedIn: https://www.linkedin.com/in/faazele-ishola-46b334252/

---

By following this README, users and collaborators can easily understand the purpose of your project, set it up locally, and contribute to its development.
