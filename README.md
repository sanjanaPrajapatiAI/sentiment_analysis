# 🧠 FeelingsFinder - A Simple Sentiment Analyzer

```
  ______      _ _       _             
 |  ____|    (_) |     | |            
 | |__  __  ___| |_   _| | ___  ___   
 |  __| \ \/ / | | | | | |/ _ \/ __|  
 | |____ >  <| | | |_| | |  __/\__ \  
 |______/_/\_\_|_|\__,_|_|\___||___/  
                                      
         FeelingsFinder 🧠❤️
```

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

## 🧾 Full Code

```python
from textblob import TextBlob

def analyze_sentiment(text):
    blob = TextBlob(text)
    polarity = blob.sentiment.polarity
    subjectivity = blob.sentiment.subjectivity
    if polarity > 0:
        sentiment = "Positive"
    elif polarity < 0:
        sentiment = "Negative"
    else:
        sentiment = "Neutral"
    return sentiment, polarity, subjectivity

def main():
    print("Welcome to the Sentiment Analyzer!")
    while True:
        text = input("\nEnter text to analyze (or type 'exit' to quit): ")
        if text.lower() == 'exit':
            break
        sentiment, polarity, subjectivity = analyze_sentiment(text)
        print(f"\nSentiment: {sentiment}")
        print(f"Polarity Score: {polarity}")
        print(f"Subjectivity Score: {subjectivity}")
        print("-" * 50)

if __name__ == "__main__":
    main()
```

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

## 👩‍💻 Author

**Sanjana Prajapati**  
*BSc AIML | Passionate about AI and building creative tools*

---

## 📁 Folder Structure

```
FeelingsFinder/
│
├── sentiment_analyzer.py
└── README.md
```

---

> If you like this project, feel free to give it a ⭐ on GitHub or suggest new features!