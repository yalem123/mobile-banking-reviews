# 📊 Mobile Banking App Reviews Analysis

**Omega Consultancy Challenge Project**
*Analyzing customer satisfaction with mobile banking apps in Ethiopia*

## 🚀 Project Overview

This project analyzes Google Play Store reviews of mobile banking apps from three major Ethiopian banks:

* Commercial Bank of Ethiopia (CBE)
* Bank of Abyssinia (BOA)
* Dashen Bank

The goal is to help Omega Consultancy provide actionable recommendations to improve customer satisfaction, retention, and app features.

---

## 📂 Repository Structure

| Branch   | Description                       |
| -------- | --------------------------------- |
| `task-1` | Data Collection and Preprocessing |
| `task-2` | Sentiment and Thematic Analysis   |
| `task-3` | Database Storage                  |
| `task-4` | Insights and Recommendations      |

---

## ✨ Project Tasks

### ✅ Task 1: Data Collection and Preprocessing

* Scraped 400+ reviews per bank using `google-play-scraper`.
* Preprocessed data:

  * Removed duplicates.
  * Normalized dates.
  * Saved clean dataset to CSV.

### ✅ Task 2: Sentiment and Thematic Analysis

* Applied sentiment analysis using VADER.
* Extracted and clustered keywords using TF-IDF.
* Defined 3-5 key themes per bank.
* Mapped themes to individual reviews.

### 🕑 Task 3: Database Storage

* Store cleaned data in PostgreSQL database (Neon).
* Define schema for Banks and Reviews tables.
* Insert data using Python.

### 🕑 Task 4: Insights and Recommendations

* Visualize sentiment trends and rating distributions.
* Identify drivers of satisfaction and pain points.
* Provide actionable recommendations for each bank.
* Document potential review biases.



## 🗂️ Dataset

* Total reviews collected: **\~1200+**
* Fields:

  * `review_text`
  * `rating`
  * `date`
  * `bank`
  * `source`
  * `sentiment_label`
  * `sentiment_score`
  * `identified_theme(s)`



## 📌 Technologies Used

* **Python**: Main language (Google Colab used for development)
* **google-play-scraper**: Web scraping reviews
* **Pandas / NumPy**: Data processing
* **VADER / NLTK / spaCy**: Sentiment and NLP analysis
* **TF-IDF (sklearn)**: Keyword extraction
* **PostgreSQL (Neon.tech)**: Database storage
* **Matplotlib / Seaborn**: Data visualization
* **GitHub**: Version control and project management



## Limitations and Ethical Considerations

* Reviews may have selection bias (negative skew common).
* Some reviews are short or ambiguous and may affect sentiment/theme accuracy.
* Only public data from Google Play Store used.



##  Project Status

✅ Task 1 Completed
✅ Task 2 Completed
   Task 3 In Progress
  Task 4 Planned


## 💻 How to Run

1. Clone the repo
2. Follow task branch-specific README for setup and scripts
3. Run in Google Colab or local environment


*Developed by Yalem for Omega Consultancy Challenge in TEN Academy*


# How to Use

👉 Just copy this and save it as `README.md` in your main branch
👉 Update status of tasks as you progress
👉 This looks very professional for reviewers

