# Football Player Sentiment Analysis (Reddit + PDFs)

## Overview
End-to-end project that collects football-player related text (mainly Reddit posts, plus PDF-derived text), cleans it, and performs sentiment analysis and ML experiments related to players.

## Pipeline (Notebooks)
1. `01_data_collection.ipynb`
   - Scrapes Reddit posts about specific football players
   - Extracts text from PDFs (including OCR when needed)
   - (Optional) Audio-to-text if audio sources are used
   - Saves intermediate text/CSV outputs

2. `02_pdf_text_cleaning.ipynb`
   - Cleans and normalizes extracted PDF text
   - Produces cleaner text for downstream analysis

3. `03_models_and_sentiment.ipynb`
   - Compares ML models on FIFA player datasets (ratings/value tasks)
   - Runs sentiment analysis on Reddit posts about players
   - Visualizes sentiment trends and distributions
   - Includes a "harsh vs not harsh" text classification experiment

## Data Sources
- Reddit (via PRAW / scraping)
- PDFs (text extraction and OCR where required)
- FIFA player dataset (CSV)

## Tools & Libraries
Python, pandas, numpy, scikit-learn, nltk, matplotlib, seaborn, wordcloud,
praw, bs4, requests, pdfminer, pdf2image, pytesseract, pydub, speech_recognition, spacy.

## Notes
- Raw datasets (large PDFs/audio/scraped dumps) are not included in this repo.
- Configure API keys/secrets locally (do not upload them).
