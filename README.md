# Fake News Detector

## Overview
This project implements a machine learning model to detect fake news articles. The model uses a combination of **Word2Vec embeddings**, **Gradient Boosting**, and an **LSTM-based neural network** to classify news articles as either **reliable (0)** or **unreliable (1)**.

## Dataset
https://www.kaggle.com/competitions/fake-news/data

## Features
- **Data Preprocessing**: 
  - Cleans text by removing non-alphabetic characters.
  - Converts text to lowercase.
  - Removes stopwords and applies stemming using `PorterStemmer`.
- **Word2Vec Embeddings**: 
  - Converts text into dense word vectors using a trained Word2Vec model.
- **Gradient Boosting Model**:
  - Uses extracted Word2Vec features for classification.
- **LSTM Neural Network**:
  - Uses an LSTM-based deep learning model for sequence classification.
  - Includes dropout layers to prevent overfitting.

## Installation
Ensure you have Python installed, then install dependencies using:

```sh
pip install -r requirements.txt
```

## Dataset
The dataset consists of two files:
- `train.csv` – Includes `id`, `title`, `author`, `text`, and `label`.
- `test.csv` – Includes `id`, `title`, `author`, and `text` (without labels).

## Usage
Run the following script to train the models:

```sh
python fake_news_detector.py
```
