# Sentiment Analysis with Two Datasets

This repository contains a sentiment analysis project using two distinct datasets with over 2 million samples. The analysis covers data exploration, preprocessing, and model training for sentiment classification. The project is split into multiple Jupyter notebooks, with each handling specific tasks like data cleaning, preprocessing, and model training.

## Project Overview

The goal of this project is to build a sentiment analysis model capable of classifying text data (such as tweets) into different sentiment categories (e.g., positive, negative, or neutral). The workflow includes:
- Data exploration
- Preprocessing
- Training a machine learning model using GRU (Gated Recurrent Unit) on two large-scale datasets

## Datasets Used

1. **[Sentiment Dataset with 1 Million Tweets](https://www.kaggle.com/datasets/tariqsays/sentiment-dataset-with-1-million-tweets)**  
   This dataset contains over 1 million labeled tweets, where each tweet is associated with a sentiment label (positive, negative, or neutral). For more information on a similar project using this dataset, see this [GitHub repository](https://github.com/basel5621/Sentiment-Analysis-with-Sentiment140-dataset.git).

2. **[Sentiment140 Dataset](https://www.kaggle.com/datasets/kazanova/sentiment140)**  
   This dataset contains 1.6 million tweets, each labeled with sentiment (positive, negative, or neutral). A related project implementation for this dataset can be found in this [GitHub repository](https://github.com/basel5621/Sentiment-Analysis-with-Sentiment-Dataset-with-1-Million.git).


## Files in the Repository

1. **Cleaning_dataset1.ipynb**  
   This notebook handles the cleaning of the first dataset, "Sentiment Dataset with 1 Million Tweets." It involves:
   - Loading and exploring the dataset.
   - Performing data cleaning (e.g., removing noise, handling missing values).
   - Text preprocessing, such as tokenization, stemming, lemmatization, and removing stopwords.

2. **Cleaning_dataset2.ipynb**  
   This notebook is dedicated to the second dataset, "Sentiment140." It follows similar preprocessing steps to ensure consistency between the two datasets.

3. **trained_GRU_model.ipynb**  
   This notebook is used for training the sentiment analysis model using a GRU (Gated Recurrent Unit) neural network. It covers:
   - Splitting the data into training and validation sets.
   - Model training and evaluation using metrics like accuracy, precision, recall, and F1 score.
   - Saving the trained model for future use.

## Requirements

To run this project, you need the following Python libraries:
- `pandas` for data manipulation.
- `numpy` for numerical operations.
- `matplotlib` and `seaborn` for data visualization.
- `scikit-learn` for model training and evaluation.
- `nltk` or `spaCy` for natural language processing tasks.

You can install the required libraries by running:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn nltk
```

## Running the Project

1. **Data Cleaning**:  
   Run the `Cleaning_dataset1.ipynb` and `Cleaning_dataset2.ipynb` notebooks to clean and preprocess the datasets. These steps are essential for preparing the data for the sentiment analysis model.

2. **Model Training**:  
   Use the `trained_GRU_model.ipynb` notebook to train a sentiment analysis model using the preprocessed data. The notebook guides you through splitting the data, training the model, and evaluating its performance.
