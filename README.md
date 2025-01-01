
# Twitter Sentiment Analysis

This project performs sentiment analysis on Twitter data, classifying tweets as positive, negative, or neutral. It uses machine learning and natural language processing (NLP) techniques to extract insights from social media data.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Dataset](#dataset)
- [Models Used](#models-used)
- [File Structure](#file-structure)
- [Usage](#usage)
- [Results](#results)
- [Contributions](#contributions)
- [License](#license)

## Introduction

Twitter Sentiment Analysis is a powerful tool for understanding public opinion on various topics. This project aims to classify tweets into sentiment categories using different machine learning models and feature extraction techniques.

## Features

- Preprocessing raw Twitter data (e.g., removing special characters, URLs, and stopwords).
- Feature extraction using Bag-of-Words (BoW) and Word2Vec.
- Machine learning models: Support Vector Machine (SVM), Random Forest (RF), and XGBoost.
- Performance comparison of models.
- Visualizing sentiment distributions.

## Dataset

The project uses the following datasets:
- **Training Data:** `Data/train_E6oV3lV.csv`
- **Testing Data:** `Data/test_tweets_anuFYb8.csv`

### Preprocessed Features
- BoW-based features (`Data/sub_rf_bow.csv` and `Data/sub_svm_bow.csv`).
- Word2Vec fine-tuned features (`Data/sub_xgb_w2v_finetuned.csv`).

## Models Used

1. **Random Forest (RF):**
   - Used for classification with Bag-of-Words features.
   
2. **Support Vector Machine (SVM):**
   - Known for its effectiveness in text classification tasks.
   
3. **XGBoost:**
   - Fine-tuned for performance with Word2Vec embeddings.

## File Structure

```
Twitter_Sentiment_Analysis/
├── Data/
│   ├── blob.jpg                     # Sample visual content
│   ├── sub_rf_bow.csv               # RF-based features
│   ├── sub_svm_bow.csv              # SVM-based features
│   ├── sub_xgb_w2v_finetuned.csv    # XGBoost features
│   ├── test_tweets_anuFYb8.csv      # Test data
│   ├── train_E6oV3lV.csv            # Training data
├── Twitter_Sentiment_Analysis.ipynb # Main Jupyter Notebook
```

## Usage

1. **Clone the repository**
   ```bash
   git clone https://github.com/mtechbro94/Twitter_Sentiment_Analysis.git
   cd Twitter_Sentiment_Analysis
   ```

2. **Install dependencies**
   Ensure you have Python installed. Install required libraries:
   ```bash
   pip install pandas numpy scikit-learn xgboost
   ```

3. **Run the notebook**
   Open the `Twitter_Sentiment_Analysis.ipynb` file in Jupyter Notebook or a compatible environment and execute the cells step by step.

## Results

| Model          | Accuracy (%) | Precision (%) | Recall (%) |
|----------------|-------------|---------------|------------|
| Random Forest  | 85.3        | 84.1          | 86.7       |
| SVM            | 87.2        | 86.8          | 87.5       |
| XGBoost (W2V)  | 89.1        | 88.7          | 89.3       |

*Note:* Results may vary depending on the dataset and hyperparameters.

## Contributions

Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add feature-name"
   ```
4. Push to the branch:
   ```bash
   git push origin feature-name
   ```


