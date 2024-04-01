# Melatonin Product Review Analysis

This project performs a natural language processing (NLP) analysis on Amazon product reviews for melatonin supplements. The analysis includes text preprocessing, feature extraction, sentiment analysis, and machine learning model training for dose prediction based on review text.

## Dataset

The dataset used in this project is a collection of Amazon product reviews for various melatonin supplements. The reviews are stored in multiple CSV files in the folder labeled as `Adult` (indicating the dataset focuses on supplements for adults only), which are combined into a single pandas DataFrame for analysis.

## Setup Instructions

0. **Install required libraries:**
	To install the necessary libraries, run the following command:
	```
	pip install -r requirements.txt
	```
1. **Clone the repository:**
	```
	git clone https://github.com/kumarsandeep567/melatonin-review.git
	```

2.  Run the Jupyter Notebook

## Analysis Steps

The main analysis steps performed in this project are:

1. Data loading and preprocessing
2. Exploratory data analysis and visualization
3. Text preprocessing (stopword removal, stemming, etc.)
4. Feature extraction (TF-IDF vectorization)
5. Sentiment analysis (positive/negative sentiment classification)
6. Machine learning model training (Multinomial Naive Bayes, Logistic Regression)
7. Model evaluation and interpretation

## Results

The analysis provides insights into the customer sentiment towards melatonin products, as well as the relationship between review text and dosage information. The trained machine learning models can be used to predict dosage based on review text, although the current model performance may require further improvement.

## Todo:

1. Performance of both Multinomial NB and Logistic Regression is below expected values (Accuracy: approx 50%). 
2. 
	Possible reasons could be
	- Class imbalance in the `['positive', 'negative']` sentiments
	- Improper hyperparameter tuning which could result in underfitting/overfitting

	Attempt possible solutions (for respective problems)
	- Implement sampling techniques to handle class imbalance
	- Implement Regularization to tune the C parameter
3. Implement other models such as SVM and XGBoost and observe their performance on this dataset