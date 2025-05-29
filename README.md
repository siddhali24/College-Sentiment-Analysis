# College-Sentiment-Analysis
Sentiment Analysis based on College reviews using ML models and Django 

**ABOUT THE PROJECT:**
Education is a crucial decision, and choosing the right college shapes a student’s future. With countless options, students and parents rely on online reviews, but manually analyzing them is time-consuming. A Sentiment Analysis model can automate this process by analyzing reviews and categorizing them as positive ,negative or neutral, helping students get a quick and clear understanding of a college’s reputation

The project aims to develop a Machine Learning-based Sentiment Analysis model that can:

1. Accept the name of a college and review as input from users. Classify the sentiment of these reviews as positive, negative or neutral and give as output.

2. Accept the name of a college as input from users and give the college status based on reviews as positive, negative or neutral.
   
Technologies used
For ML model: BERT [since based on NLP]
For Webapp: HTML,CSS,Django,Python

**Run on your local machine by:**
git clone https://github.com/siddhali24/College-Sentiment-Analysis.git

python manage.py runserver

then go to port http://127.0.0.1:8000/ to run the local server

# How to Set Up Model Files
The machine learning model files (Naive Bayes or BERT) are **not included in the main repo** due to size limits.
They are available for download from the **Releases** page of this repository:

👉 [Download Model Files from Releases]https://github.com/siddhali24/College-Sentiment-Analysis.git/releases/

## After Downloading

1. Extract the downloaded `.zip`.

2. **Place the files as follows:**

  sentiment/analysis/ml_model/bert_model/
  
  also
  
  ml_model/balanced_reviews(1).csv

  ensure bert_model folder has following: 
  * `config.json`
  * `model.safetensors`
  * `special_tokens_map.json`
  * `tokenizer_config.json`
  * `vocab.txt`

## Important Notes

* Make sure the files are placed exactly in the above folders, as the code depends on these paths.
* If you change folder names, update the paths in your Django views accordingly.
* After placing the files, run your Django server as usual.

