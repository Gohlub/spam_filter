# Naive Bayes Spam Filter

A simple yet effective spam filter using the Naive Bayes algorithm, implemented in R.

## Overview

This project aims to classify messages as either "spam" or "ham" (not spam) based on their content. The Naive Bayes algorithm, a probabilistic classifier, is used to predict the category of a given message. The model is trained on a dataset containing labeled messages and then evaluated for accuracy.

## Features

- Data Exploration: Initial exploration of the dataset to understand the distribution of spam and ham messages.
- Data Cleaning: Standardization of messages by removing punctuation, converting to lowercase, and omitting numbers.
- Model Training: The model is trained using a subset (80%) of the dataset.
- Model Testing: The model's accuracy is tested using the remaining 20% of the dataset.
- Parameter Tuning: The model's performance is optimized by tuning the Laplace smoothing parameter, alpha.
- Message Classification: Functionality to classify custom messages as spam or ham.
Getting Started

## Prerequisites
Ensure you have the following R packages installed:

- tidyverse
- readr
- stringr
- ggplot2
- dplyr
- purrr
- Usage

## Usage
- Clone this repository.
- Load your data or use the provided spam.csv dataset.
- Run the R script to train and test the model.
- Use the classify_message function to classify custom messages and test.

## Results
### Data Overview:
The dataset contained 5,572 entries, with 87% labeled as 'ham' (not spam) and 13% as 'spam'.

### Model Training:

The Naive Bayes model was trained on 80% of the data (4,458 entries), maintaining a similar distribution to the original dataset.

### Posterior Distributions:

Using the Naive Bayes approach, we calculated word likelihoods for the 'spam' and 'ham' categories. Laplace smoothing was applied with an optimized alpha parameter.

### Model Performance:

The model achieved a 97% accuracy on the test set (1,114 entries). Sensitivity analysis revealed an optimal alpha value of 0.25 for Laplace smoothing.

### Limitations:

- The model assumes word independence given the class.
- Word sequence isn't considered.
- Numbers were removed, potentially excluding important features.


