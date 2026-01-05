# 🎵 Spotify Lyric Search – Text Identification Model

## 📌 Project Overview
This project implements a **lyric-based text identification system** that predicts the **song title** and **artist name** when a short snippet of song lyrics is provided as input.

The main goal of this task is to demonstrate the application of **text preprocessing techniques** and a **similarity-based approach** for identifying songs using lyrics.

---

## 📊 Dataset Information
- **Dataset Name:** Spotify Million Song Dataset  
- **Total Records:** 57,651  
- **Columns Used:**
  - `artist`
  - `song`
  - `text` (lyrics)

The dataset is sourced from **Kaggle** and contains song lyrics along with their respective artist and song titles.

Due to GitHub file size limitations, the complete dataset is **not included** in this repository.

---

## 📁 Dataset Access
The full dataset can be downloaded from Kaggle using the link below:

🔗 https://www.kaggle.com/datasets/joebeachcapital/57651-spotify-songs

For reference and testing purposes, a **sample dataset (`spotify_sample.csv`)** is included in this repository.

---

## 🛠️ Technologies Used
- **Python**
- **Pandas**
- **Natural Language Processing (NLP)**
- **Scikit-learn**
- **Jupyter Notebook**

---

## ⚙️ Methodology
1. Lyrics text is preprocessed using:
   - Lowercasing
   - Tokenization
   - Stop-word removal
   - Removal of punctuation and special characters
2. **TF-IDF Vectorization** is applied to transform text data into numerical form.
3. **Cosine Similarity** is used to measure similarity between lyric snippets.
4. The most similar lyric entry is selected to predict the **song title** and **artist**.

This approach is effective for **lyric-based search and text matching applications**.

---

## 🎯 Model Usage
The model accepts a short lyric snippet as input and returns:
- **Predicted Song Title**
- **Predicted Artist**

### Example Input: she makes me feel fine who could ever believe
### Example output: Predicted Song Title: She's My Kind Of Girl
Predicted Artist: ABBA


---

## 📈 Model Evaluation
Model performance is demonstrated within the **Jupyter Notebook** by comparing predicted results with actual song titles from a test dataset.

---

## 🚀 Installation & Execution
1. Open the Jupyter Notebook file  
2. Ensure the dataset is available:
   - Download the full dataset from Kaggle, or  
   - Use the provided `spotify_sample.csv`  
3. Run all cells in sequence  
4. Enter a lyric snippet in the input cell to test the model  

➡️ No additional setup is required.

---

## 📝 Notes
- This project follows a **similarity-based text identification approach**  
- Focus is on clarity, correctness, and ease of understanding  
- All work is **original** and complies with the **no-plagiarism policy**



