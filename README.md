# Fake News Detection

This project replicates the analysis conducted by Nathaniel Hoy and Theodora Koulouri in their paper "Exploring the Generalisability of Fake News Detection Models" (2022). It evaluates the generalizability of traditionnal fake news detection models across different feature extraction techniques and datasets.

## Datasets

The datasets used in this project are from Kaggle:

1. [ISOT Fake News dataset](https://www.kaggle.com/datasets/csmalarkodi/isot-fake-news-dataset/) 
2. [Fake or Real News dataset](https://www.kaggle.com/datasets/jillanisofttech/fake-or-real-news)

## Installation

1. Clone the repository
   ```
   git clone https://github.com/lu-julia/fake-news-detection.git
   ```
2. Install the requirements
   ```
   pip install -r requirements.txt
   ```

## Notebooks

| Notebook                  | Description |
|---------------------------|-------------|
| `1-isot.ipynb`            | Performs data loading, preprocessing, feature extraction, and model training on the **ISOT** dataset. All models are evaluated using cross-validation, and trained models are saved for future evaluation. |
| `2-fake_or_real.ipynb`    | Mirrors the workflow of the first notebook but for the **Fake or Real** dataset. It includes feature extraction and model training specific to this dataset. |
| `3-cross_dataset.ipynb`   | Loads the saved models and features from both datasets and performs **cross-dataset evaluation**—testing models trained on one dataset against the other. Results are summarized and visualized to assess model generalizability. |
