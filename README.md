Combining both parts into a cohesive README for your Sentiment Analysis project:

---

# Sentiment Analysis Project

This project focuses on analyzing sentiments expressed in text data, specifically using Amazon reviews. The goal is to classify the sentiments as either positive or negative. The project demonstrates the process of reading, cleaning, preprocessing data, conducting exploratory data analysis (EDA), and training a machine learning model for sentiment classification.

## Dataset

The dataset consists of `polarity`, `title`, and `text` columns, where `polarity` indicates the sentiment (1 for negative and 2 for positive sentiments). The dataset can be obtained from Kaggle. For efficiency, only 40,000 rows from both the train and test datasets are used.

## Getting Started

### Installation

1. **Clone the repository** to your local machine:

```bash
git clone https://github.com/PovilasUrb/Sentiment-Analysis.git
```

2. **Download and extract the dataset** from [Kaggle](https://www.kaggle.com/datasets/kritanjalijain/amazon-reviews/data) into the project directory.

3. **Set up a virtual environment** and install the required dependencies:

```bash
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

Your project directory should now look like this:

```
.
├── README.md
├── requirements.txt
├── SentimentAnalysis.ipynb
├── test.csv
├── train.csv
└── venv
```

4. **Download the required NLTK libraries** using the following Python commands:

```python
import nltk
nltk.download('punkt')
nltk.download('stopwords')
```

Alternatively, these commands are included in the `SentimentAnalysis.ipynb` notebook and should execute automatically when you run it.

### Running the Project

Follow these steps to run the project:

1. **Activate your virtual environment** (if you haven't already):

```bash
source venv/bin/activate
```

2. **Run the `SentimentAnalysis.ipynb` notebook**:

Open the notebook in Jupyter Notebook or JupyterLab and execute the cells. The notebook includes steps for data preprocessing, EDA, model training, and sentiment prediction.

Upon completion, the notebook will output two `.joblib` files for the trained TF-IDF vectorizer and the LinearSVC classifier model. These can be used for sentiment prediction in other programs.

---
