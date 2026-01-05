# 🧭 Weekend Getaway Ranker – Travel Recommendation System

## 📌 Overview
This project implements a **rule-based recommendation system** that ranks suitable **weekend travel destinations in India** based on a given source city.

The objective is to help users discover **nearby, popular, and practical destinations** that are ideal for short weekend trips.

---

## 📊 Dataset Description
The project uses a travel dataset containing information about major tourist destinations across India.

### Key Fields Used:
- City  
- State  
- Zone  
- Tourist Place Name  
- Google Review Rating  
- Number of Google Reviews  

The dataset provides sufficient details to generate meaningful rankings **without relying on external APIs**.

---

## ⚙️ Ranking Approach
Destinations are ranked using a weighted scoring mechanism based on three factors:

### 1️⃣ Distance Proximity
Since exact geographical distances were not available, proximity was estimated logically using:
- Same city  
- Same state  
- Same zone  
- Different zone  

Higher penalties were assigned to distant locations to ensure **realistic weekend recommendations**.

---

### 2️⃣ Rating Score
Google review ratings were **normalized** and used to represent overall visitor satisfaction.

---

### 3️⃣ Popularity Score
Popularity was derived from the **number of Google reviews** and normalized to maintain scale consistency.

---

### 🔢 Final Scoring Weights
- **Distance Score:** 45%  
- **Rating Score:** 35%  
- **Popularity Score:** 20%  

Destinations are ranked based on the **final combined score**.

---

## 📁 Files Included
- `weekend_getaway_ranker.py` – Python script implementing the ranking logic  
- `requirements.txt` – Required Python dependency  
- `sample_output.txt` – Sample ranked results for selected source cities  

---

## 🚀 How to Run
1. Ensure the dataset CSV file is present in the same directory as the script  
2. Install the required dependency using `requirements.txt`  
3. Run the Python script  
4. Enter a source city when prompted  
5. View the ranked list of recommended weekend destinations  

---

## 🏙️ Sample Cities Tested
- Delhi  
- Mumbai  
- Kolkata  

Outputs for these cities are included in the `sample_output.txt` file.

---

## 📝 Notes
- This project focuses on **data engineering and ranking logic**, not machine learning  
- The solution is designed to be **simple, explainable, and practical**  
- All work is **original** and complies with the **no-plagiarism policy**

