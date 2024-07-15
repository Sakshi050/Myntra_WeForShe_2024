# Trend-Centric Recommendations System
Employ AI-driven recommendation system that analyze current fashion trends, customer preferences, and purchase history to deliver tailored product suggestions, enhancing customer engagement and conversion rates in the fast fashion segment.
In the dynamic world of fashion, staying ahead of trends, understanding customer preferences and purchase history to deliver tailored product suggestions, is crucial. Our project addresses the challenge of providing trend-centric recommendations using AI-driven systems. It focuses on enhancing customer engagement and conversion rates in the fast fashion segment.
## Goal of our project
The main goal of this project is to provide a personalized fashion recommendation system that can help users find fashion products that match their preferences.
## Key Objectives
**1) Customer Preference Analysis:** Understand and predict customer preferences based on past behaviors, trends and customer purchase history.

**2) Trend Analysis:** Utilize AI to identify and analyze current fashion trends.

**Personalized Recommendation:** Provide tailored fashion recommendations to enhance the shopping experience.

## Data Collection and Preprocessing
• Sources include customer reviews, sales data, and social media trends. The data can be extracted from various online shopping sites like Myntra through Web Scraping. 

**Tools used:** Selenium, Octoparse, Beautiful Soup, Scrapy etc.

• Data cleaning and preprocessing to ensure accuracy.

Data Cleaning
   
    --> Missing Data
      Ignore the tuple and fill missing values(manually by mean or by most probable value)
          
    --> Noisy Data
      Remove these type of data through Regression and Clustering

Data Transformation
   
    --> Normalization   
    
    --> Attribute Selection

Data Reduction
   
    --> Data Cube Aggregation
    
    --> Attribute Subset Selection

    --> Dimensionality Reduction

## Model Developement
• Collaborative Filtering Model:

    --> Analyzes user-item interactions to provide recommendations based on user similarities.
  
    --> Tools used are: Alternating Least Squares (ALS) algorithm, KNN from the implicit library

• Content-Based Filtering Model:

    --> Uses attributes of items (e.g., category, brand, material) to recommend similar items.

    --> Tools used are: TF-IDF, Cosine Similarity, NLTK, spaCy from the implicit library

## Hybrid System

Combines collaborative and content-based filtering for more accurate and comprehensive recommendations.

The goal of the hybrid system is to improve the accuracy and robustness of recommendations

## Tools and Technologies used overall:
• Python Libraries:

  Pandas: For data manipulation and preprocessing.
  
  NumPy: For numerical operations.
  
  scikit-learn: For feature extraction (TF-IDF) and similarity calculations.
  
  SpaCy: For advanced natural language processing.
  
  implicit: For collaborative filtering using ALS.
  
  SciPy: For sparse matrix operations.

  
• Model Training and Evaluation:

  TensorFlow/Keras: For building deep learning and neural network models.
  
  PyTorch: For developing and training complex models.
  
  scikit-learn: For evaluation metrics and machine learning algorithms.
