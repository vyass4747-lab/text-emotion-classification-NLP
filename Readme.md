# Text Emotion Classification using NLP and Machine Learning

## Overview

This project focuses on **Text Emotion Classification**, a Natural Language Processing (NLP) task that identifies emotions expressed in text.

The project explores text preprocessing, feature extraction, and machine learning classification algorithms to predict emotion labels from textual data. Different feature extraction techniques and classification models are evaluated to compare their performance.

The project is implemented in Python using a Jupyter Notebook.

## Objectives

- Understand and preprocess textual data for NLP tasks.
- Perform exploratory data analysis on an emotion-labelled dataset.
- Convert text into numerical features using Bag of Words and TF-IDF.
- Train machine learning models for emotion classification.
- Compare model performance using accuracy scores.
- Identify the best-performing model among the implemented approaches.

## Technologies Used

- **Python** — Programming language
- **Pandas** — Data manipulation and analysis
- **NumPy** — Numerical computing
- **Matplotlib** — Data visualization
- **Seaborn** — Statistical visualization
- **NLTK** — Natural language processing and text preprocessing
- **Scikit-learn** — Feature extraction, model training, and evaluation
- **Jupyter Notebook** — Interactive development environment

## Dataset

The project uses an emotion-labelled text dataset loaded from `train.txt`.

- **Text:** Input sentence or text sample.
- **Emotion:** Corresponding emotion label.
- **Dataset size:** 16,000 samples.

The dataset is used to explore text preprocessing, feature extraction, and supervised machine learning techniques.

**Note:** The dataset file must be available in the expected location for the notebook to run successfully.

## Project Workflow

### 1. Data Loading and Exploration

- Load the dataset using Pandas.
- Inspect the dataset structure and emotion labels.
- Explore the distribution of emotion categories.

### 2. Text Preprocessing

Prepare the text for machine learning by applying the preprocessing operations implemented in the notebook.

### 3. Feature Extraction

**Bag of Words (BoW)**

Converts text into numerical vectors based on word occurrence counts.

**TF-IDF (Term Frequency–Inverse Document Frequency)**

Converts text into weighted numerical features that reflect the importance of words across the dataset.

### 4. Model Training

The following machine learning approaches are explored:

- Multinomial Naive Bayes with Bag of Words features.
- Multinomial Naive Bayes with TF-IDF features.
- Logistic Regression with TF-IDF features.

### 5. Model Evaluation

The trained models are evaluated using accuracy scores to compare their classification performance.

## Results and Model Comparison

The following accuracy scores were obtained in the notebook:

| Feature Extraction | Classification Model | Accuracy |
|---|---|---:|
| Bag of Words | Multinomial Naive Bayes | 76.81% |
| TF-IDF | Multinomial Naive Bayes | 66.09% |
| TF-IDF | Logistic Regression | **86.15%** |

### Best-Performing Model

**Logistic Regression with TF-IDF achieved 86% accuracy**, making it the best-performing approach among the three reported experiments.

The results demonstrate that the choice of classification algorithm and text representation can significantly influence model performance.

*Note: These are the recorded notebook results. Accuracy alone does not establish generalization performance; evaluation on an appropriate held-out dataset and additional metrics would provide a more complete assessment.*

## Project Structure

```text
text-emotion-classification-nlp/
│
├── Emotion.ipynb
├── Readme.md
├── .gitignore
└── train.txt
```

- `Emotion.ipynb` — Notebook containing the implementation and experiments.
- `Readme.md` — Project documentation.
- `.gitignore` — Specifies files and directories Git should ignore.
- `train.txt` — Dataset used by the notebook.

Include the dataset in the public repository only if its licence permits redistribution.

## Installation and Setup

### Prerequisites

- Python 3.9 or a compatible version
- pip
- Jupyter Notebook

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/text-emotion-classification-nlp.git
cd text-emotion-classification-nlp
```

Replace `YOUR-USERNAME` with your GitHub username.

### 2. Create a virtual environment (recommended)

```bash
python -m venv .venv
```

Activate it on Windows:

```bash
.venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install numpy pandas matplotlib seaborn scikit-learn nltk jupyter
```

If the notebook requires additional NLTK resources, download the resources specified by the preprocessing code.

### 4. Prepare the dataset

Place `train.txt` in the location expected by the notebook. If the notebook uses a relative file path, keeping the dataset in the repository root will generally be appropriate.

### 5. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open `Emotion.ipynb` and execute the cells in order.

## Key Learnings

- Text preprocessing and cleaning for NLP.
- Exploratory analysis of emotion-labelled text.
- Text vectorization using Bag of Words and TF-IDF.
- Training and comparing machine learning classifiers.
- Evaluating classification models using accuracy.
- Understanding how feature extraction affects model performance.

## Future Improvements

- Evaluate models using precision, recall, F1-score, and a confusion matrix.
- Perform hyperparameter tuning to improve model performance.
- Validate performance on a separate, unseen test dataset.
- Analyze incorrectly classified text samples.
- Experiment with additional machine learning and deep learning approaches.
- Explore transformer-based models for more context-aware emotion classification.

## Project Information

**Domain:** Natural Language Processing (NLP)

**Category:** Machine Learning / Text Classification

**Language:** Python

**Environment:** Jupyter Notebook

---

This project demonstrates a practical application of NLP and machine learning for emotion classification, with experiments comparing Bag of Words, TF-IDF, Multinomial Naive Bayes, and Logistic Regression.
