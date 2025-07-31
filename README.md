

````markdown
# 🎯 Sentiment Analysis of Movie Reviews

This project performs sentiment analysis on movie reviews using natural language processing (NLP) techniques and a logistic regression classifier. It predicts whether a given review is **Positive** or **Negative**.

---

## 📁 Dataset

The dataset file should be named `dataset.csv` and must contain:

- `review`: Raw text of the review
- `sentiment`: Corresponding label — `positive` or `negative`

---

## 🧰 Libraries Used

- `nltk` (for tokenization & stopwords)
- `spacy` (for lemmatization)
- `pandas`, `re` (for data handling and regex)
- `scikit-learn` (for model training and evaluation)
- `matplotlib`, `seaborn` (for plotting)

---

## ⚙️ Workflow Overview

### 1. Preprocessing
- Remove HTML tags
- Lowercasing
- Remove punctuation and numbers
- Tokenization
- Stopword removal
- Lemmatization using SpaCy

### 2. Feature Extraction
- TF-IDF vectorization (top 5000 words)

### 3. Model
- Logistic Regression (using `liblinear` solver)

### 4. Evaluation
- Accuracy Score
- Classification Report
- Confusion Matrix (plotted with seaborn)

---

## 🧪 Sample Predictions

```text
Review: "This movie was absolutely fantastic! The acting was superb and the plot was gripping."
Prediction: Positive

Review: "I was so bored throughout the entire film. It was a complete waste of time and money."
Prediction: Negative

Review: "The film was okay, not great but not terrible either. Some parts were good."
Prediction: Negative
````

---

## 📊 Example Output: Confusion Matrix

Confusion matrix of predictions on the test set:

|                 | Predicted Negative | Predicted Positive |
| --------------- | ------------------ | ------------------ |
| Actual Negative | 43                 | 7                  |
| Actual Positive | 6                  | 44                 |

---

## 🏁 Getting Started

### 🛠️ Requirements

Install dependencies via:

```bash
pip install nltk spacy pandas scikit-learn matplotlib seaborn
python -m nltk.downloader stopwords punkt
python -m spacy download en_core_web_sm
```

### ▶️ Run the Notebook

1. Make sure your `IMDB Dataset.csv` is in the same directory.
2. Open the notebook:

```bash
jupyter notebook HR_Screening.ipynb
```

---
## 📂 Project Structure

```text
resume_job_matcher/
├── imdb-dataset/
│   └── IMDB Dataset.csv
├── sample.ipynb
├── README.md

---

## 🙋‍♂️ Author

**Raheen Bukhari**

📧 Email: [raheenbukhari.01@gmail.com](mailto:raheenbukhari.01@gmail.com)
🔗 LinkedIn: [@syeda-raheen-bukhari](https://www.linkedin.com/in/syeda-raheen-bukhari-5366aa2b2/)

---


