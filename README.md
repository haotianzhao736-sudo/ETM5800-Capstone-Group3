# ETM5800-Capstone-Group3
ETM5800 Capstone Project: Multi-Method Text Analytics on Amazon Reviews (Group 3)
# Understanding Customer Dissatisfaction in E-Commerce (ETM5800 Group 3)

## Project Overview
This capstone project applies a multi-method text analytics workflow to 18,000 Amazon product reviews. The objective is to identify drivers of negative customer experiences using Exploratory Data Analysis, LDA Topic Modelling, DistilBERT Sentiment Classification, and Aspect-Based Sentiment Analysis (ABSA).

## Team Members
* Lyu Li (35770856)
* Zhao Haotian (35990635)
* Lu Dingming (35644559)
* Liu Zizheng (36573582)

## Repository Structure
* `/Dataset`: Contains all project datasets.
  * `raw_amazon_reviews.csv`: The original, uncleaned Amazon review dataset (18,000 entries across 3 categories).
  * `cleaned_amazon_reviews.csv`: The preprocessed dataset used for all modeling and analytics.
* `ETM5800_A3_Capstone.ipynb`: The annotated Jupyter Notebook containing all code for EDA, Unsupervised, Supervised, and Advanced text analytics.
* `requirements.txt`: List of dependencies required to run the notebook.

## How to Run the Code
1. Clone this repository.
2. Install the required dependencies: `pip install -r requirements.txt`
3. Open and run `ETM5800_A3_Capstone.ipynb` in sequential order. (Note: DistilBERT models require GPU acceleration, such as Google Colab T4).

## Key Findings
* Negative reviews tend to be longer (median 45 tokens) than positive ones (40 tokens).
* DistilBERT achieved the highest classification performance (F1 = 0.899).
* LDA identified 7 distinct complaint themes, validated by K-Means (ARI = 0.419).
