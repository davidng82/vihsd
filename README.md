# Hate Speech Detection in Vietnamese Social Media

This project is aimed at developing a system to detect and classify offensive language in Vietnamese text using a combination of PhoBERT and Convolutional Neural Networks (CNN).

## Project Overview

Social media has become an essential part of our daily communication, but it has also fostered the rise of toxic environments, particularly through the spread of hate speech. This project focuses on addressing this issue by building a model that can effectively classify Vietnamese social media comments as either *clean* or *offensive*.

### Key Features:
- **Data Source**: The model uses the **ViHSD** dataset, which consists of 31,706 user comments from Vietnamese Facebook pages and YouTube videos.
- **Model**: A combination of **PhoBERT** (for text embeddings) and **CNN** (for feature extraction and classification).
- **Preprocessing**: Includes steps like removing URLs, emojis, emails, mention tags, and special characters from the dataset.
- **Performance**: Achieved an accuracy of **83.54%** on the test set.

## Table of Contents

1. [Background](#background)
2. [Related Work](#related-work)
3. [Study Goal](#study-goal)
4. [System Architecture](#system-architecture)
5. [Dataset](#dataset)
6. [Results](#results)
7. [Conclusions](#conclusions)
8. [License](#license)

## Background

Hate speech on social media is a growing concern. It not only degrades the quality of online interactions but also poses a threat to netizens' mental well-being. Detecting such content is crucial to maintaining a healthy online environment.

## Related Work

This project builds on existing research in the field of hate speech detection, including systems developed for Amharic and Danish languages, utilizing machine learning models and different natural language processing techniques.

- **System 1**: Hate Speech Detection in Amharic
    - Dataset: User-generated comments from Facebook.
    - Model: Word2Vec and TF-IDF for feature selection, and Random Forest and Naïve Bayes for classification.
- **System 2**: Hate Speech Detection in Danish
    - Dataset: User-generated comments from Reddit and Facebook.
    - Model: Automatic classification systems for offensive language in both English and Danish.

## Study Goal

The goal of this project is to develop a system for detecting and classifying offensive language in Vietnamese text. To achieve this:
- The **PhoBERT** model will be used for tokenization and text embeddings.
- A **CNN** will be integrated for feature extraction.
- The combined model will be fine-tuned to optimize performance.

## System Architecture

1. **Data Preprocessing**:
    - Input text is preprocessed by converting to lowercase and removing unnecessary elements (e.g., URLs, emojis).
    - The dataset is split into training, validation, and test sets with a 7:1:2 ratio.

2. **Model**:
    - **PhoBERT**: Utilized for tokenization and generating text embeddings.
    - **CNN**: Used to extract features from the embeddings and perform classification.

3. **Evaluation**:
    - Metrics such as **Precision**, **Recall**, **F1-Score**, and **Accuracy** were used to evaluate the model's performance.

## Dataset

The **ViHSD** dataset used in this project was taken from the following repository: [ViHSD Dataset](https://github.com/sonlam1102/vihsd).

- **Description**: The dataset consists of user comments related to entertainment, celebrities, and social issues from various Vietnamese Facebook pages and YouTube videos. 
- **Size**: 31,706 comments labeled as either *CLEAN* or *OFFENSIVE*.
- **Data Splitting**: The dataset was divided into train, validation, and test sets using a 7:1:2 ratio.

## Results

The model demonstrates robust performance with the following metrics:
- **Accuracy**: 83.54%
- **F1-Score (Clean)**: 0.8341
- **F1-Score (Offensive)**: 0.8368

## Conclusions

The project successfully developed a system capable of detecting offensive language in Vietnamese social media. Future improvements could focus on incorporating more Vietnamese slang and dialects to enhance the model's understanding of different regional variations in language use.

## License

This project is licensed under the MIT License.

The ViHSD dataset is available under the terms outlined in its repository at [ViHSD Dataset Repository](https://github.com/sonlam1102/vihsd).
