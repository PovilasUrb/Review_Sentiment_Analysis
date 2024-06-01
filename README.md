# Sentiment Analysis Project

This project focuses on analyzing sentiments expressed in text data, using Amazon and Yelp reviews. The goal is to classify sentiments as either positive or negative, demonstrating the process of data preprocessing, exploratory data analysis (EDA), and training machine learning models for sentiment classification.

## Datasets

1. **Amazon Reviews**: Contains `polarity`, `title`, and `text` columns. `Polarity` indicates the sentiment (1 for negative and 2 for positive). Dataset: [Amazon Reviews](https://www.kaggle.com/datasets/kritanjalijain/amazon-reviews/data).
2. **Yelp Reviews**: Contains customer reviews from Yelp. Dataset: [Yelp Reviews](https://www.kaggle.com/datasets/ilhamfp31/yelp-review-dataset/data).

## Directory Structure

```
.
├── README.md
├── requirements.txt
├── Amazon_Review_analysis
│   ├── SentimentAnalysis.ipynb
│   ├── train.csv
│   └── test.csv
├── Yelp_Review_analysis
│   ├── yelp
│   │   └── pretrained_model.joblib
│   ├── YelpSentimentAnalysis.ipynb
│   ├── train.csv
│   └── test.csv
└── venv
```

## Getting Started

### Installation

1. **Clone the repository**:

   ```bash
   git clone https://github.com/PovilasUrb/Sentiment-Analysis.git
   ```

2. **Download and extract the datasets** into the appropriate project directories. You may need to alter the paths, since the models were trained in google colab.

3. **Set up a virtual environment** and install the dependencies:

   ```bash
   python -m venv venv
   source venv/bin/activate
   pip install -r requirements.txt
   ```

4. **Download the required NLTK libraries**:

   ```python
   import nltk
   nltk.download('punkt')
   nltk.download('stopwords')
   ```

   Alternatively, these commands are included in the notebooks and should execute automatically.

### Running the Project

1. **Activate the virtual environment**:

   ```bash
   source venv/bin/activate
   ```

2. **Run the Jupyter notebooks**:

   - For Amazon reviews: Open and run `Amazon_Review_analysis/SentimentAnalysis.ipynb`.
   - For Yelp reviews: Open and run `Yelp_Review_analysis/Sentiment_Analysis.ipynb`.

   These notebooks include steps for data preprocessing, EDA, model training, and sentiment prediction.

### Pretrained Models

1. **Yelp** review sentiment analysis includes a pretrained model located in `Yelp_Review_analysis/yelp/model.pth`, which can be used for predicting sentiments of Yelp reviews.
2. **Amazon** review sentiment analysis includes a pretrained model located in `Amazon_Review_analysis/classifier.pth`, which can be used for predicting sentiments of Amazon reviews.

