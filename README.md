# Sentiment Analysis of Book Reviews using Recurrent Neural Networks

## Overview

This project implements a deep learning model to classify book reviews as either positive or negative using a Recurrent Neural Network (RNN). The dataset used for this classification task originates from a Twitter sentiment analysis dataset sourced from Kaggle. Since social media plays a crucial role in gauging public reception of products and services, this model could be used to analyze sentiment and help companies understand consumer preferences.

## Motivation

The goal of this project is to explore deep learning techniques for Natural Language Processing (NLP), particularly using RNNs for sentiment analysis. The model's ability to parse key words and detect sentiment is useful for companies aiming to analyze customer feedback and improve recommendations.

## Dataset

The dataset consists of tweets related to various products and services, with each tweet labeled as either positive or negative. This is a binary classification problem with no class imbalance.

## Features

- **Text data**: The primary feature in this dataset is the text of the reviews themselves.

## Data Preprocessing

To prepare the data for training, the following preprocessing steps are applied:

- Convert all text to lowercase
- Remove stop words
- Apply stemming
- Tokenization
- Convert text into word embeddings using an embedding layer

## Model Architecture

The model is based on a deep learning approach, utilizing:

- Word embeddings mapped to tokens
- Two Long Short-Term Memory (LSTM) layers for sequence processing
- A final output layer for classification

## Model Training and Evaluation

- The model is trained using a combination of feed-forward and recurrent architectures.
- Performance is evaluated using **AUC (Area Under the Curve)**, which measures classification effectiveness independently of any classification threshold.
- If RNNs pose computational challenges, a downsampled RNN will be tested against a full dataset feed-forward network.

## Potential Improvements

- Experimenting with different neural network architectures (e.g., GRUs, Transformers)
- Optimizing hyperparameters for better performance
- Utilizing pre-trained word embeddings such as Word2Vec or GloVe

## Requirements

- Python
- TensorFlow / PyTorch
- Kaggle API (for dataset retrieval)
- NLP libraries (e.g., NLTK, SpaCy)

## How to Run

1. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
2. Load and preprocess the dataset.
3. Train the model using the Jupyter Notebook provided.
4. Evaluate the model using the defined metrics.

## Future Work

- Implement sentiment analysis on other datasets
- Expand the model to multi-class classification (e.g., neutral sentiment)
- Deploy the model as an API for real-time analysis

## Acknowledgments

- Kaggle for providing the dataset
- Open-source NLP and deep learning communities


