# Spam/Not Spam Mail Classifier

## Project Overview

The **Spam/Not Spam Mail Classifier** is a machine learning project that automatically classifies emails as either spam or not spam. Using a variety of text preprocessing techniques and machine learning models, this project aims to create a robust system for filtering unwanted emails based on their content.

Three different vectorization methods—**CountVectorizer**, **TF-IDF**, and **Word2Vec**—are used to transform the text data into numerical features, and a **Naive Bayes classifier** is trained for each. The project compares the performance of these methods to determine the most effective approach for email classification.

## Features

- Text preprocessing: tokenization, stemming, and spell correction
- Three vectorization methods: **CountVectorizer**, **TF-IDF**, and **Word2Vec**
- Naive Bayes classifier for email classification
- Performance evaluation using accuracy metrics and confusion matrices
- Comparison of models based on different feature extraction techniques

## Dataset

The dataset used in this project consists of emails labeled as **spam** or **not spam**, with text data in one column and the label in another. The dataset is preprocessed to remove noise and irrelevant characters, and is split into training and testing sets.

## Methods

1. **Text Preprocessing**:
   - Lowercasing, removing special characters, tokenization
   - Stemming using the PorterStemmer
   - Spell correction using the `autocorrect` library
   - Removal of stop words

2. **Vectorization Methods**:
   - **CountVectorizer**: Converts text into a bag-of-words model
   - **TF-IDF**: Computes term frequency-inverse document frequency to represent text
   - **Word2Vec**: Creates word embeddings to capture the semantic meaning of words

3. **Classification**:
   - **Naive Bayes classifier** is used to classify the emails for each vectorization technique.

## Results

- **CountVectorizer**: Accuracy of 84.48%
- **TF-IDF**: Accuracy of 84.30%
- **Word2Vec**: Accuracy of 95.87%

The **Word2Vec** method outperforms the other two vectorization techniques, achieving the highest accuracy and the lowest misclassification rates.

## Conclusion
This project provides a practical solution to email classification, with Word2Vec emerging as the most effective vectorization method. The classifier can be further improved with more sophisticated models or a larger dataset, but it serves as a solid foundation for spam detection.
