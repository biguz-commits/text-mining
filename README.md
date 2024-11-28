### README: Named Entity Recognition (NER) and Text Mining Project

---

## **Project Overview**

This repository contains a Named Entity Recognition (NER) and Text Mining project, focusing on analyzing text data from Wikipedia articles. The dataset used in this project has been preprocessed, with each token assigned an IOB (Inside-Outside-Beginning) tag, which is commonly used in computational linguistics for chunking and NER tasks.

The project implements several neural network models, including the transformer-based **BERT**, to extract and classify named entities efficiently.

---

## **Dataset Description**

The dataset consists of Wikipedia articles where tokens are labeled with IOB tags. The following five tags were used:

1. **I-PER**: Person
2. **I-LOC**: Location
3. **I-ORG**: Organization
4. **I-MISC**: Miscellaneous (named entities that don't belong to the above categories)
5. **O**: Outside (not a named entity)

The dataset has been verified to contain no missing values or empty strings, ensuring data quality for further analysis.

---

## **Project Structure**

### **1. Exploratory Data Analysis (EDA)**
- **Data Cleaning**: Ensures the dataset is free of missing values and other inconsistencies.
- **Tag Distribution Analysis**: Visualizes the frequency and distribution of IOB tags across the dataset.
- **Token-Level Insights**: Explores the structure and patterns of tokenized text.

### **2. Named Entity Recognition (NER)**
- **Models Implemented**:
  1. **Feed-Forward Neural Networks (FFNN)**:
     - A basic neural network architecture used as a baseline model for token classification.
  2. **Long Short-Term Memory (LSTM)**:
     - A recurrent neural network (RNN) variant that captures long-term dependencies in sequences for better NER performance.
  3. **Gated Recurrent Units (GRU)**:
     - Another RNN variant, similar to LSTM but with a simplified architecture, used for sequence modeling.
  4. **BERT (Bidirectional Encoder Representations from Transformers)**:
     - A state-of-the-art transformer model that captures contextual relationships between tokens, providing advanced NER capabilities.
- **Evaluation**:
  - Performance metrics such as accuracy, precision, recall, and F1-score were used to measure model effectiveness.
  - Comparison of results between neural architectures to identify the most effective model for the task.

### **3. Data Visualization**
- **Entity Trends**: Visualizes the occurrence of named entities across the dataset.
- **Token Tagging Distribution**: Highlights the balance (or imbalance) in IOB tagging.
- **Model Performance Metrics**: Visualizes and compares precision, recall, and F1-scores across models.

---

## **Key Features**
- End-to-end pipeline for processing text data for NER tasks.
- Implementation of advanced neural network architectures, including transformers (BERT).
- Detailed exploratory data analysis to identify trends in named entities.
- Comprehensive evaluation and comparison of neural network models for NER.

---

## **Dependencies**
The project requires the following Python libraries:
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `tensorflow` (for LSTM, GRU, and BERT models)
- `transformers` (for BERT implementation)
- `scikit-learn` (for evaluation metrics)
- Any additional dependencies are listed in the Jupyter Notebook.

---

## **Usage**
1. Clone the repository:
   ```bash
   git clone <repository-link>
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Open and run the Jupyter Notebook:
   ```bash
   jupyter notebook NER-NLP.ipynb
   ```

---

## **Contributors**
This project was developed by:
- Alessia Marisa Antognini
- Tommaso Biganzoli
- Giovanni Caminiti
- Alex Costa

Feel free to reach out for collaboration or suggestions!

---

## **License**
This project is licensed under the [MIT License](LICENSE).

