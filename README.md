# Sentiment Analysis of Product Reviews Using NLP and Machine Learning

## Project Overview

This project classifies product reviews into two sentiment categories:

- Positive
- Negative

The project uses Natural Language Processing (NLP) techniques for text preprocessing and machine learning algorithms for sentiment classification.

## Dataset

A public labeled product-review dataset is used.

- Initial reviews selected: **500**
- Positive: **250**
- Negative: **250**
- Duplicate records removed: **2**
- Final dataset: **498 reviews**

## Objectives

- Understand a basic NLP workflow.
- Clean and preprocess review text.
- Perform tokenization.
- Remove stopwords.
- Apply lemmatization.
- Convert text into numerical features using TF-IDF.
- Train different machine learning models.
- Compare model performance.
- Predict the sentiment of new reviews.

## Technologies Used

- Python
- Pandas
- NLTK
- Scikit-learn
- Matplotlib
- Jupyter Notebook
- VS Code

## NLP Techniques Used

### 1. Text Cleaning
Converts text to lowercase and removes unnecessary characters and extra spaces.

### 2. Tokenization
Splits reviews into individual words.

### 3. Stopword Removal
Removes common words that provide limited information for classification while keeping important negative words such as `not`, `no`, and `never`.

### 4. Lemmatization
Converts words into their basic dictionary form.

### 5. TF-IDF
Converts processed text into numerical features for machine learning.

## Machine Learning Models

The project compares:

1. Naive Bayes
2. Logistic Regression
3. Linear SVM

## Results

| Model | Accuracy |
|---|---:|
| Naive Bayes | **74%** |
| Logistic Regression | **77%** |
| Linear SVM | **80%** |

### Best Model

**Linear SVM** achieved the highest accuracy of **80%**.

For the Linear SVM classification report:

- Precision: **0.80**
- Recall: **0.80**
- F1-score: **0.80**

The test set contains **100 reviews**, with 50 Positive and 50 Negative reviews.

## Project Workflow

```text
Review Dataset
      ↓
Data Cleaning
      ↓
Tokenization
      ↓
Stopword Removal
      ↓
Lemmatization
      ↓
Processed Text
      ↓
TF-IDF
      ↓
Train-Test Split
      ↓
Machine Learning Models
      ↓
Model Evaluation
      ↓
Sentiment Prediction
```

## How to Run

Install the required packages:

```bash
pip install -r requirements.txt
```

Open `Sentiment_Analysis_Project_Final_v2.ipynb` in VS Code with the Python and Jupyter extensions installed, then use **Run All**.

## Project Files

```text
Sentiment-Analysis-Project/
├── Sentiment_Analysis_Project_Final_v2.ipynb
├── reviews_dataset.csv
├── reviews_dataset.txt
├── requirements.txt
├── README.md
├── Summer_Internship_Project_Report_Final.docx
└── Summer_Internship_Project_Report_Final.txt
```

## Advantages

- Simple and easy-to-understand NLP pipeline.
- Uses commonly available Python libraries.
- Compares multiple machine learning models.
- Includes standard evaluation metrics.
- Can classify new reviews automatically.

## Limitations

- Only Positive and Negative sentiment classes are used.
- Performance depends on dataset size and quality.
- Traditional machine learning may have difficulty with sarcasm and complex language.

## Future Scope

- Use a larger labeled dataset.
- Add a Neutral sentiment class.
- Experiment with advanced NLP models.
- Build a simple web interface for real-time prediction.

## Learning Outcomes

- Understanding of basic NLP preprocessing.
- Practical use of Python for text analysis.
- Understanding of TF-IDF feature extraction.
- Experience with machine learning classification.
- Understanding of accuracy, precision, recall, and F1-score.
- Experience building an end-to-end NLP project.

## Conclusion

This project demonstrates how NLP preprocessing and traditional machine learning can be combined to classify product reviews. Among the three tested models, Linear SVM performed best with an accuracy of **80%**.
