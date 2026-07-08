# Yelp Review Classification using NLP

## Project Description

This project applies Natural Language Processing (NLP) techniques to classify Yelp reviews based on their star ratings. The notebook uses the Yelp review dataset to build a text classification model that distinguishes between **1-star** and **5-star** reviews using the Multinomial Naive Bayes algorithm.

The project covers text preprocessing, exploratory data analysis, feature extraction, model training, and evaluation using Scikit-learn.

---

## Dataset

Dataset: `yelp.csv`

Features include:

* `text` – Review text
* `stars` – Rating (1 to 5)

For the classification task, only:

* 1-Star Reviews
* 5-Star Reviews

are used.

---

## Project Workflow

### Data Exploration

The notebook includes:

* Loading the Yelp review dataset
* Viewing the dataset using `head()`
* Dataset information using `info()`
* Statistical summary using `describe()`
* Creating a new feature:

  * `text length`

---

## Exploratory Data Analysis (EDA)

The notebook includes:

* Histogram of review text lengths grouped by star ratings
* Box plot of text length versus star ratings
* Count plot of review ratings
* Correlation matrix of grouped numerical features
* Heatmap for correlation analysis

---

## Data Preparation

The notebook prepares the dataset by:

* Selecting only 1-star and 5-star reviews
* Extracting:

  * Features (`text`)
  * Target (`stars`)
* Splitting the dataset into training and testing sets.

---

## Feature Extraction

The project converts text into numerical features using:

### Bag of Words (BoW)

* `CountVectorizer`

### TF-IDF Transformation

* `TfidfTransformer`

---

## Machine Learning Model

Algorithm:

* Multinomial Naive Bayes

Steps:

1. Convert review text into Bag of Words features.
2. Train the Naive Bayes classifier.
3. Predict review ratings.
4. Evaluate model performance.

---

## NLP Pipeline

The notebook builds a Scikit-learn Pipeline consisting of:

1. CountVectorizer
2. TfidfTransformer
3. Multinomial Naive Bayes

The pipeline is trained on the training dataset and used to predict the test dataset.

---

## Model Evaluation

The model is evaluated using:

* Classification Report
* Confusion Matrix

Both the standalone model and the Pipeline model are evaluated.

---

## Concepts Used

* Natural Language Processing (NLP)
* Text Classification
* Exploratory Data Analysis (EDA)
* Feature Engineering
* Bag of Words (BoW)
* CountVectorizer
* TF-IDF
* TfidfTransformer
* Multinomial Naive Bayes
* Train-Test Split
* Scikit-learn Pipeline
* Classification Report
* Confusion Matrix

---

## Project Structure

```text
Yelp-Review-Classification-using-NLP/
│
├── 02-NLP Project.ipynb
├── yelp.csv
└── README.md
```

---

## Requirements

* Python 3.x
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

## How to Run

1. Clone this repository.
2. Place the `yelp.csv` dataset in the project folder.
3. Open `02-NLP Project.ipynb`.
4. Run all cells from top to bottom.

---

## Author

Meet Tailor — Data Science Learner

GitHub: https://github.com/MeetTailor-Data

---

## License

Created for learning and educational purposes only.
