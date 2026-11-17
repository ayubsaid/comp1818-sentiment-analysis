# comp1818-sentiment-analysis
# How to run
1. Open `sentiment_coursework.ipynb` in Google Colab.
2. Runtime -> Restart session and run all (CPU is enough, about 25-40 minutes).
3. The notebook saves figures and tables to an `outputs/` folder in Colab.

# Files
- `sentiment_coursework.ipynb`: full pipeline with results
- `*.pdf` and `*.csv` in this folder: copies of the figures and result tables from the final run

Thanks for testing my work, enjoy your time!

## Data (downloaded automatically)
- IMDb: huggingface.co/datasets/stanfordnlp/imdb
- Yelp polarity: huggingface.co/datasets/fancyzhx/yelp_polarity

## Trained models
`trained_models.joblib` holds the trained TF-IDF vectoriser, logistic regression,
hybrid models and chosen settings. Load it with
`models = joblib.load("trained_models.joblib")`. It was saved with
scikit-learn 1.6.1; the notebook can retrain everything from scratch.
