# fashion-sentiment-analysis
# E-Commerce Customer Review Sentiment Analysis

## Project Overview

This project focuses on analyzing customer reviews from an e-commerce clothing platform and classifying them into three sentiment categories: **Positive, Neutral, and Negative**.

The goal is to understand customer opinions, identify sentiment patterns, and extract meaningful insights from textual customer feedback using Natural Language Processing (NLP) and Machine Learning.

## Dataset

- **Dataset:** Women's E-Commerce Clothing Reviews
- **Source:** [Hugging Face Datasets](https://huggingface.co/datasets/chibifire/kaggle-womens-ecom-clothing-reviews)
- Contains customer reviews and associated product ratings.

## Technologies Used

- Python
- Pandas & NumPy
- Scikit-learn
- Matplotlib & Seaborn
- NLP
- TF-IDF Vectorization
- Support Vector Machine (SVM)

## Project Workflow

1. **Data Loading:** Loaded the e-commerce customer reviews dataset.
2. **Data Preprocessing:** Cleaned and prepared textual review data.
3. **Exploratory Data Analysis:** Examined sentiment distribution and review patterns.
4. **Feature Extraction:** Applied TF-IDF to convert textual reviews into numerical features.
5. **Model Training:** Trained a Support Vector Machine (SVM) classifier.
6. **Hyperparameter Tuning:** Optimized model parameters to improve classification performance.
7. **Model Evaluation:** Evaluated performance using accuracy, precision, recall, and F1-score.

## Model Performance

The tuned SVM model achieved the following results:

| Metric         |  Score |
| -------------- | -----: |
| Accuracy       | 82.89% |
| Macro F1-Score | 0.6354 |

The project also highlights the challenges of classifying minority sentiment categories, particularly Neutral and Negative reviews, due to class imbalance.

## Saved Model

The trained model pipeline is saved as:

`sentiment_pipeline.pkl`

The saved pipeline can be reused for sentiment prediction without repeating the entire training process.

## Repository Structure

```text
ecommerce-sentiment-analysis/
│
├── sentiment_analysis.ipynb
├── sentiment_pipeline.pkl
├── requirements.txt
└── README.md
```

## Installation

Clone the repository:

```bash
git clone https://github.com/Reenadewangan/ecommerce-sentiment-analysis.git
```

Navigate to the project directory:

```bash
cd ecommerce-sentiment-analysis
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## Future Improvements

- Improve classification of minority sentiment categories.
- Experiment with advanced NLP techniques.
- Deploy the trained model using Streamlit.
- Develop an interactive sentiment analysis dashboard.

## Conclusion

This project demonstrates how NLP and machine learning can be applied to customer feedback analysis. It provides a foundation for understanding customer sentiment and generating insights that can support data-driven business decisions.
