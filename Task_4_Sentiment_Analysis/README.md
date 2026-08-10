# Task 4: Sentiment Analysis

## 📌 Project Overview
This project performs **Natural Language Processing (NLP)** and **Sentiment Analysis** on Twitter text data (`Twitter_Data.csv`) as part of the **CodeAlpha Data Analytics Internship**. The goal is to preprocess raw social media text, extract feature vectors, and classify public feedback into distinct sentiment categories: **Positive (1)**, **Neutral (0)**, and **Negative (-1)**.

---

## Repository Structure
```text
Task_4_Sentiment_Analysis/
├── README.md                   # Task documentation & findings
├── Sentiment_Analysis.ipynb    # Jupyter Notebook with text preprocessing & Naive Bayes model
└── Twitter_Data.csv            # Social media sentiment dataset

Workflow & Methodology
​Data Preprocessing: Clean raw text by lowercasing, stripping URLs, removing user mentions (@username), removing hashtags, and dropping special characters/numbers using regular expressions (re).
​Sentiment Distribution: Map numeric labels (1, 0, -1) to human-readable categories (Positive, Neutral, Negative) and evaluate class balance.
​Feature Extraction: Transform cleaned text into numerical representations using TF-IDF Vectorization (max_features=5000).
​Model Training & Evaluation: Train a Multinomial Naive Bayes classifier, evaluated using Accuracy, Precision, Recall, F1-Score, and a Confusion Matrix heatmap.
​
Tools & Libraries
​Language: Python 3.x
​Libraries: pandas, numpy, scikit-learn, matplotlib, seaborn, re
​
Key Results & Insights
​Data Quality: Standardized raw text entries and removed missing values cleanly across the dataset.
​Model Performance: TF-IDF feature extraction combined with Naive Bayes provided a solid classification baseline across all sentiment categories.
​Visual Outputs: Generated a Sentiment Count Plot and Confusion Matrix for clear evaluation of classification performance.
