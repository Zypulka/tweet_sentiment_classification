# Tweet Text Analysis + Sentiment Classification (NLP)

This repository contains three notebooks prepared as coursework for the **“Introduction to Machine Learning”** class.  
The project follows an end-to-end NLP workflow on a tweets dataset: **EDA → feature engineering → modeling**.  
The goal is to analyze tweet content (topics, frequent words, hashtags) and build models that predict **sentiment**  from text.

---

## 1) Exploratory Data Analysis (EDA)

Work done in this stage:

- basic cleaning and label formatting,
- sentiment distribution and tweet length/token statistics,
- most frequent **words** and **hashtags** (overall and by sentiment),
- bigrams/collocations and keyword contrasts,
- lexicon sentiment signals (VADER / TextBlob / Afinn) and emotion-style cues (NRC, punctuation, caps).

Outcome: understanding what people talk about and which text patterns separate sentiments.

---

## 2) Feature Engineering

This stage focused on extracting stronger representations for downstream models:

- preprocessing pipeline: tokenization, stopwords, POS tagging, lemmatization,
- word embeddings (semantic features),
- engineered features: hashtag/mention/URL counts, negation, length, punctuation, uppercase ratios,
- sentiment/emotion features: VADER, TextBlob, Afinn, NRC.

Outcome: richer feature sets ready for modeling.

---

## 3) Modeling

Modeling notebook contains comparative experiments:

- baseline classifiers on TF-IDF,
- tree/boosting models trained on engineered features,
- neural network model trained on engineered features,
- transformer-based sentiment model (BERT).

Outcome: the **transformer-based model (BERT)** achieved the **best overall metrics**.  

Models trained mainly on **engineered features** (tree/boosting and neural network) also worked, but achieved **lower scores** compared to the transformer approach.
