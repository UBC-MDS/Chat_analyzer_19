# textanalyzer

`TextAnalyzer` includes powerful tools to perform natural language processing on English texts.

`TextAnalyzer` is a Python package designed for performing comprehensive Natural Language Processing (NLP) tasks on English texts. 
This package provides tools for sentiment analysis, keyword extraction, topic modeling, and the detection and visualization of language patterns, making it ideal for text mining and content analysis projects.

## Installation

```bash
$ pip install textanalyzer
```

## Usage

- `analyze_sentiment(message, model="default")`: This function analyzes the sentiment of a given message and prints alert message if it's highly negative. 
- `topic_modeling()`: This function performs topic extraction from a text or a list of texts by using Nonnegative Matrix Factorization. 
- `extract_keywords(messages, method="tfidf", num_keywords=5)`: This function extracts the top keywords from a list of messages using specified methods like TF-IDF or RAKE.
- `detect_language_patterns(messages, method="language", n=2, top_n=5)`: This function detects language patterns such as detected languages, common n-grams, or character usage patterns from a list of messages.
- `visualize_language_patterns(patterns, method="language")`: This function visualizes the detected language patterns using bar charts for language frequency, n-grams, or character patterns.

## Ecosystem Fit

`TextAnalyzer` integrates into the Python NLP ecosystem by offering a simple yet powerful toolkit for analyzing text data. While other Python libraries like [NLTK](https://www.nltk.org/) and [spaCy](https://spacy.io/) provide extensive NLP functionalities, `TextAnalyzer` focuses on making sentiment analysis, keyword extraction, and language pattern visualization more accessible and user-friendly. 

For keyword extraction, packages like [YAKE](https://github.com/LIAAD/yake) and [RAKE-NLTK](https://pypi.org/project/rake-nltk/) provide similar functionality. However, TextAnalyzer combines these tasks into a unified and streamlined workflow.


## Contributing

Interested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.(TO DO - add link)

## Dependencies

- [`TextBlob`](https://textblob.readthedocs.io/): For sentiment analysis.
- [`langdetect`](https://pypi.org/project/langdetect/): For language detection.
- [`scikit-learn`](https://scikit-learn.org/): For keyword extraction and n-gram analysis (`CountVectorizer`).
- [`collections.Counter`](https://docs.python.org/3/library/collections.html): For frequency analysis.


## License

`textanalyzer` was created by Quanhua Huang, Adrian Leung, Anna Nandar, Colombe Tolokin. It is licensed under the terms of the MIT license.

## Credits

`textanalyzer` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).
