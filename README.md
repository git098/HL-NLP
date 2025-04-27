# HL-NLP: Sentiment Analysis of News Headlines using H2O and XGBoost

## Overview

This project performs sentiment analysis on news headlines to determine whether a headline expresses a positive, negative, or neutral sentiment. It utilizes the H2O AutoML library for initial model exploration and then employs XGBoost for sentiment prediction.

## Functionality

The project performs the following steps:

1.  **Data Loading and Cleaning:** Loads news headline data from a CSV file (`SEntFiN-v1.1.csv`), removes duplicate entries, and extracts sentiment labels.
2.  **Exploratory Data Analysis (EDA):** Analyzes the distribution of sentiment labels in the dataset.
3.  **Data Preprocessing:**
    *   Applies stemming to reduce words to their root form.
    *   Removes stop words (common words like "the", "a", "is") to focus on important words.
    *   Tokenizes the headlines into individual words.
4.  **Model Training:**
    *   Uses H2O AutoML to automatically train and evaluate various machine learning models.
    *   Selects XGBoost as the best-performing model.
    *   Trains an XGBoost classifier on the processed headline data.
5.  **Sentiment Prediction:** Predicts the sentiment of new news headlines using the trained XGBoost model.

## Installation

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/git098/HL-NLP.git
    cd HL-NLP
    ```

2.  **Install the dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

## Usage

1.  **Download the SEntFiN-v1.1.csv dataset:**

    *   Place the `SEntFiN-v1.1.csv` file in the `/content/drive/MyDrive/Colab Notebooks/` directory (or modify the `path` variable in the notebook to point to the correct location).
2.  **Run the Jupyter Notebook:**

    *   Open `HL_NLP.ipynb` using Jupyter Notebook or JupyterLab.
    *   Run the cells in the notebook to perform sentiment analysis on news headlines.
3.  **Configure H2O:**
    * The notebook uses H2O for AutoML. Ensure H2O is properly initialized.
4.  **Interpret the results:**
    * The notebook outputs a confusion matrix and classification report to evaluate the performance of the XGBoost model.
    * It also includes an example of predicting the sentiment of a new headline.

## Requirements

*   Python 3.6+
*   `pandas`
*   `scikit-learn`
*   `h2o`
*   `nltk`
*   `datatable`
*   `polars`
*   `pyarrow`
*   `xgboost`

## License

This project is licensed under the MIT License - see the `LICENSE` file for details.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes.
