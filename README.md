# 📊 Topic Modeling on BBC News Articles

[![Pandas](https://img.shields.io/badge/-Pandas-150458?logo=pandas)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/-NumPy-4D77CF?logo=numpy)](https://numpy.org/)
[![Scikit-learn](https://img.shields.io/badge/-Scikit--learn-F7931E?logo=scikit-learn)](https://scikit-learn.org/)
[![NLTK](https://img.shields.io/badge/-NLTK-3776AB?logo=python&logoColor=white)](https://www.nltk.org/)
[![Gensim](https://img.shields.io/badge/-Gensim-C1554D)](https://radimrehurek.com/gensim/)
[![pyLDAvis](https://img.shields.io/badge/-pyLDAvis-E8772E)](https://github.com/bmabey/pyLDAvis)
[![Matplotlib](https://img.shields.io/badge/-Matplotlib-11557c)](https://matplotlib.org/)
[![Seaborn](https://img.shields.io/badge/-Seaborn-4c72b0)](https://seaborn.pydata.org/)

## 📝 Project Overview

This project applies Natural Language Processing (NLP) and Topic Modeling techniques to a dataset of news articles from the BBC. Using the **Latent Dirichlet Allocation (LDA)** algorithm, the project analyzes the texts to automatically extract the main underlying topics and themes in an unsupervised manner.

This analysis provides valuable insights into the thematic distribution of the articles and highlights the key terms that define each topic, which is crucial in fields like content organization, trend analysis, and recommendation engines.

-----

## ✨ Key Features

  - **🧹 Advanced Text Preprocessing:** The project includes an integrated pipeline for text data preprocessing, including the removal of punctuation, stopwords, and conversion to lowercase.
  - **📚 Lemmatization:** Utilizes the NLTK library to reduce words to their base or root form, improving the accuracy of topic extraction.
  - **🔢 TF-IDF Vectorization:** Implements the Term Frequency-Inverse Document Frequency (TF-IDF) technique to convert text data into a numerical matrix that reflects the importance of each word in the articles.
  - **🤖 LDA Topic Modeling:** Applies the Latent Dirichlet Allocation algorithm to identify 5 distinct hidden topics within the news article dataset.
  - **📊 Interactive Visualization:** Uses the `pyLDAvis` library to create an interactive dashboard for exploring the discovered topics, their most relevant keywords, and their distribution across the dataset.

-----

## 🛠️ Prerequisites

To run this project successfully, please ensure you have the following requirements installed:

  - **Python:** Version 3.8 or higher.
  - **Core Libraries:**
      - `pandas`
      - `numpy`
      - `scikit-learn`
      - `nltk`
      - `gensim`
      - `pyLDAvis`
      - `matplotlib`
      - `seaborn`
  - **NLTK Data:** The `stopwords`, `punkt`, and `wordnet` packages are required for text preprocessing.

-----

## 🚀 Installation & Setup

Follow these steps to set up your environment and run the project locally:

1.  **Clone the Repository:**

    ```bash
    git clone https://github.com/Zeyad-GenAI/Topic_Modeling_on_BBC_News.git
    cd Topic_Modeling_on_BBC_News
    ```

2.  **Create and Activate a Virtual Environment (Recommended):**

    ```bash
    python -m venv venv
    # For Windows
    venv\Scripts\activate
    # For macOS/Linux
    source venv/bin/activate
    ```

3.  **Install Required Libraries:**
    It is best to create a `requirements.txt` file with the libraries listed above and install them using the following command:

    ```bash
    pip install -r requirements.txt
    ```

4.  **Download Necessary NLTK Data:**
    Run Python and execute the following commands to download the required packages:

    ```python
    import nltk
    nltk.download('stopwords')
    nltk.download('punkt')
    nltk.download('wordnet')
    ```

5.  **Run the Jupyter Notebook:**
    You can now launch the Jupyter Notebook to explore and run the code:

    ```bash
    jupyter notebook topic-modeling-on-bbc-news-articles.ipynb
    ```

-----

## 📖 Usage

The project's usage revolves around running the `topic-modeling-on-bbc-news-articles.ipynb` notebook step-by-step. The notebook begins by loading the data from the `bbc-news-data.csv` file, then moves through the stages of preprocessing, model building, and finally, interactive visualization of the results.

You can modify parameters such as the number of topics (`n_components` in the LDA model) to experiment with different outcomes and explore thematic patterns more deeply.

-----

## 📁 Project Structure

```
bbc-news-topic-modeling/
│
├── data/
│   └── bbc-news-data.csv      # The dataset used in the analysis
│
├── topic-modeling-on-bbc-news-articles.ipynb  # Jupyter Notebook with code and analysis
│
├── requirements.txt           # File containing required libraries
│
└── README.md                  # This file
```

-----

## 🤝 Contributing

Contributions to improve and expand this project are welcome. If you would like to contribute, please follow these steps:

1.  Fork the repository.
2.  Create a new branch for the feature you are working on (`git checkout -b feature/AmazingFeature`).
3.  Implement your changes and improvements.
4.  Commit your changes with clear messages (`git commit -m 'Add some AmazingFeature'`).
5.  Push your changes to your branch (`git push origin feature/AmazingFeature`).
6.  Open a Pull Request.

-----

## 📄 License

This project is licensed under the **MIT License**. You can find the full license details [here](https://opensource.org/licenses/MIT).

-----

## 🙏 Acknowledgments

  - **Dataset:** The project uses a publicly available dataset of BBC News articles.
  - **Libraries:** A special thanks to the developers of the powerful libraries that made this project possible, especially `Scikit-learn`, `NLTK`, `Gensim`, and `pyLDAvis`.
