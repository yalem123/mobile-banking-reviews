

## 📌 Project Overview

This project simulates a consulting task where I act as a Data Analyst at **Omega Consultancy**, helping Ethiopian banks improve their mobile banking apps.

Goals:

✅ Scrape app reviews from Google Play
✅ Analyze sentiment and extract key themes
✅ Identify customer satisfaction drivers and pain points
✅ Store cleaned data in a PostgreSQL database (Neon.tech)
✅ Visualize insights and provide actionable recommendations

---

## 🗺️ Project Structure

```
/data                  → Cleaned CSV files  
/notebooks             → Google Colab notebooks (scraping, analysis, visualization)  
/scripts               → Python scripts (functions, reusable code)  
/visuals               → Exported plots/images  
README.md              → Project documentation  
requirements.txt       → Project dependencies  
.gitignore             → Ignored files (e.g. .ipynb_checkpoints)  
```

---

## ⚙️ Tools & Technologies

* Google Colab (Python 3)
* google-play-scraper
* pandas
* nltk / VADER
* scikit-learn (TF-IDF)
* PostgreSQL (Neon.tech cloud database)
* Git & GitHub

## 🚀 Tasks Breakdown

### Task 1: Data Collection and Preprocessing

✅ Scraped **400+ reviews per bank** from Google Play Store
✅ Cleaned data:

* Removed duplicates
* Normalized dates (YYYY-MM-DD)
* Saved as `cleaned_reviews.csv`

**Source:** Google Play Store
**Columns:** `review`, `rating`, `date`, `bank`, `source`


### Task 2: Sentiment and Thematic Analysis

✅ Sentiment analysis using **VADER** and optionally **DistilBERT**
✅ Classified reviews into: **Positive**, **Neutral**, **Negative**

✅ Thematic analysis:

* Extracted significant keywords (TF-IDF)
* Grouped keywords into **3-5 main themes per bank**:

  * Account Access Issues
  * Transaction Performance
  * UI & UX
  * Support
  * Feature Requests

✅ Saved as `sentiment_theme_reviews.csv`



### Task 3: Store Cleaned Data in PostgreSQL

✅ Created database on Neon.tech
✅ Defined schema:

* `bank_reviews` table: stores cleaned reviews with sentiment and themes

✅ Inserted full dataset (> 1,000 reviews) using SQLAlchemy

---

### Task 4: Insights and Recommendations

✅ Visualizations:

* Sentiment distribution per bank
* Rating distribution per bank
* Word clouds of common keywords

✅ Insights:

* Identified top **drivers** and **pain points**
* Compared banks (CBE vs BOA vs Dashen)
* Provided **2+ actionable recommendations** per bank

✅ Ethical considerations:

* Acknowledge potential **review biases** (e.g. more negative reviews due to unhappy users)

## 💡 Key Insights

### CBE

**Drivers:** Fast navigation, user-friendly UI
**Pain Points:** Login issues during maintenance

### BOA

**Drivers:** New features (QR payment)
**Pain Points:** App crashes during transactions

### Dashen

**Drivers:** Fingerprint login support
**Pain Points:** Delayed OTP deliverables


## 📋 Recommendations

* Improve backend stability to avoid transaction errors
* Optimize app loading time, especially during transfers
* Enhance customer support response times within the app
* Monitor app reviews weekly for emerging issues


## ⚠️ Ethical Considerations

* Google Play reviews are subject to **selection bias**
* Highly dissatisfied users tend to post more reviews
* Recommendations should be validated with additional user feedback (e.g. surveys)



## 🗂️ How to Run the Project

### 1️⃣ Clone this repo


git clone https://github.com/yourusername/mobile-banking-reviews.git
cd mobile-banking-reviews

### 2️⃣ Install dependencies

pip install -r requirements.txt

### 3️⃣ Run notebooks

* Open Google Colab
* Upload and run notebooks in `/notebooks` folder

### 4️⃣ View database

* Connect to **Neon.tech** using your PostgreSQL credentials
* Explore `bank_reviews` table

## 🙏 Acknowledgments

* Ten academy 

## OUTCOME

✅ 1200+ reviews scraped
✅ Cleaned CSV produced
✅ Sentiment + themes analyzed
✅ Data stored in PostgreSQL
✅ Visuals and recommendations generated
