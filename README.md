# Fashion Sentiment Analysis

## E-Commerce Customer Review Sentiment Analysis

## Project Overview

This project focuses on analyzing customer reviews from an e-commerce clothing platform and classifying them into three sentiment categories: **Positive, Neutral, and Negative**.

The objective is to understand customer opinions, identify sentiment patterns, evaluate product performance, and extract meaningful business insights using Natural Language Processing (NLP) and Machine Learning.

## Dataset

- **Dataset:** Women's E-Commerce Clothing Reviews
- **Source:** [Hugging Face Datasets](https://huggingface.co/datasets/chibifire/kaggle-womens-ecom-clothing-reviews)
- Contains customer reviews, product information, ratings, and recommendation indicators.

## Technologies Used

- Python
- Pandas & NumPy
- Scikit-learn
- Matplotlib & Seaborn
- Natural Language Processing (NLP)
- TF-IDF Vectorization
- Support Vector Machine (SVM)

## Project Workflow

1. **Data Loading:** Loaded the customer reviews dataset.
2. **Data Cleaning:** Handled missing values and prepared the review data.
3. **Exploratory Data Analysis:** Analyzed sentiment distribution, ratings, and customer review patterns.
4. **Text Preprocessing:** Cleaned and prepared textual reviews for NLP.
5. **Feature Extraction:** Applied TF-IDF vectorization to convert text into numerical features.
6. **Model Training:** Trained and compared multiple machine learning classifiers.
7. **Hyperparameter Tuning:** Optimized the SVM model.
8. **Model Evaluation:** Evaluated performance using accuracy, precision, recall, and F1-score.
9. **Sentiment Prediction:** Classified customer reviews into sentiment categories.
10. **Business Analysis:** Analyzed product recommendations, category performance, and customer complaints.

## Model Performance

The tuned SVM model achieved the following results:

| Metric | Score |
|---|---:|
| Accuracy | 82.89% |
| Macro F1-Score | 0.6354 |

The results highlight the challenges of classifying minority sentiment categories, particularly Neutral and Negative reviews, due to class imbalance.

## Business Analysis & Insights

The project explores customer recommendation patterns and product performance across different dimensions.

Key findings:

- **Sentiment Distribution:** Positive reviews dominate the dataset.
- **Recommendation Patterns:** Positive reviews have a substantially higher recommendation rate than Neutral and Negative reviews.
- **Department Analysis:** Bottoms recorded the highest recommendation rate at 84.95%.
- **Category Analysis:** Lounge recorded the highest recommendation rate at 85.80%, while Trend had the lowest at 74.58%.
- **Age Group Analysis:** Customers aged 50–60 and 60+ showed recommendation rates of 83.69% and 85.19%, respectively.
- **Customer Complaints:** Complaint patterns were analyzed to identify categories requiring further attention.

## Repository Structure

```text
fashion-sentiment-analysis/
│
├── README.md
├── sentiment_analysis.ipynb
├── sentiment_pipeline.pkl
├── requirements.txt
│
└── outputs/
    ├── category_performance_analysis.csv
    ├── customer_complaint_summary.csv
    └── category_complaint_analysis.csv
```

## Saved Model

The trained machine learning pipeline is saved as:

`sentiment_pipeline.pkl`

It can be reused for sentiment prediction without repeating the entire model training process.

## Installation

Clone the repository:

```bash
git clone https://github.com/Reenadewangan/ecommerce-sentiment-analysis.git
```

Navigate to the project directory:

```bash
cd ecommerce-sentiment-analysis
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

## Future Improvements

- Improve classification of minority sentiment categories.
- Experiment with advanced NLP techniques.
- Deploy the sentiment classification model using Streamlit.
- Develop an interactive sentiment analysis dashboard.

## Conclusion

This project demonstrates how NLP and Machine Learning can be applied to customer feedback analysis. By combining sentiment classification with recommendation and complaint analysis, it provides insights into customer preferences and product performance that can support data-driven business decisions.





