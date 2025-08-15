# 📱 TikTok Google Play Reviews Sentiment Analysis using Machine Learning

This project performs **Sentiment Analysis** on TikTok app reviews collected from **Google Play Store**.  
It uses **Natural Language Processing (NLP)** techniques to clean the data, generate **word clouds**, and determine **positive, negative, and neutral sentiment scores** using the **VADER Sentiment Analyzer**.

---

## 📌 Features
- Cleans raw review text (lowercasing, punctuation removal, stopword removal, stemming).
- Visualizes **rating distribution** using Plotly donut chart.
- Generates **word clouds** for:
  - All reviews
  - Positive reviews
  - Negative reviews
- Calculates **sentiment scores** (Positive, Negative, Neutral).
- Classifies the **overall sentiment** of the dataset.

---

## 📂 Dataset
The dataset (`tiktok_google_play_reviews.csv`) contains:
- `content` → User review text.
- `score` → Star rating (1–5).

---

## 🛠 Steps Performed

### 1️⃣ Data Preprocessing
- Removed `NaN` values.
- Selected only `content` and `score` columns.
- Applied a `clean()` function to:
  - Lowercase all text
  - Remove HTML tags, URLs, and punctuation
  - Remove stopwords
  - Apply **stemming** using NLTK's SnowballStemmer

### 2️⃣ Exploratory Data Analysis
- **Rating Distribution**: Created a **donut pie chart** to visualize the number of reviews per rating.
- **Overall Word Cloud**: Generated a **WordCloud** for the most frequent words in reviews.

### 3️⃣ Sentiment Analysis
- Used **VADER SentimentIntensityAnalyzer** from NLTK to calculate:
  - **Positive**
  - **Negative**
  - **Neutral** scores for each review.
- Aggregated total scores:

Positive: 196,353
Negative: 16,512
Neutral: 244,169
Overall Sentiment: Neutral 🙂


---
🏷 License

This project is open-source under the MIT License.

---
Author


Saniya Chhabra
---
