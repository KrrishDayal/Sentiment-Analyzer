# Daily Journal Sentiment Tracker

A simple Python project that lets you log daily diary entries, analyzes their sentiment using **VADER** sentiment analysis, and visualizes your emotional trends over time 📈.

## Features

- Prompt-based daily journaling
- Sentiment analysis using `nltk`'s VADER
- Auto-log sentiment scores to a CSV file
- Line chart visualization of sentiment trends
- Automatically updates the CSV if the entry for a day already exists

## How It Works

1. The script prompts you to write your daily journal entry in the terminal.
2. It analyzes the emotional tone of your entry using the **VADER SentimentIntensityAnalyzer** from NLTK.
3. A **compound sentiment score** (ranging from -1 to 1) is generated:
   - Positive (> 0.05)
   - Neutral (between -0.05 and 0.05)
   - Negative (< -0.05)
4. This score, along with the current date, is logged in a CSV file named `journal_sentiment.csv`.
5. If an entry for the same date already exists, it will be updated instead of duplicated.
6. Finally, the script plots a **line chart** showing how your sentiment has changed over time.
