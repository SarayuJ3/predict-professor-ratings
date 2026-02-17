# Predicting Professor Ratings  
**Personal Project | December 2025**

A machine learning project that fine-tunes a BERT transformer model to predict professor ratings from textual student reviews. The model performs sentiment analysis on professor feedback and infers corresponding numeric ratings. [presentation link](https://docs.google.com/presentation/d/1Rso8tbWSLRDUhBD3TvWBi5x16zz6Ib5BocqTE_qrZxA/edit?usp=sharing)
---

## Overview

This project explores how transformer-based NLP models can be used to quantify qualitative feedback. Using approximately 250 student reviews retrieved from a REST API, I trained and optimized a BERT-based classifier to predict professor ratings based solely on written comments.

The final model achieved **70% accuracy** on the evaluation set.

---

## Features

- Fine-tuned **bert-base-uncased** using HuggingFace Transformers  
- Performed **grid search across 18 hyperparameter configurations**  
- Built a full **data ingestion and preprocessing pipeline**  
- Converted free-text reviews into **numeric rating predictions**  
- Pulled review data directly from a **REST API**

---

## Model Details

- **Base Model:** `bert-base-uncased`  
- **Framework:** HuggingFace Transformers + PyTorch  
- **Task:** Text classification (sentiment → rating prediction)  
- **Dataset Size:** ~250 professor reviews

### Training Strategy

- Tokenization using BERT tokenizer  
- Train/validation split  
- Hyperparameter tuning via grid search  

### Hyperparameters Explored

- Learning rate  
- Batch size  
- Number of epochs  
- Weight decay  

---

## Data Pipeline

1. Pulled professor reviews from a REST API  
2. Cleaned and preprocessed text data  
3. Tokenized reviews using BERT tokenizer  
4. Converted textual sentiment into structured training labels  
5. Trained model and evaluated predictions  
6. Output predicted numeric ratings  

---

## Results

- **Final Accuracy:** 70%  
- Demonstrated strong performance despite relatively small dataset size  
- Performance improved through systematic hyperparameter tuning  

---

## Future Improvements

- Increase dataset size to improve generalization  
- Implement cross-validation instead of single train/test split  
- Experiment with cased vs. uncased BERT transformer models  

