# beats-data-analysis

## Project Overview
This project aims to analyze customer reviews for various headphone products, including Beats Studio 3, Apple Airpods Max, Bose QuietComfort, Sennheiser, Sony M5, BERIBES, JBL, Soundcore Anker, Beats Studio Pro, and Beats Solo 4. The goal is to gain insights into consumer satisfaction and preferences for Beats by Dr. Dre products by leveraging data gathering, cleaning, analysis, and natural language processing.

## Data Collection
- The reviews were gathered using the Oxylabs API, which provided access to Amazon reviews for the specified headphone products. The API allowed us to efficiently collect a large volume of reviews for each product, ensuring a comprehensive dataset for analysis.
- included one of the json files obtained from the API -> data (4).json 

## Data Cleaning and Preprocessing 
The collected data underwent a thorough cleaning process, which included:
- Handling missing values by filling them with appropriate placeholders or removing incomplete entries.
- Standardizing the format of key columns, such as `timestamp` and `rating`.
- Ensuring consistency in the `product_attributes` column to facilitate accurate analysis.

## Dataset
The cleaned dataset includes the following key columns:
- `title`: The title of the review.
- `author`: The author of the review.
- `rating`: The rating given by the reviewer.
- `content`: The content of the review.
- `timestamp`: The date and time the review was posted.
- `profile_id`: The ID of the reviewer's profile.
- `is_verified`: Whether the review is from a verified purchase.
- `helpful_count`: The number of helpful votes the review received.
- `product_attributes`: Additional attributes of the product.

## Sentiment Analysis
Sentiment analysis was performed on the review texts using the VADER sentiment analyzer from the NLTK library. This helped classify reviews into positive, negative, and neutral sentiments, providing deeper insights into consumer opinions.

## Analysis Using Gemini AI
We utilized the Gemini AI model to analyze and summarize the key points from the reviews. The Gemini AI model helped in generating comprehensive insights for each subset of reviews.

## Installation
To run this project, ensure you have the following dependencies installed:
- pandas
- numpy
- seaborn
- matplotlib
- nltk
- google-generativeai
