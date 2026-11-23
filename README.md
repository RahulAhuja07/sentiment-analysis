# Sentiment Analysis Using Classical Machine Learning Techniques

**Live App**: [Streamlit Demo](https://omchandrasharma-sentiment-analysis-sentiment-appapp-p762tr.streamlit.app/)  
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
   [https://omchandrasharma-sentiment-analysis-sentiment-appapp-p762tr.streamlit.app/](https://omchandrasharma-sentiment-analysis-sentiment-appapp-p762tr.streamlit.app/)

2. In the left sidebar, select any model (e.g., Logistic Regression, KNN, Naive Bayes)

3. Scroll to the "Live Simulation" section

4. Enter a sentence or review in the input box

5. Click the "Predict" button

6. View the output label (Positive/Negative) and the prediction confidence score

---

## Folder Structure

.
├── ANN/ # Artificial Neural Network model, graphs & analysis
├── backend/ # FastAPI backend for model inference
├── clustering/ # Clustering algorithms and visualizations
├── decision_tree/ # Decision Tree implementation and analysis
├── KNN/ # K-Nearest Neighbors model and plots
├── linear_regression/ # Linear Regression model, graphs & performance
├── logistic_regression/ # Logistic Regression implementation & visuals
├── naive_bayes/ # Naive Bayes model for classification & sentiment
├── sentiment_app/ # Sentiment analysis logic and app code
├── svm/ # Support Vector Machine implementation and evaluation
├── .DS_Store
├── .gitattributes
├── README.md
├── Sentiment Analysis Dataset Report.pdf
├── SentimentClassificationReport.pdf

## Installation

Use Python 3.11 and run these commands from the project root:

```bash
python -m pip install -r sentiment_app/requirements.txt
python -m streamlit run sentiment_app/app.py
```

## Deploy Your Copy on Streamlit Community Cloud

1. Upload the latest project files to `RahulAhuja07/sentiment-analysis` on GitHub, including `sentiment_app/photos_members/Rahul.jpeg` and `sentiment_app/requirements.txt`.
2. Sign in at [Streamlit Community Cloud](https://share.streamlit.io/) using your GitHub account, then select **Create app** and **Yup, I have an app**.
3. Set the repository to `RahulAhuja07/sentiment-analysis`, select the branch containing your uploaded files, and set the main file path to `sentiment_app/app.py`.
4. In **Advanced settings**, select **Python 3.11** to match this project's existing dependency pins.
5. Choose an available app subdomain, such as `rahul-ahuja-sentiment-analysis`, and deploy. The suggested name is subject to availability.
6. Open the new app and check its pages, your portrait, graphs, and **Live Simulation** predictions. Once verified, replace both old Live App URLs in this README with the actual deployed URL.

The current prediction page calls the Cloud Run API configured in `sentiment_app/subpages/simulation.py`. Graphs also load from the existing `sentimentann` Google Cloud Storage bucket. Publishing a new Streamlit app does not transfer these services; confirm that they remain available, or migrate them and update the corresponding URLs. Trained models are not included in this project folder.

See the [official Streamlit deployment guide](https://docs.streamlit.io/deploy/streamlit-community-cloud/deploy-your-app/deploy) for the deployment form and settings.
