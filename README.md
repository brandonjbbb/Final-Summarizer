Final Summarizer

A Python-based text summarization project that processes HTML articles, analyzes sentiment scores, and generates summaries using both token-based and lemma-based approaches. This repository showcases advanced text analysis and summarization techniques leveraging libraries such as TextBlob, spaCy, and BeautifulSoup.

Table of Contents

Features
Installation
Usage
Project Workflow
Results
File Structure
Contributing
License
Features

Extracts and processes text from HTML articles.
Token-based sentiment analysis for summary generation.
Lemma-based sentiment analysis for comparison.
Sentence polarity histogram visualization.
Generates concise and meaningful summaries.
Compares original article sentiment with generated summaries.
Installation

Prerequisites
Python 3.7 or higher
pip package manager
Required Libraries
Install the required Python libraries using:

pip install -r requirements.txt
Example libraries in requirements.txt:

beautifulsoup4
textblob
spacy
matplotlib
nltk
Download NLTK Data
Ensure necessary NLTK corpora are installed:

python3 -m nltk.downloader punkt
python3 -m textblob.download_corpora
Install spaCy Model
Install the English language model for spaCy:

python3 -m spacy download en_core_web_sm
Usage

Prepare the Article:
Save the article HTML using the provided script in scripts/fetch_article.py.
Run the Summarization:
Process the article for sentiment analysis and summaries:
python scripts/summarizer.py
Visualize Results:
The script generates sentiment histograms for both token and lemma scores and prints the summaries in the console.
Project Workflow

HTML Article Processing:
Parse the article HTML with BeautifulSoup to extract text.
Token-Based Sentiment Analysis:
Score sentences using TextBlob token polarity.
Lemma-Based Sentiment Analysis:
Lemmatize sentences with spaCy and analyze sentiment.
Histogram Visualization:
Plot sentence polarity distributions for tokens and lemmas.
Generate Summaries:
Create summaries based on token and lemma cutoff scores.
Polarity Comparison:
Compare article and summary polarity scores.
Results

Token-Based Summary:
Concise and context-preserving summaries focusing on key points.
Lemma-Based Summary:
Abstracted summaries with emphasis on core ideas.
Histograms:
Visualizations showing sentiment polarity distribution for sentences.
File Structure

Final-Summarizer/
├── output/
│   ├── article.html           # Extracted HTML article
├── scripts/
│   ├── fetch_article.py       # Script to fetch article HTML
│   ├── summarizer.py          # Main summarization script
├── requirements.txt           # List of required libraries
├── README.md                  # Project README
Contributing

Contributions are welcome! To contribute:

Fork the repository.
Create a feature branch (git checkout -b feature-name).
Commit your changes (git commit -m 'Add feature-name').
Push to the branch (git push origin feature-name).
Create a pull request.
License

This project is licensed under the MIT License.
