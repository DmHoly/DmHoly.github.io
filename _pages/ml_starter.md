---
layout: tutorial      # ← use the tutorial layout, not default
title: "ML Starter — Titanic, Penguins & Iris"
date: 2025-07-21 10:00:00 +0000
permalink: /projects/ml-starter/
repo_url: https://github.com/DmHoly/ML_Starter
iris_notebook : https://github.com/DmHoly/ML_Starter/blob/master/notebooks/iris.ipynb
penguins_notebook : https://github.com/DmHoly/ML_Starter/blob/master/notebooks/penguins.ipynb
titanic_notebook : https://github.com/DmHoly/ML_Starter/blob/master/notebooks/titanic.ipynb
generic_pipeline : https://github.com/DmHoly/ML_Starter/blob/master/notebooks/full_sk_pipe.ipynb 
---

![Illustration](/assets/images/banner_ml_starter.png)

Welcome to the ML Starter series, a progressive set of tutorials for beginners.
We'll start with the basics of machine learning and gradually introduce more complex concepts using popular datasets.

All the datasets are available on [Kaggle](https://www.kaggle.com/datasets) but more easily accessible on seaborn and scikit-learn.

- Disclaimer: This is not a comprehensive course, but rather a series of notebooks to get you started with practical machine learning tasks.
- Disclaimer#2 : For most of this dataset a naive method can be used to achieve a good accuracy, remember the best model is the one that solves the problem (and the simpler the better), not the most complex one.

## Getting Started
To get started, make sure you have the following libraries installed:

```bash
pip install pandas numpy scikit-learn seaborn matplotlib
```

You can use Jupyter Notebook, or any Python IDE of your choice. The code is structured to be run in a Jupyter Notebook environment, but you can adapt it to any Python script.

Note : On the code i propose some utility functions to help you with the data exploration and visualization, feel free to use them or not, they are not mandatory.
you can also check on generic pipelines on this notebook [here]({{ page.generic_pipeline }}).
This notebook provides a generic pipeline for data preprocessing, model training, and evaluation using scikit-learn. It can be adapted to any dataset.
On src/utils.py you can find some utility functions and how to add classes compatible with sklearn pipelines (you need notion of heritage in python to understand this part).

## Iris Classification (Beginner)

The Iris dataset is a classic introduction to classification. In this section, we'll:

- Load the Iris dataset
- Explore feature distributions
- Train a simple classifier
- Evaluate model performance (accuracy, confusion matrix etc...)

The notebook for this task is available [here]({{ page.iris_notebook }}).

## Penguins Classification (Intermediate)

The Palmer Penguins dataset adds complexity:
In this dataset there are missing values and categorical features. 

We'll cover:

1. Handle missing values
2. Perform feature encoding 
3. Compare multiple models
4. Evaluate model performance
5. Introduction to cross-validation (to compare models)

The notebook for this task is available [here]({{ page.penguins_notebook }}).

## Titanic Classification (Advanced)

Predict survival on the Titanic with:
This dataset is more complex with a mix of numerical and categorical features, missing values, and requires more advanced techniques.

- Advanced feature engineering (titles, family size)
- Cross-validation
- Ensemble methods

The notebook for this task is available [here]({{ page.titanic_notebook }}).

## Regression Task (Coming Soon)

Stay tuned for regression tasks using datasets like Boston Housing or California Housing. We'll cover:
- Data preprocessing
- Model training
- Evaluation metrics
and a bit more complexity.

All notebooks and data are available on [GitHub]({{ page.repo_url }}). Happy learning!