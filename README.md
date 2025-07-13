# 🧠 FeelingsFinder - A Simple Sentiment Analyzer

## 📌 Overview

**FeelingsFinder** is a beginner-friendly **Python** tool that uses **TextBlob** to perform sentiment analysis on user-inputted text. It classifies the sentiment as **Positive**, **Negative**, or **Neutral**, and provides **polarity** and **subjectivity** scores.

---

## ✅ Features

- Analyze sentiment in real-time from user input
- Provides:
  - Sentiment (Positive / Negative / Neutral)
  - Polarity score (range: -1 to 1)
  - Subjectivity score (range: 0 to 1)
- Loops until user types `exit`
- Easy to use and modify

---

## 🔧 Installation

1. Make sure Python is installed.
2. Install **TextBlob** using pip:
   ```bash
   pip install textblob
   ```
3. Download TextBlob corpora:
   ```bash
   python -m textblob.download_corpora
   ```

---

## 🚀 How to Run

1. Save the code below as `sentiment_analyzer.py`
2. Run the script in terminal:
   ```bash
   python sentiment_analyzer.py
   ```
3. Enter any sentence to analyze.

---

## 📊 Sample Output

```
Welcome to the Sentiment Analyzer!

Enter text to analyze (or type 'exit' to quit): I love programming and learning new things!

Sentiment: Positive
Polarity Score: 0.5
Subjectivity Score: 0.6
--------------------------------------------------
```

---

## 💡 Future Ideas

- Add a GUI using Tkinter or Streamlit
- Store analysis history in a file
- Support batch text analysis
- Add emoji or color-based output

---