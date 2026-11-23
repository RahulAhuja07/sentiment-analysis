# Sentiment Analysis Using Classical Machine Learning Techniques

**Live App**: [App](https://sentiment-analysis-rahul-ahuja.streamlit.app/)
**Dataset**: [Kaggle Dataset](https://www.kaggle.com/datasets/abhi8923shriv/sentiment-analysis-dataset/data)

---

## Project Overview

This project presents a unified sentiment analysis platform built using classical machine learning models. The primary goal is to classify textual data (e.g., reviews or comments) based on emotional tone — positive or negative.

### Features

- Text preprocessing (cleaning, normalization)
- TF-IDF and Bag-of-Words (BoW) vectorization
- Dimensionality reduction using Singular Value Decomposition (SVD)
- Multiple ML algorithms:
  - Logistic Regression
  - Linear Regression
  - K-Nearest Neighbors (KNN)
  - Naive Bayes
  - Decision Tree
  - Artificial Neural Network (ANN)
  - Support Vector Machine (SVM)
  - Clustering (Unsupervised)
- Interactive real-time inference and model comparison via a Streamlit dashboard
- Modular and scalable architecture

---

## How to Use the Web App

1. Open the app:  
   [Sentiment Analysis App](https://sentiment-analysis-rahul-ahuja.streamlit.app/)

2. In the left sidebar, select any model (e.g., Logistic Regression, KNN, Naive Bayes)

3. Scroll to the "Live Simulation" section

4. Enter a sentence or review in the input box

5. Click the "Predict" button

6. View the output label (Positive/Negative) and the prediction confidence score

---

## Folder Structure

```text
sentiment-analysis/
├── .devcontainer/           # Development environment configuration
├── ANN/                     # Neural network implementation and results
├── backend/                 # FastAPI prediction service
├── clustering/              # Clustering algorithms and results
├── decision_tree/           # Decision Tree and Random Forest analysis
├── KNN/                     # K-Nearest Neighbors implementation and results
├── linear_regression/       # Linear Regression implementation and results
├── logistic_regression/     # Logistic Regression implementation and results
├── naive_bayes/             # Naive Bayes implementation and results
├── sentiment_app/           # Streamlit dashboard
│   ├── app.py               # App entrypoint and navigation
│   ├── photos_members/      # Team portraits
│   ├── subpages/            # Home, model analysis, simulation, and About pages
│   ├── utils/               # Preprocessing and model helpers
│   └── requirements.txt     # Dashboard dependencies
├── svm/                     # Support Vector Machine implementation and results
├── .gitattributes
├── .gitignore
├── README.md
└── Sentiment Analysis Dataset Report.pdf
```

## Installation

Use Python 3.11 and run these commands from the project root:

```bash
python -m pip install -r sentiment_app/requirements.txt
python -m streamlit run sentiment_app/app.py
```
