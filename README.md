# sms_spam_detector
# SMS Spam Classification with Gradio Interface

## Overview

This project implements a machine learning model to classify SMS messages as either "spam" or "not spam" using a Naive Bayes classifier. The model is built using Python, with the `scikit-learn` library, and deployed through an interactive user interface using Gradio. Users can input up to four SMS messages at a time to receive a prediction on whether each message is spam or not.

## Features

- **Text Classification**: Classifies SMS messages into "spam" or "not spam".
- **Interactive Interface**: A user-friendly Gradio interface for easy interaction.
- **Batch Prediction**: Allows input of up to four SMS messages simultaneously.

## Project Structure

- **gradio_sms_text_classification.ipynb**: The Jupyter notebook containing the entire workflow for loading data, preprocessing, model training, and deployment with Gradio.
- **SMSSpamCollection.csv**: The dataset containing SMS messages labeled as "spam" or "ham" (not spam).
- **README.md**: Documentation file providing an overview of the project.

## Getting Started

### Prerequisites

Ensure you have the following installed:

- Python 3.7 or higher
- Jupyter Notebook
- `scikit-learn`
- `pandas`
- `gradio`

You can install the required Python packages using:

pip install scikit-learn pandas gradio

### Installation

**Clone the Repository:**

   ```bash
   git clone https://github.com/yourusername/sms-spam-classification.git
   cd sms-spam-classification'''
   
### Dataset

```markdown

## Dataset

The dataset used for training the model is `SMSSpamCollection.csv`, which contains a collection of SMS messages labeled as "spam" or "ham". The dataset is divided into two columns:

- `label`: The label for each message, either "spam" or "ham".
- `message`: The content of the SMS message.

## Model

The model used is a **Naive Bayes classifier** with a **TF-IDF vectorizer**. The model is trained to identify patterns in text that are indicative of spam.

## How It Works

1. **Data Preprocessing:**
   - Convert the text data into a TF-IDF matrix using `TfidfVectorizer`.
   
2. **Model Training:**
   - Train a Naive Bayes classifier on the processed data.
   
3. **Prediction:**
   - Input SMS messages that are vectorized using the same TF-IDF process.
   - The model predicts the likelihood of each message being spam.

4. **Deployment:**
   - A Gradio interface is provided for users to interact with the model in real-time.
