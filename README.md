# Beats-by-Dre-Consumer-Insights

**Project Title:** Consumer Insights Data Analytics Externship of Beats by Dre  
**Student Name:** Ferdinand Virtudes  
**Program Date:** June 29 2024 to September 2, 2024

### Overview

This project analyzes Amazon reviews for Beats by Dre and competitor Bluetooth speakers to extract actionable consumer insights. Using Python, EDA, sentiment analysis (TextBlob, NLTK), and Gemini AI, it identifies trends, pain points, and opportunities for product improvement.

### Key Findings

* Sentiment-Rating Gap: Beats shows high sentiment scores (positive language) but lower actual ratings, suggesting unmet expectations.
* Price Sensitivity: Products priced 50−150 receive higher satisfaction (avg. rating: 4.8–5.0).
* Top Pain Points: Connectivity issues, battery life, and sound quality inconsistencies.
* Competitor Benchmark: Brands like JBL and Bose outperform Beats in ratings despite similar sentiment.

### Methods

1. Data Collection: Scraped ~1,000 Amazon reviews using Oxylabs API.
2. EDA: Analyzed rating distributions, price vs. satisfaction trends, and review length patterns.
3. Sentiment Analysis: Leveraged VADER and TextBlob to quantify sentiment polarity.
4. AI Insights: Gemini AI summarized recurring themes (e.g., design praise, durability complaints).

### Recommendations

* Product: Enhance Bluetooth stability, battery life, and mid-range sound clarity.
* Marketing: Leverage positive sentiment in campaigns; address pricing/value perception.
* Future Research: Expand data to include demographics and competitor feature breakdowns.

### Tools

* Python (Pandas, Matplotlib, Seaborn)
* NLTK, TextBlob, Gemini AI
* Oxylabs API (web scraping)

### Files

* merged_data.csv: Processed review dataset.
* Beats_Consumer_Insights.ipynb: Full analysis notebook.