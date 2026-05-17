# Spam Message Classification using Machine Learning

This project focuses on detecting spam messages using Machine Learning and Natural Language Processing (NLP) techniques. The text messages are preprocessed and transformed into numerical feature vectors using CountVectorizer before training different classification models.

The project compares the performance of multiple Machine Learning algorithms including:
- Naive Bayes
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)

## Project Workflow

### 1. Data Preprocessing
- Imported and cleaned the spam dataset
- Converted message categories into binary values:
  - Spam → 1
  - Ham (Non-Spam) → 0

### 2. Text Vectorization
Used CountVectorizer with:
- N-grams ranging from 1 to 3
- Minimum document frequency of 5
- Maximum feature size of 8000

This converts text messages into numerical vectors that can be used by Machine Learning models.

### 3. Train-Test Split
The dataset was divided into:
- 80% Training Data
- 20% Testing Data

using:
- random_state = 42

### 4. Model Training
Implemented and compared:
- Gaussian Naive Bayes
- KNN Classifier
- Support Vector Machine (SVM)

## Model Performance

| Model | Training Accuracy | Testing Accuracy |
|-------|-------------------|------------------|
| KNN | 93.60% | 92.91% |
| Naive Bayes | 94.79% | 94.52% |
| SVM | 99.43% | 98.38% |

## Prediction Example

Input Message:
```python
"You won 25 lakh" -> 1(Spam)
