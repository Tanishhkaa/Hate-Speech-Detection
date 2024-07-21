# Hate Tweet Classifier

The Hate Tweet Classifier is a web-based application designed to identify and classify tweets based on their content. It utilizes a machine learning model to detect hate speech, offensive language, or classify a tweet as non-offensive. This project aims to create a tool for filtering harmful language on social media platforms.

## Theory

### Overview

Social media platforms often encounter issues with harmful content, such as hate speech and offensive language. To address this, we developed a machine learning model that classifies tweets into three categories:
1. **Hate Speech Detected**: Tweets containing hate speech.
2. **Offensive Language Detected**: Tweets containing offensive but non-hate speech.
3. **No Hate and Offensive Speech**: Tweets that do not contain any harmful content.

### Approach

1. **Data Collection**: The model is trained on a dataset of tweets, which includes labeled examples of hate speech, offensive language, and non-offensive content.

2. **Preprocessing**: Tweets are cleaned and preprocessed to enhance the model's performance. This involves:
   - Converting text to lowercase.
   - Removing URLs, HTML tags, and punctuation.
   - Removing words containing digits and stopwords.
   - Applying stemming to reduce words to their root forms.

3. **Feature Extraction**: The cleaned text data is transformed into numerical features using the `CountVectorizer`, which converts text into a matrix of token counts.

4. **Model Training**: A Decision Tree Classifier is trained on the preprocessed data. Decision Trees are chosen for their interpretability and ability to handle both numerical and categorical data.

5. **Prediction**: The trained model is used to classify new tweets into one of the predefined categories based on their content.

### Implementation

The application is built using Flask, a lightweight web framework for Python. It provides a user interface where users can input tweets and receive predictions from the model.

## Features

- **User Interface**: A simple and clean web interface for inputting tweets and displaying predictions.
- **Text Preprocessing**: Automatically cleans and preprocesses the tweet text for accurate classification.
- **Machine Learning Model**: Utilizes a Decision Tree Classifier to categorize tweets.

## Requirements

- Python 3.x
- Flask
- Pandas
- NumPy
- Scikit-learn
- NLTK

  ![image](https://github.com/user-attachments/assets/80773076-1cd9-4cd2-986d-015c51253a9c)
