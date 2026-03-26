# Fake News Detection Project

## Overview
This project develops machine learning models to classify news articles as either **reliable** or **fake/unreliable**. It explores a baseline Logistic Regression model using a Bag-of-Words approach and an advanced Linear Support Vector Machine (SVM) using TF-IDF features. The models are trained on the FakeNewsCorpus and evaluated for cross-domain generalization using the LIAR dataset.

## Requirements and Dependencies
To run the Jupyter Notebook, you will need Python 3 installed along with the following libraries:
- `pandas`
- `numpy`
- `nltk`
- `scikit-learn`
- `matplotlib`
- `seaborn`

*Note: The notebook includes code to automatically download the necessary NLTK data (`punkt`, `punkt_tab`, and `stopwords`) on its first run.*

## Data Setup and Folder Structure
Due to size constraints (especially the 995K subset), the datasets are **not** included in this repository. To reproduce the results, you must download the datasets and place them in specific folders relative to the Jupyter Notebook.

Please ensure your directory looks exactly like this before running the code:

```text
├── Fake_News_Project.ipynb      # The main Jupyter Notebook
├── README.md                    # This file
├── data/                        # Create this folder!
│   ├── news_sample.csv          # Download from the FakeNewsCorpus GitHub
│   └── 995,000_rows.csv         # Download from the course Absalon page
└── liar_dataset/                # Create this folder!
    ├── README                   
    ├── test.tsv                 # Used in the notebook for evaluation
    ├── train.tsv                
    └── valid.tsv
