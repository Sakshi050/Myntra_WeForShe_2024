# Trend-Centric Recommendations System
In the dynamic world of fashion, staying ahead of trends, understanding customer preferences and purchase history to deliver tailored product suggestions, is crucial. Our project addresses the challenge of providing trend-centric recommendations using AI-driven systems. It focuses on enhancing customer engagement and conversion rates in the fast fashion segment.
## Goal of our project
The main goal of this project is to provide a personalized fashion recommendation system that can help users find fashion products that match their preferences and also following the current trends.

## Key Objectives
**1) Trend Analysis:** Utilize AI to identify and analyze current fashion trends.

**2) Customer Preference Analysis:** Understand and predict customer preferences based on past behaviors, trends and customer purchase history.

**3) Personalized Recommendation:** Provide tailored fashion recommendations by integrating trend analysis and customer preference analysis to enhance the shopping experience.

# Methodology
## Data Collection and Preprocessing
- Sources include customer reviews, sales data, and social media trends. The data can be extracted from various online shopping sites like Myntra through Web Scraping. 

**Tools used:** Selenium

- Data cleaning and preprocessing to ensure accuracy.

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
- **Trend Analysis Model :**

   -> LSTM (Long short-term memory):      
   
      --> LSTMs are used to model user behavior over time, capturing the sequence of interactions, purchases,
      or browsing history to predict future preferences.                  
      
      --> LSTMs can analyze temporal data such as sales trends, seasonal patterns, and emerging fashion trends
      to forecast future trends and adjust recommendations accordingly.

- **Customer Preference Analysis Model :**

   -> Collaborative Filtering Model:

      --> Analyzes user-item interactions to provide recommendations based on user similarities.
  
      --> Tools used are: Alternating Least Squares (ALS) algorithm, KNN from the implicit library

   -> Content-Based Filtering Model:

      --> Uses attributes of items (e.g., category, brand, material) to recommend similar items.

      --> Tools used are: TF-IDF, NLTK, spaCy from the implicit library

- **Integrating the above models :**

      In this step the Trend Analysis Model and the Customer Preference Model are integrated together to provide tailored and personalized
      recommendations to the users according to their interests from the data we have acquired.

## Hybrid System

Combines collaborative and content-based filtering for more accurate and comprehensive recommendations.
The goal of the hybrid system is to improve the accuracy and robustness of recommendations.

The role of the model built is to:
- To extract winning designs from these real world products, we use a recommendation engine
- We feed trendy clothing items from social media to the recommender system.
- The job of the recommender system is to find the most similar images from the images obtained from Online Fashion Portals
![image](https://github.com/user-attachments/assets/bf8f18c5-fd83-42e1-98e2-e3b0dd8d041f)


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

## Screenshots:
**Simple UI**
![image](https://github.com/user-attachments/assets/9288e6d3-47a1-4a6a-9726-979b3bd37182)

This is the type of prototype we are planning to make for our recommendation system

## Repository Structure:

The repository contains several directories:

- **data:** This directory contains all the datasets.
- **models:** This directory contains the machine learning models' weights, excluding the large SAM model which is not included in the repo due to its size.
- **research:** This directory contains Jupyter notebooks file.
- **python scripts:** These are a series of Python files responsible for different steps in the pipeline. The order of execution is as follows:
    1. `data_preprocessing.py`
    2. `download_images.py`
    3. `image_segmentation.py`
    4. `latent_space_creator.py`
    5. `latent_space_clustering.py`

## How to Use

To use the project, run the python scripts in the order specified above. 

## Installation:

Use pip to install the requirements.

~~~bash
pip install -r requirements.txt
~~~

## Built With/Dependencies

- **OpenCV** - Open Source Computer Vision and Machine Learning software library
 
- **Tensorflow** - TensorFlow is an end-to-end open source platform for machine learning.

- **Tqdm** - tqdm is a Python library that allows you to output a smart progress bar by wrapping around any iterable.

- **streamlit** - Streamlit is an open-source app framework for Machine Learning and Data Science teams. Create beautiful data apps in hours, not weeks.

- **pandas** - pandas is a fast, powerful, flexible and easy to use open source data analysis and manipulation tool, built on top of the Python programming language.

- **Pillow** - PIL is the Python Imaging Library by Fredrik Lundh and Contributors.

- **scikit-learn** - Scikit-learn is a free software machine learning library for the Python programming language.

- **opencv-python** - OpenCV is a huge open-source library for computer vision, machine learning, and image processing.



## Results:
