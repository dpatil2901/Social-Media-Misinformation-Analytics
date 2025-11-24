# 📰 Social Media Misinformation Analysis  


---
<img width="1536" height="1024" alt="ChatGPT Image Nov 24, 2025, 10_38_17 AM" src="https://github.com/user-attachments/assets/dec7652b-eb42-4831-989b-8c8d2872683a" />

## 🛠 Tech Stack

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Plotly**
- **Jupyter Notebook**

---
## 📌 Project Overview
The purpose of this project is to analyze social media data and uncover insights related to:

- Misinformation behavior and spread  
- Platform-wise trends  
- User posting patterns  
- Engagement differences  
- Geographic distribution  
- Fact-checking effectiveness  

The dataset contains **500 posts** collected across multiple platforms, with **31 features** including sentiment, toxicity, author details, factual similarity scores, timestamps, and misinformation labels.

---

## 📂 Dataset Summary

- **Rows:** 500  
- **Columns:** 31  
- **Target Variable:** `is_misinformation` (1 = misinformation, 0 = genuine post)

### Key Data Fields:
- Post metadata (author, platform, timestamp, location)
- Engagement metrics (likes, reposts, etc.)
- Linguistic features (readability, sentiment)
- AI detection signals (bot or synthetic likelihood)
- Fact-checking & source reliability details

---

## 🔧 Data Processing

Steps performed:

1. **Loading CSV dataset**
2. **Handling missing values**:
   - Median imputation for numeric fields
   - "Unknown" fill for categorical fields
3. **Duplicate removal**
4. **Feature engineering**:
   - Log scaling for large numeric values
   - Extracting posting hour
   - Binning follower count

---

## 📊 Key Insights

### 🅰 Platform Analysis
- **Twitter had the highest misinformation rate**
- **Reddit and Telegram misinformation posts received higher engagement**

### 🅱 User Behavior
- Verified and unverified users shared misinformation at **similar rates**
- Users with **higher follower counts posted slightly more misinformation**
- Misinformation was more common among posts with high **bot-likeness scores**

### 🅾 Content Characteristics
- No strong relationship was seen between misinformation and:
  - Readability  
  - Number of URLs, hashtags, or mentions  
  - Toxicity score

### 🕓 Time Trends
- Posting times fluctuated without a significant repeating pattern

### 🌎 Geographic Trends
- **Brazil, UK, and Germany had the highest misinformation levels**
- Brazil also showed the **highest engagement overall**

### 🧐 Fact-Checking & Reliability
- Posts with fact-checking received **lower engagement**
- Higher domain reliability correlated with **lower misinformation rates**

---

## 💼 Business Value

This analysis can help platforms:

- Identify high-risk platforms and regions  
- Improve early misinformation detection  
- Leverage synthetic/bot signals for automated flagging  
- Strengthen fact-checking visibility  
- Avoid assuming verified users are safer sources
