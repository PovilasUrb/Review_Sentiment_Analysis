# Sentiment analysis using Amazon reviews

## Step 1:

Download and extract the [dataset](https://www.kaggle.com/datasets/kritanjalijain/amazon-reviews/data) into the current directory.

## Step 2:

Setup virtual environment and install the required dependancies.
```
python -m venv venv
source venv/bin/activate

pip install -r requirements.txt
```

## Step 3:

Run the install the required NLTK libraries using:

```
import nltk

nltk.download('punkt')
nltk.download('stopwords')
```

Alternatively, these commands are included in the notebook file and should download on their own.

## Step 4:

Run the notebook file, SentimentAnalysis.ipynb
