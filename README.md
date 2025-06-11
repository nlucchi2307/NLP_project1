# NLP_project1

# Hotel Price Analysis During Events Using Text Mining and DiD

This project explores the effect of large events on hotel prices using a combination of web scraping, natural language processing, and econometric modeling.

## 🏙️ Context
We analyze how the **2025 Mobile World Congress in Barcelona** affects hotel prices, using **Madrid** as a control city. The methodology is based on a **Difference-in-Differences (DiD)** design.

## 🔍 Project Structure

### 1. Scraping
- Built a custom pipeline with a headless browser to scrape hotel listings from Barcelona and Madrid for selected date ranges.
- Scraper handles popups, infinite scroll, and description loading using multithreading.

### 2. Text Analysis (NLP)
- Cleaned hotel descriptions via tokenization, stopword removal, and stemming.
- Generated word clouds before/after preprocessing to visualize text changes.
- Text features were used later as control variables in the regression models.

### 3. Econometric Modeling
- Estimated the price effect using:
  - Simple DiD
  - DiD with controls (e.g. ratings)
  - DiD with fixed effects
  - DiD with text-based controls
  - DiD with heterogeneous treatment effects based on hotel quality

## 📈 Key Results
- Event increased average hotel prices by ~916€ (FE model).
- Text features helped identify higher-end hotels, where price increases were even larger.

## 📂 Files
- `web_scraping_pipeline.ipynb`: hotel data collection
- `text_analysis_DiD.ipynb`: preprocessing, word clouds, regression

## 👥 Authors
Text Mining and Introduction to NLP - BSE 2024-2025
Deepak Kumar Malik, Noemi Lucchi, Tirdod Behbehani  
