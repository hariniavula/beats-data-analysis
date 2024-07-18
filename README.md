# beats-data-analysis

## Project Overview
This project was part of an internship with Extern and Beats by Dr.Dre. I analyzed customer reviews for various headphone products, including Beats Studio 3, Apple Airpods Max, Bose QuietComfort, Sennheiser, Sony M5, BERIBES, JBL, Soundcore Anker, Beats Studio Pro, and Beats Solo 4. The goal was to gain insights into consumer satisfaction and preferences for Beats by Dr. Dre products by leveraging data gathering, cleaning, analysis, and natural language processing.


## Final Insights  
- file: `Harini_Avula:_Beats_by_Dre_Consumer_Insights_-_Capstone_Project.ipynb`
- Comprehensive analysis and final insights derived from the project. 

## Data Collection 
- file: `gathering_data.ipynb`
- The reviews were gathered using the *Oxylabs API*, which provided access to Amazon reviews for the specified headphone products. The API allowed us to efficiently collect a large volume of reviews for each product, ensuring a comprehensive dataset for analysis.
- included one of the json files obtained from the API: `data (4).json`
- raw data file: `Reviews-update.csv`

## Data Cleaning and Preprocessing 
- file: `data_cleaning.ipynb`
- The collected data underwent a thorough cleaning process, which included:
- Handling missing values by filling them with appropriate placeholders or removing incomplete entries.
- Standardizing the format of key columns, such as `timestamp` and `rating`.
- cleaned data file: `cleaned_data.csv`

## Dataset
The dataset includes the following key columns:
- `title`: The title and preview of the review.
- `author`: The author of the review.
- `rating`: The rating given by the reviewer.
- `content`: The content of the review.
- `timestamp`: The date and time the review was posted.
- `profile_id`: The ID of the reviewer's profile.
- `is_verified`: Whether the review is from a verified purchase.
- `helpful_count`: The number of helpful votes the review received.
- `product_attributes`: Additional attributes of the product.

## Data Analysis and Visualization
- file: `EDA_and_analysis.ipynb`
- Descriptive statistics, data visualization, correlation analysis was performed on various variables and subsets. 
- Sentiment analysis was performed on the review texts using the VADER sentiment analyzer from the NLTK library. This helped classify reviews into positive, negative, and neutral sentiments, providing deeper insights into consumer opinions.
- Conclusion of findings/insights at the bottom. 

## Analysis Using Gemini AI
- file: `GeminiAI_Insights.ipynb`
- We utilized the *Gemini AI* model to analyze and summarize the key points from the reviews. The model helped in generating comprehensive insights for each subset of reviews.

## Installation
To run this project, ensure you have the following dependencies installed:
- pandas
- numpy
- seaborn
- matplotlib
- nltk
- google-generativeai
