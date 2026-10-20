# Text Emotion Classification using NLP

## Overview

This project focuses on **Text Emotion Classification**, a Natural Language Processing (NLP) task that identifies the emotion expressed in a piece of text.

Using text preprocessing, feature extraction techniques, and machine learning algorithms, the project explores how textual data can be converted into numerical features and classified into different emotion categories.

The project is implemented in Python using a Jupyter Notebook.

## Objectives

- Understand and preprocess textual data for NLP tasks.
- Explore and analyze an emotion-labelled text dataset.
- Convert text into numerical representations using Bag of Words and TF-IDF.
- Train and evaluate machine learning classification models.
- Compare model performance using accuracy scores.

## Technologies Used

- **Python** — Core programming language
- **Pandas** — Data manipulation and analysis
- **NumPy** — Numerical operations
- **Matplotlib & Seaborn** — Data visualization
- **NLTK** — Natural language processing and text preprocessing
- **Scikit-learn** — Feature extraction, model training, and evaluation
- **Jupyter Notebook** — Interactive development environment

## Machine Learning Techniques

### 1. Text Preprocessing
Cleaning and preparing text data for machine learning.

### 2. Bag of Words (BoW)
Converts text into numerical features based on word occurrence counts.

### 3. TF-IDF
Represents text using Term Frequency–Inverse Document Frequency to assign weights to words.

### 4. Multinomial Naive Bayes
A probabilistic classifier trained on text features to predict emotion labels.

### 5. Logistic Regression
An additional classification algorithm explored using TF-IDF features.

## Dataset

The notebook loads a text dataset from a file named `train.txt`.

- **Text:** Input sentence or text sample.
- **Emotion:** Corresponding emotion label.
- **Dataset size:** 16,000 samples.

The dataset file is required to run the notebook from start to finish.

## Model Evaluation

The notebook includes the following recorded results:

| Feature Extraction | Classification Model | Accuracy |
|---|---|---:|
| Bag of Words | Multinomial Naive Bayes | 76.81% |
| TF-IDF | Multinomial Naive Bayes | 66.09% |

These values are the recorded notebook results and may vary when the notebook is rerun with different data or configurations.

Logistic Regression is also explored in the notebook.

## Project Structure

```text
Text-Emotion-Classification/
│
├── finalproject.ipynb
├── train.txt
└── README.md
```

`train.txt` is the dataset file expected by the notebook. Include it in the repository only if its licence permits redistribution.

## Installation and Setup

### Prerequisites

- Python 3.9 or a compatible Python version
- Jupyter Notebook
- pip

### 1. Clone the repository

```bash
git clone <your-repository-url>
cd <your-repository-folder>
```

### 2. Create a virtual environment (recommended)

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install numpy pandas matplotlib seaborn scikit-learn nltk jupyter
```

If the notebook uses NLTK resources, download any required corpora or tokenizers specified by its preprocessing code.

### 4. Add the dataset

Place `train.txt` in the same directory as `finalproject.ipynb`, preserving the expected file name and format.

### 5. Run the notebook

```bash
jupyter notebook
```

Open `finalproject.ipynb` and execute the cells in order.

## Key Learnings

- Text cleaning and preprocessing
- Exploratory data analysis
- Text vectorization using BoW and TF-IDF
- Training machine learning classifiers
- Evaluating and comparing classification accuracy

## Future Improvements

- Compare additional machine learning algorithms.
- Evaluate models using precision, recall, F1-score, and a confusion matrix.
- Improve preprocessing and experiment with different text representations.
- Tune model hyperparameters and investigate classification errors.
- Explore deep learning and transformer-based NLP models.

## Project Type

Machine Learning | Natural Language Processing | Text Classification

---

**Note:** This is a learning project focused on exploring NLP and machine learning techniques. The reported accuracy reflects the experiments documented in the notebook, not a guarantee of performance on unseen real-world text.
