# Financial News Sentiment Analysis using FinBERT

This project uses the [FinBERT](https://huggingface.co/ProsusAI/finbert) transformer model to perform sentiment analysis on financial news headlines sourced from Yahoo Finance RSS feeds. It visualizes sentiment trends (positive, negative, neutral) and calculates an overall sentiment score for a given stock ticker.

---

## 🔍 Features

- ✅ Scrapes financial headlines using Yahoo Finance RSS feed  
- ✅ Filters relevant news using keywords  
- ✅ Analyzes sentiment using FinBERT (finance-trained BERT)  
- ✅ Calculates overall sentiment score  
- ✅ Visualizes sentiment distribution with a pie chart

---
## Customization
Change the ticker or keyword at the top of the script:
ticker = 'META'
keyword = 'meta'

## 🧠 How it Works
You specify a stock ticker (e.g., META) and a keyword (meta).

It pulls recent news from:
http://finance.yahoo.com/rss/headline?s=META
It filters articles containing your keyword in the summary.

The FinBERT model analyzes the sentiment of each summary.

It prints:

News title, link, publish date, and summary

Sentiment result and confidence score

Computes an overall score and visualizes it with matplotlib.

## 📦 Dependencies

Install dependencies via pip:

```bash
pip install transformers
pip install feedparser
pip install matplotlib
```


🙌 Credits
FinBERT by ProsusAI

Yahoo Finance RSS Feeds

