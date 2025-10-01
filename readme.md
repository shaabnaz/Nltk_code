# Lecture 01 — Text Preprocessing 

## Overview
This notebook (`lec_01.ipynb`) is an introductory lesson on **text preprocessing** for Natural Language Processing (NLP).  
It demonstrates basic steps to clean and prepare raw text for downstream tasks such as tokenization, feature extraction, and modeling.

## Main Topics Covered
- Text cleaning:
  - Lowercasing
  - Removing URLs, mentions, digits, and punctuation
  - Normalizing whitespace
- Tokenization (word-level and sentence-level)
- Stopword removal
- Stemming and lemmatization (with POS-aware lemmatization)
- Part-of-speech (POS) tagging
- Simple vectorization (TF-IDF) and inspecting feature names
- Frequency analysis of tokens

## Key Functions / Steps (short)
- `basic_clean(text)` — lowercases and removes URLs/digits/punctuation.
- `tokenize(text)` — splits text into tokens (words).
- `remove_stopwords(tokens)` — filters out common stopwords.
- `stem_tokens(tokens)` and `lemmatize_tokens(tokens)` — reduce tokens to stems/lemmas.
- `preprocess_text(text, method='lemma')` — a wrapper performing the pipeline.
- `TfidfVectorizer(...)` — convert preprocessed docs to TF-IDF features and inspect top words.
