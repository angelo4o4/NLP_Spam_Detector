## Overview

This project implements a spam detection system based on the textual **content** of emails, using the ***Email Spam Classification Dataset***, available from Kaggle: [Link to Dataset](https://www.kaggle.com/datasets/balaka18/email-spam-classification-dataset-csv).

- The dataset is based on the frequency of the most common words in the 5172 emails, pre-processed into a bag-of-words format (~3000 features).


- Since no information about the provenance is provided, the task focuses exclusively on **word occurrence features**.


- The final implementation achieves an F1-score of 96.4% on the test set, demonstrating its effectiveness.


## Methodology

For this binary classification task I compared the performance of three models:
- **Naive Bayes (MultinomialNB)**
- Simple **Feed Forward NN (single layer)**
- Custom **Multilayer Perceptron (MLP)**

Additional techniques used:
- **Grid Search** for hyperparameter tuning (MLP)
- **PCA** for data visualization
- **F1-score** as main evaluation metrics (unbalanced data)
- **Permutation Importance** of features

An experiment was also set up to evaluate the impact of removing English stopwords.

## Setup & Libraries
Libraries used are listed in the notebook, to install all the dependencies run the following command:
```bash
pip install -r requirements.txt
