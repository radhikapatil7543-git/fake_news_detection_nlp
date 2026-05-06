# Fake News Detection using NLP (R Project)

##  Project Overview
This project builds a machine learning model to classify news articles as **Fake** or **Real** using Natural Language Processing (NLP) techniques. The model processes raw text data and applies machine learning algorithms to detect misinformation.

##  Objective
To develop an automated system that can accurately identify fake news articles using text mining and classification techniques.

##  Dataset
- Source: Kaggle Fake and Real News Dataset  
- Files Used:
  - Fake.csv
  - True.csv  

##  Techniques Used

###  NLP Preprocessing
- Lowercasing text
- Removing punctuation
- Removing numbers
- Removing stopwords
- Removing extra whitespace

###  Feature Extraction
- Document-Term Matrix (DTM)
- TF-IDF weighting
- Sparse term reduction

###  Machine Learning Model
- Support Vector Machine (SVM)
- Linear Kernel

##  Workflow

1. Load dataset (Fake & True news)
2. Merge and label data
3. Clean and preprocess text
4. Convert text to numerical features (TF-IDF)
5. Split data into training and testing sets
6. Train SVM model
7. Predict and evaluate results

## Model Performance
- Evaluated using Confusion Matrix
- Accuracy calculated on test data

## Results
The model successfully classifies news articles into:
-  Real News
-  Fake News

##  Tools & Libraries
- R Programming
- tm (text mining)
- caret (model training & evaluation)
- e1071 (SVM model)
- SnowballC (text processing)

##  How to Run the Project
# Step 1: Set working directory
setwd("C:/Your/Project/Path")

# Step 2: Load libraries
library(tm)
library(caret)
library(e1071)

# Step 3: Run script
source("fake_news_model.R")
