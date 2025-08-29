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

### 2. Emotion Detection

Used Hugging Face’s [`j-hartmann/emotion-english-distilroberta-base`](https://huggingface.co/j-hartmann/emotion-english-distilroberta-base) model to classify each review into one of:

- Joy
- Anger
- Sadness
- Fear
- Disgust
- Surprise
- Neutral

### 3. Visualization

Built an interactive dashboard using **Streamlit** to:

- Explore emotion distributions
- Filter reviews by detected emotion
- View raw reviews and metadata

---

## 🧪 Sample Output

| Review                                                 | Emotion |
|--------------------------------------------------------|---------|
| Absolutely love this product, it smells amazing!       | Joy     |
| I received a broken item, very disappointed.           | Sadness |
| What a waste of money. Do not buy!                     | Anger   |

---


```bash
streamlit run app.py
