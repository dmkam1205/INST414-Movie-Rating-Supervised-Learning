# Movie Rating Supervised Learning Analysis

This repository contains the code and data for my INST414 supervised learning assignment.

## Project Question

Can basic movie metadata help predict whether a movie will receive a high IMDb rating?

## Dataset

The dataset was constructed from raw IMDb movie records covering movies released between 2000 and 2022.

The supervised target is:

- `1` if IMDb rating is 7.0 or higher
- `0` if IMDb rating is below 7.0

## Features

The model uses:

- release year
- runtime
- IMDb vote count
- genre indicator variables

## Model

A Decision Tree Classifier was used with:

- `max_depth=6`
- `random_state=42`
- 80/20 train-test split

## Evaluation

The model was evaluated using:

- accuracy
- precision
- recall
- F1-score
- confusion matrix

The analysis also examines five movies the model classified incorrectly.

## Files

- `movie_rating_supervised_learning.ipynb` - full analysis
- `constructed_movie_supervision_dataset.csv` - constructed dataset
- `five_misclassified_movies.csv` - five incorrect predictions
- `feature_importance.csv` - model feature importance values
- `movie_rating_confusion_matrix.png` - confusion matrix
- `movie_rating_feature_importance.png` - feature importance visualization
