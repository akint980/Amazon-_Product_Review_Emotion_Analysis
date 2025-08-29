# 🧠 Amazon Product Review Emotion Analysis

This project focuses on extracting, cleaning, and analyzing **Amazon product reviews** to detect the **emotional tone** behind user feedback using **transformer-based NLP models**.

While traditional sentiment analysis classifies reviews as positive or negative, **emotion analysis** dives deeper — identifying human emotions such as **joy**, **anger**, **sadness**, and more. These insights can help brands better understand their customers and improve products and services.

---

## 🎯 Project Objectives

- Extract Amazon reviews from OpenDataBay
- Clean and preprocess textual data
- Apply a transformer-based model to classify the **dominant emotion** in each review
- Visualize and analyze emotional trends across the dataset

---

## 📦 Dataset

- **Source**: [OpenDataBay - Amazon Product Queries and Reviews](https://www.opendatabay.com/)
- **Fields Used**:
  - `query`: Product search query
  - `ori_review`: Original user review
  - `ori_rating`: User rating (1–5 stars)

---

## 🛠️ Process Overview

### 1. Data Cleaning

- Removed duplicates and missing reviews
- Removed URLs and special characters
- Lowercased text
- Removed reviews shorter than 10 characters

### 2. Sentiment Analysis
<img width="547" height="115" alt="image" src="https://github.com/user-attachments/assets/d521b768-de19-4ea5-8c71-0727fb582af4" />

###3. Emotion Analysis
Used Hugging Face’s [`j-hartmann/emotion-english-distilroberta-base`](https://huggingface.co/j-hartmann/emotion-english-distilroberta-base) model to classify each review into one of:

- Joy
- Anger
- Sadness
- Fear
- Disgust
- Surprise
- Neutral
## 🧪 Output
<img width="704" height="128" alt="image" src="https://github.com/user-attachments/assets/446dc031-7098-4020-8d1f-ce27f4cc70ef" />

### 4. Visualization
<img width="594" height="455" alt="image" src="https://github.com/user-attachments/assets/c61081fa-7ff2-456a-955a-ee329ffad3cd" />
Analysis of Sentiment Distribution:

-Positive sentiment dominates the reviews, with around 15,000 reviews. This indicates that most customers had a favorable experience or expressed positive emotions about the products.
-Neutral sentiment comes next with roughly 4,000 reviews. This could represent customers who were indifferent, factual, or neither strongly positive nor negative.
-Negative sentiment is the least frequent, with around 1,800 reviews. This means fewer customers expressed dissatisfaction or negative emotions.
-Sentiment distribution of the top 10 categories by total reviews per product category
<img width="487" height="289" alt="image" src="https://github.com/user-attachments/assets/b62c2f83-9283-48ee-9f84-207fe1db6498" />



### 5. Conclusion
While customers are generally pleased with their purchases on Amazon, addressing the concerns raised in neutral and negative reviews could help boost sales and enhance overall customer satisfaction



---



