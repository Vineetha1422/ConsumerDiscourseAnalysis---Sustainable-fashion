# Analyzing Consumer Discourse on Reddit's Sustainable Fashion Community

## Overview
This project investigates how consumers discuss sustainable fashion choices on Reddit, focusing on material preferences, ethical considerations, and purchasing behaviors. With social media becoming a critical platform for shaping sustainable consumption patterns, this analysis reveals key conversation drivers and sentiment trends in eco-fashion communities.

## Tools
- **Python Libraries**: 
  ![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![PRAW](https://img.shields.io/badge/PRAW-FF4500?style=flat&logo=reddit&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![NLTK](https://img.shields.io/badge/NLTK-222222?style=flat)
![Scikit--learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)
![Empath](https://img.shields.io/badge/Empath-Analysis-blue?style=flat)
- **Methods**: Non-Negative Matrix Factorization (NMF), TF-IDF vectorization, lexicon-based sentiment analysis

## Approach
1. **Data Collection**:  
   - Collected 1,300 comments from r/SustainableFashion using Reddit API
   - Filtered to 1,146 quality comments after removing duplicates/short texts

2. **Topic Modeling**:
   - Identified 6 key discussion themes using NMF with coherence score 0.6437
   - Created document-term matrix with TF-IDF (max_df=0.95, min_df=2)

3. **Sentiment Analysis**:
   - Evaluated 5 emotional dimensions: Positive/Negative Emotion, Money, Shopping, Business
   - Normalized scores across 6 identified topics

4. **Classification**:
   - Tested 4 ML models on topic predictions
   - Split data 80/20 train-test ratio

## Results
- **Top-Performing Model**: Logistic Regression (81% accuracy, 0.80 F1-score)
- **Key Findings**:
  - 23% of discussions focused on Quality/Brand Perception
  - Sustainable Fabric Sourcing had lowest representation (9%)
  - Business-related terminology dominated Eco-Friendly Mate

## File Details
Code : 
- Dataset collection - Sustainable fashion.ipynb : code to collect data from Reddit using PRAW.
- SustainableFashion_Analysis : code for complete analysis mentioned in the paper.

Data : sustainable_fashion_data.csv.
