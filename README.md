# Beats-by-Dre-Consumer-Insights

## 1. Title Page
**Project Title:** Consumer Insights Data Analytics Externship of Beats by Dre  
**Student Name:** Ferdinand Virtudes  
**Date:** June 29 2024 to September 2, 2024

The purpose of this project is to collaborate with Beats by Dr. Dre to provide consumer insights that strengthen product development and refine strategy. Using tools like Python, EDA, sentiment analysis, and AI, the project focuses on data-driven decision-making to enhance business outcomes.

The information below are key highlights of the project.

Key Objectives:

*   Gather and Clean Data: Collect relevant data and ensure its quality for accurate analysis.
* Perform EDA and Sentiment Analysis: Analyze data to uncover trends and understand consumer feedback.
* Leverage AI Tools for Deeper Insights: Utilize AI to extract meaningful themes and insights from customer reviews.
* Develop Strategic Recommendations: Use insights to propose data-driven improvements for product and strategy.

## 2. Table of Contents
1. Introduction
2. Data Description
3. Exploratory Data Analysis (EDA)
4. Sentiment Analysis
5. AI-Generated Insights
6. Comparative Analysis
7. Strategic Recommendations
8. Conclusion
9. References


### 4.2 Data Collection
Explaining the data gathering process, including any challenges faced and how they were overcome.

The data gathering process involved extracting Amazon reviews for the new Beats Pill Bluetooth Speakers and similar products within the same category and price range. The goal was to collect approximately 100 reviews per product, totaling around 1,000 reviews. Here’s a breakdown of the steps and challenges faced:

Step-by-Step Process:
1. Accessing Oxylabs API:
* Signed up for a trial account on Oxylabs, which allows up to 5,000 requests during a 7-day trial period.
* Used the eCommerce Scraper API to handle Amazon’s dynamic content, simplifying the review extraction process.
2. Filling in the API Form:
* Entered the ASIN (Amazon Standard Identification Number) for each product.
* Selected a user agent (desktop) and allowed structured data parsing without JavaScript rendering.
* Chose the appropriate Amazon domain (e.g., .com for the US market) and specified the starting page number and the number of pages (up to 20).
3. Extracting Reviews:
* Extracted reviews for each product, using multiple page numbers to maximize data collection. Due to Amazon’s limitations, the extraction often capped at 100 reviews or 10 pages per product.
* To overcome this limitation, diversified the number of products and explored different page numbers to achieve the target of 1,000 reviews.
4. Exporting and Parsing Data:
* Exported the extracted data in JSON format and used provided Google Colab code to parse the JSON into a structured dataset.
* Converted the parsed data into a DataFrame and saved it as a CSV file.
5. Compiling and Merging Data:
* Repeated the extraction process for additional products.
* Loaded all CSV files into DataFrames and merged them to create a comprehensive dataset.
* Saved the final merged DataFrame as a CSV file for further analysis.

**Challenges Faced and Solutions:**
* **API Limitations:** Amazon reviews are often capped at 100 reviews or 10 pages per product. To address this, we increased the number of products and experimented with different page numbers to collect sufficient data.
* **Time Constraints:** The trial period for Oxylabs was limited to 7 days. To optimize data collection, we prepared in advance and completed all requests within the trial period.
* **Dynamic Content:** Scraping dynamic content from Amazon posed challenges, but using the Oxylabs API simplified the process, allowing us to focus on data analysis.

By following these steps, we successfully compiled a robust dataset of Amazon reviews for the targeted product category, ready for sentiment analysis and consumer insights.

## 5. Exploratory Data Analysis (EDA)

### 5.1 Data Overview
Provide a summary of the dataset, including key statistics (mean, median, mode, standard deviation, etc.).

Rating:
* Average is high at 4.55, with most ratings being 5.
Indicates generally positive feedback.

Helpful Count:
* Low median (0) but a high maximum (2116), suggesting a few reviews received significantly more attention than others.

Date Range:
* Reviews span from November 1, 2018, to August 9, 2024, with a concentration around 2023 and 2024.

Day and Month:
* Reviews are spread across all days and months, with slight peaks in mid-month and in July.

Price:
* Average price is $150.26, with most prices clustering between $98 and $200.
Indicates a moderate price range for the products being reviewed.

### 6.2 Results
Present the sentiment analysis results, including visualizations of sentiment distribution, and discuss the overall sentiment towards Beats by Dre products.

Results:
* The sentiment analysis reveals that the reviews for Beats by Dre generally contain positive language, but this does not translate into higher product ratings.

Visualizations:

* The bar chart indicates that Beats by Dre has one of the higher average sentiment scores among competitors, yet actual product ratings may not align with these sentiments.

Discussion of Overall Sentiment:

* The overall sentiment toward Beats by Dre products is positive in textual content but may be tempered by unmet expectations, price sensitivity, or other specific disappointments that lead to lower final ratings. This suggests a gap between perceived value and customer expectations that the brand might need to address to improve its ratings.

Observations:

Expectations vs. Reality:
* Customers may have high expectations for Beats by Dre due to its strong brand reputation. When the product doesn't fully meet these expectations, even slightly, customers may rate it lower despite mentioning some positive aspects in their reviews.

Brand Premium Effect:
* As a premium brand, Beats by Dre products are often priced higher. Customers might expect top-tier performance and quality for the price they pay. If they perceive any shortcomings, their overall rating could be negatively impacted, regardless of some positive features they discuss.

Selective Emphasis in Reviews:
* In reviews, customers may mention specific positive features (e.g., sound quality) while still rating the product lower due to other issues (e.g., durability, value for money). This can cause a mismatch between the sentiment expressed in the text and the overall rating given.

Key Insights Summarized

Overall, customers appreciate speakers that balance sound quality, durability, ease of use, and price. However, connectivity issues, app limitations, and some specific sound quality concerns are common drawbacks.

Common Findings Across All Reviews:

1. Common Complaints or Issues:
* Sound Quality Issues:
Lack of deep bass or muddy bass at high volumes.
Issues with midrange clarity and treble harshness.
Spatial or stereo sound features not performing as expected.
* Connectivity Problems:
Frequent Wi-Fi and Bluetooth connection drops or difficulties in pairing.
Problems with multi-device connectivity and audio synchronization.
* Battery and Charging Concerns:
Battery life not meeting advertised duration, especially with advanced features enabled.
Complaints about charging issues or short charging cables.
* App and Feature Limitations:
Users report app bugs, limited features, or a lack of customization options.
Discontent with mandatory app use for essential functions.
* Physical and Design Concerns:
Size and weight affecting portability.
Limited color options or aesthetic features.
Durability concerns with refurbished products or specific components.
2. Ease of Use:
* Generally Positive Feedback:
Most products are praised for easy setup and straightforward controls.
Seamless Bluetooth connectivity and user-friendly apps (with some exceptions).
Portability and intuitive design are frequently mentioned.
* Minor Usability Issues:
Occasional difficulty with setup instructions or connecting to multiple devices.
Some features, such as spatial audio or advanced sound modes, require specific placements or settings, which can be challenging.
3. Reasons for Purchase:
* Sound Quality:
Many users prioritize rich, clear sound with good bass and balanced audio for a variety of music genres.
Speakers with customizable EQ settings are particularly appealing.
* Design and Portability:
Compact, durable designs with waterproof or rugged features are highly valued for outdoor use.
Lightweight and easy-to-carry speakers with practical design elements like handles or straps are preferred.
* Value for Money:
High sound quality and durability for the price point, especially when discounted or on sale.
Attractive offers on refurbished or renewed models.
* Brand Trust and Features:
Well-known brands and built-in features like smart assistants (Alexa) add to the purchase appeal.
Specific features like multi-device connectivity, long battery life, and unique sound enhancement modes are key selling points.

Sources
1. Research Papers:
* He, S., et al. (2022). Detecting fake-review buyers using network structure: Direct evidence from Amazon. PNAS, 119(47), e2211932119. https://doi.org/10.1073/pnas.2211932119
2. Blog Posts:
* Patel, N. (2023). 15 Product Marketing Strategies Proven to Increase Sales. Neil Patel. https://neilpatel.com/blog/product-marketing-strategies/
* RJ Audio. (2023, October 3). What are the best features of Bluetooth speakers. RJ Audio. https://www.rjbluetoothspeaker.com/blog/the-best-features-of-bluetooth-speakers/
3. User Data:
* CSV file with product IDs and reviews scraped from Amazon using GEMINI AI and sentiment analysis data.
4. Tools
Data Analysis:
* Pandas: For data management and analysis.
* Python: For processing and analyzing data.
* Gemini AI: AI-generated insights.
* OxyLABs API: Scrape reviews from Amazon.
5. Visualization:
* Matplotlib: For creating graphs and plots.
* Seaborn: For advanced visualizations like violin plots.
6. Sentiment Analysis:
* VADER: For sentiment scoring.
* TextBlob: For polarity and subjectivity analysis.
7. References
* Insights on sentiment analysis, marketing strategies, and Bluetooth speaker features were drawn from the sources above, using APA style for citations.