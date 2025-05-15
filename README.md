# 🗣️ Inaugural Address NLP Analysis — U.S. Presidents

This project analyzes the **first inaugural speeches** of the last five U.S. Presidents:

- **Bill Clinton**
- **George W. Bush**
- **Barack Obama**
- **Donald Trump**
- **Joe Biden**

Natural Language Processing (NLP) techniques are used to explore their rhetorical styles, sentiment, and language patterns.

---

## 📁 Project Structure

<pre>

├── inaugural_speeches.txt    # Combined speech file (separated by "===" and tagged with -lastname)
├── inaugural_analysis.ipynb  # Main Jupyter Lab analysis notebook
├── README.md
  
</pre>


---

## 🧪 Goals & Methods

The main objective is to **compare and contrast the linguistic characteristics** of these presidents' inaugural addresses using NLP.

### ✅ Preprocessing
- Speech file parsing and separation by president (`-lastname` tags)
- Sentence tokenization, punctuation handling, and abbreviation normalization (e.g., `U.S.` → `US`)
- Text cleaning and stopword removal

### 🔍 Analyses Performed

| Task                         | Description |
|------------------------------|-------------|
| **Sentence & Word Counts**   | Measures speech length and complexity |
| **Word Frequency Analysis**  | Most common words and bigrams/trigrams |
| **Word Clouds**              | Visual summary of key terms |
| **Sentiment Analysis**       | Using `TextBlob` for polarity & subjectivity |
| **TF-IDF**                   | Signature terms unique to each speaker |
| **Conclusion & Observations**| High-level comparison of styles and tones |

---

## 📊 Summary Table

| President | Sentences | Words | Avg Sentence Length | Polarity | Subjectivity |
|-----------|-----------|-------|----------------------|----------|--------------|
| Clinton   | 93        | 1,582 | 17.01                | 0.15     | 0.51         |
| Bush      | 97        | 1,582 | 16.31                | 0.19     | 0.47         |
| Obama     | 122       | 2,398 | 19.66                | 0.09     | 0.47         |
| Trump     | 86        | 1,439 | 16.73                | 0.15     | 0.40         |
| Biden     | 185       | 2,506 | 13.55                | 0.17     | 0.46         |

---

## 📝 Observations

- **Biden** gave the longest speech but used shorter, simpler sentences—conveying optimism with the second-highest sentiment polarity.
- **Obama** favored long, thoughtful sentences with a more neutral tone.
- **Bush** delivered the most positive speech overall, albeit in a concise format.
- **Clinton and Trump** had similar sentence structure and polarity, but Trump used noticeably less subjective language.

These findings show how each leader's style reflects not only their personal rhetoric but the political climate at the time.

---

## ⚙️ Tools Used

- Python 3.x
- Jupyter Lab
- `nltk`, `textblob`, `matplotlib`, `seaborn`, `sklearn`, `wordcloud`, `pandas`

---

## 📌 How to Run

1. Clone the repository and open the `notebooks/inaugural_analysis.ipynb` file in Jupyter Lab.
2. Ensure you have all required Python libraries:
   ```bash
   pip install -r requirements.txt
