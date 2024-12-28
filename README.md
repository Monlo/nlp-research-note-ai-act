# Identifying AI’s Environmental Risks: Using NLP to Analyzing Public Consultation Feedback on the AI Act 

This repository contains code and resources for analyzing public consultation feedback on the **AI Act**, focusing on environmental and climate-related concerns identified by stakeholders. The analysis involves **data scraping, cleaning, preprocessing, and textual analysis** to extract insights from feedback submitted by various stakeholders.

The workflow follows key **Natural Language Processing (NLP)** techniques,  data scraping, sentence extraction, keyword filtering, and textual analysis to identify and analyze recurring themes and patterns in the feedback data.

---

## **Repository Structure**

### **data/**  
- Contains raw and processed datasets.

### **notebooks/** 

#### **01_scrapping.ipynb**  
- Scrapes public consultation feedback data from the **[European Commission's website](https://ec.europa.eu/info/law/better-regulation/have-your-say/initiatives/12527-Artificial-intelligence-ethical-and-legal-requirements_e)**.  

#### **02_data_cleaning.ipynb**  
- Cleans and standardizes the scraped text data.  

#### **03_preprocessing.ipynb**  
- Performs Exploratory Data Analysis, extracts environmental risk mentions, generates word clouds, trains a Word2Vec model, and visualizes word embeddings 

#### **04_analysis.ipynb**  
- Applies sentence embeddings, UMAP dimensionality reduction, and KMeans clustering to group environmental risk feedback into semantic clusters.
- Summarizes cluster content using a pre-trained summarization model (BART) to highlight key insights

### **output/**  
- Stores outputs generated from the analysis notebooks,

---

## **Technologies Used**

- **Data Collection and Scraping:** `selenium`  
- **Data Cleaning and Preprocessing:** `pandas`, `numpy`, `re`  
- **Natural Language Processing (NLP):** `nltk`, `Word2Vec`, `transformers`, `langdetect`, `langid`  
- **Exploratory Data Analysis (EDA):** `CountVectorizer`  
- **Machine Learning Models:**  
   - **Clustering:** `KMeans`  
   - **Dimensionality Reduction:** `umap-learn`  
   - **Sentence Embeddings:** `Word2Vec`, `transformers`  
   - **Summarization:** `torch`, `transformers`  
- **Visualization:** `matplotlib`, `seaborn`, `wordcloud` 
