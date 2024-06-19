
# Baby Names Analysis

This repository contains a project aimed at analyzing baby names data from various states in the US, with a focus on Colorado. The project uses machine learning models to predict what baby names my wife will like.

## Table of Contents

- [Introduction](#introduction)
- [Data Preprocessing](#data-preprocessing)
- [Feature Engineering](#feature-engineering)
- [Model Training](#model-training)
- [Usage](#usage)

## Introduction

This project aims to analyze baby names data from various states in the US, with a special focus on Colorado, in hopes of providing a baby name to my wife that she would like. The analysis involves preprocessing the data, engineering relevant features, and using machine learning models to predict which names would appeal to my wife.

## Data Preprocessing

The data preprocessing involves:
- Extracting and reading data from zip files.
- Aggregating data for total count and most popular year in Colorado.
- Merging and aggregating data from multiple files to get a comprehensive dataset.

## Feature Engineering

The feature engineering process involves creating several new features for the names, such as:
- Length of the name
- Number of vowels and consonants
- Syllable count
- Entropy of the name
- Whether the name starts or ends with a vowel
- Language root detection using `langdetect`

## Model Training

The project includes training several machine learning models to predict the popularity of baby names:
- Random Forest Classifier
- XGBoost Classifier
- Support Vector Machine
- K-Nearest Neighbors
- TensorFlow Deep Learning model

Each model is trained and evaluated using appropriate metrics, and the best model is selected based on its performance.

## Usage


1. Clone the repository:
    ```bash
    git clone https://github.com/danielshort3/baby_names.git
    cd baby_names
    ```

2. Install the required packages (make sure you have `pip` and `virtualenv` installed):
    ```bash
    pip install seaborn langdetect tensorflow xgboost
    ```

3. Run the Jupyter notebook `Baby_Names_Analysis.ipynb` to preprocess the data, engineer features, and train the models.

4. The final predictions and analysis can be viewed in the notebook. The top 50 predicted names for boys are highlighted based on the average predicted ratings from different models.

## Note

Ensure that the necessary data files (`namesbystate.zip` and `names.zip`) are placed in the `data/` directory for the notebook to run successfully.

