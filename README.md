# E-Commerce-App-User-Review-Topic-Prediction

🛍️🌐 Predictive Modeling of E-commerce App User Review Topics from Google Play Store using LDA and LSI.

## Project Overview
This project focuses on extracting topics from user reviews of an e-commerce application scraped from Google Play. By applying Latent Dirichlet Allocation (LDA) and Latent Semantic Indexing (LSI), this project aims to identify key aspects that users commonly comment on, providing insights into user feedback and helping to improve user experience.

### Notice
This code was developed as a final project for the **Text Mining** class. The primary goal is to apply theoretical knowledge of text mining techniques to real-world data, allowing contributors to gain practical experience in analyzing textual data, understanding user sentiments, and extracting actionable insights for business applications.

## Installation and Setup
To reproduce this project, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   ```
2. **Install required packages:**  
   This project requires Python 3.x and can be run on Google Colaboratory, where necessary packages can be installed with:
   ```python
   # Example package installations
   !pip install <package-name>
   ```

3. **Run Jupyter Notebooks:**
   The project is structured as Jupyter Notebook files, which can be run directly in Google Colaboratory or any other Jupyter-supported environment.

## Codes and Resources Used
- **Language:** Python
- **Editor:** Google Colaboratory

### Python Version
The code is compatible with Python 3.x, and specific package versions may be required for certain functionalities.

## Packages Used
Below are the primary packages utilized, categorized by purpose:

- **General Purpose:** `os`, `json`
- **Text Scrapping:**: `google_play_scraper`
- **Data Manipulation:** `pandas`, `numpy`
- **Text Preprocesing:** `re`, `emoji`, `nltk`
- **Data Visualization:** `matplotlib`, `seaborn`, `pyLDAvis`, `wordcloud`
- **Machine Learning:** `sklearn`, `gensim` 

## Data Overview
The dataset contains user reviews scraped from the Google Play store for e-commerce applications (Shopee, Tokopedia, Lazada, Blibli, Zalora, Bukalapak, OLX, Alibaba), which will be used to understand key user concerns and preferences.

The data includes various attributes such as:
- **userName:** The name of the user.
- **Score:** User rating for the app.
- **at:** Date and time of the review.
- **content:** User review for the app.
- **app_name:** The name of the application

## Results and Evaluation
The analysis of the user reviews revealed important insights into the effectiveness of the topic modeling approaches:

1. **Model Comparison:**
   - **LDA models** are effective for identifying broader themes in large datasets, while **LSI models** excel in capturing sub-themes, providing a more detailed understanding of user discussions.
   
2. **Impact of Methods:**
   - Utilizing **Bag-of-Words (BoW)** and **TF-IDF** methods has refined the identification of sub-themes within the broader categories. However, the influence of TF-IDF on sentiment analysis requires further investigation.

3. **Best Models:**
   - **Model 6 (BoW + TF-IDF, LDA, Tuned)** demonstrates the highest coherence score, suggesting strong performance. Yet, **Model 5 (BoW, LDA, Tuned)** is preferred for its stability, pending further research on TF-IDF effects.
   - **Model 7 (BoW, LSA, Tuned)** and **Model 8 (BoW + TF-IDF, LSA, Tuned)** are also viable, with Model 7 being a conservative choice until the impact of TF-IDF is fully understood.

In summary, it is currently recommended to use **Model 5** for broader topics and **Model 7** for detailed topics. Should future research confirm the neutrality of TF-IDF on sentiment analysis, **Model 6** and **Model 8** would be favored for broader and detailed topics, respectively.

## Contributors
- **Alisha Zahra Saadiya** - 2501971742
- **Diva Nabila Henryka** - 2501975620
- **Lovina Anabelle Citra** - 2540121322
