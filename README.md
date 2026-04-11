# ML1-Final-Project

# Sentiment Analysis of Cristiano Ronaldo vs Lionel Messi Tweets

This project presents a complete Natural Language Processing (NLP) pipeline for sentiment analysis on social media data. The study focuses on tweets related to two of the most influential football players: Cristiano Ronaldo and Lionel Messi.

The objective is to explore how fans express opinions online and to evaluate the performance of classical machine learning models for sentiment classification.

---

## Project Structure

```
.
├── ML1_Final_Project.ipynb          # Full implementation (data processing, modeling, analysis)
├── ML1_Report_Final_Project.pdf     # Final report (paper format)
└── README.md                        # Project overview
```

---

## Methodology

The project follows a complete machine learning workflow:

### 1. Data Preprocessing

* Text cleaning (URLs, mentions, special characters)
* Tokenization and lemmatization
* Stopword removal

### 2. Sentiment Labeling

* Sentiment scores generated using VADER (lexicon-based approach)

### 3. Feature Engineering

* TF-IDF vectorization to transform text into numerical features

### 4. Model Training

Four classifiers were trained and compared:

* Support Vector Machine (SVM)
* Multinomial Naive Bayes
* Logistic Regression
* Random Forest

### 5. Evaluation

* Train-test split
* Cross-validation
* Metrics: Accuracy, Precision, Recall, F1-score
* Confusion matrix analysis

---

## Key Results

* **Best model:** Support Vector Machine (SVM)
* **Test accuracy:** 80.46%
* Strong and balanced F1-scores across sentiment classes

### Insights:

* Social media sentiment towards both players is predominantly positive
* Vocabulary and topics are highly similar across fanbases
* Differences in sentiment exist, but are relatively small

---

## Limitations

* Sentiment labels were generated using VADER, meaning models learn to approximate its behavior rather than human-annotated sentiment
* TF-IDF does not capture semantic relationships between words
* Analysis was conducted on a 100k sample for computational efficiency

---

## Future Work

* Use deep learning models (LSTM, Transformer-based models such as BERT or RoBERTa)
* Incorporate word embeddings (Word2Vec, GloVe, FastText)
* Fine-tune pretrained language models for social media data
* Include user metadata and engagement features
* Apply data augmentation or semi-supervised learning

---

## Technologies Used

* Python
* SpaCy
* Pandas & NumPy
* Scikit-learn
* NLTK
* Matplotlib & Seaborn

---

## How to Run

1. Clone the repository:

```bash
git clone https://github.com/Daniseralz/ML1-Final-Project.git
cd ML1-Final-Project
```

2. Open the notebook:

```bash
jupyter notebook ML1_Final_Project.ipynb
```

3. Run all cells

---

## Report

The full analysis and discussion can be found in:

`ML1_Report_Final_Project.pdf`

---

## Author

Daniel Serrano Alzamora
