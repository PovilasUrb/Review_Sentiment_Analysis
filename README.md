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
When everything has been setup, it should look like this:
```
.
├── README.md
├── requirements.txt
├── SentimentAnalysis.ipynb
├── test.csv
├── train.csv
└── venv
```

## Step 3:

Download the required NLTK libraries using:

```
import nltk

nltk.download('punkt')
nltk.download('stopwords')
```

Alternatively, these commands are included in the notebook file and should download on their own.

## Step 4:

Run the notebook file, SentimentAnalysis.ipynb

<sub> When the notebook finish, you should be left with 2 joblib files, which you can use in other programs. </sub>
