# NLP-RuleBased-Regex-WordEmbedding

This repository serves as a practical guide to understanding Natural Language Processing (NLP) techniques through a Lab, focusing on rule-based methods, regular expressions (Regex), and word embedding. It consists of two Jupyter notebooks, each dedicated to a specific part of the lab:

## Part 1: Rule-Based NLP and Regex

In this section, a Python code leveraging Regex is provided to generate bills from user-provided text. The objective is to familiarize with rule-based NLP techniques for information extraction. 

The code employs rule-based techniques using regular expressions (regex) and natural language processing (NLP) to extract information from text. The methods used include:

1- Python Regex:
- Utilizes regex patterns to identify quantities, products, and prices in the input text.
- Removes stopwords and unnecessary phrases for efficient text processing.

2- Similarity using Spacy.Matcher:
- Uses SpaCy Matcher to match patterns in text based on similarity.
- Defines patterns to capture quantity, product, and price information.
- Extracts relevant data for generating the bill.

3- Matching Product Names:
- Matches product names based on predefined patterns using regex.
- Identifies products mentioned in the text by comparing with a list of known products.

## Part 2: Word Embedding

This part explores various word embedding techniques, including one-hot encoding, bag of words, TF-IDF, Word2Vec (Skip Gram, CBOW), GloVe, and FastText. The provided Jupyter notebook applies these techniques to data of Hadiths scrapped from various pages of the website https://mawdoo3.com/ The raw data was stored in a MongoDB database, and Natural Language Processing (NLP) techniques were applied to the scraped text here is the link of the repository of the project https://github.com/elmezianech/Hadiths-Scrapper-NLP-Pipeline. For this notebook, the cleaned and tokenized data is utilized, available in the repository.

Additionally, it utilizes the Tsne Algorithm to visualize and evaluate the encoded/vectorized vectors, concluding with insights into the effectiveness of each approach.

### Evaluation of Techniques

- OneHotEncoder: Offers simplicity and interpretability, making it suitable for categorical data without ordinal relationships. However, it may result in high dimensionality when dealing with a large number of unique words.
- CountVectorizer (Bag of Words): Efficient and straightforward, it excels in tasks such as text classification and sentiment analysis. Yet, it overlooks word order and may not capture nuanced semantic relationships.
- TfidfVectorizer: Similar to CountVectorizer, but it accounts for word frequency across the entire corpus, prioritizing informative words. Widely applied in information retrieval and text mining tasks.
- Word2Vec (Skip-gram and CBOW): Generates dense vector representations that preserve semantic meanings, making it invaluable for tasks like semantic similarity, analogy detection, and named entity recognition.
- FastText: Handles words as character n-grams, resulting in enhanced embeddings for less common or out-of-vocabulary terms. Particularly useful in text classification, especially for languages with complex morphology.
- GloVe: An unsupervised algorithm that captures global word-word co-occurrence statistics, emphasizing semantic relationships within the corpus.

### Conclusion

Each technique presents unique strengths and limitations, emphasizing the importance of selecting the right method for the task. While simpler techniques like OneHotEncoder, CountVectorizer, or TfidfVectorizer are efficient for computational tasks, more sophisticated methods like Word2Vec (Skip-gram and CBOW), and FastText excel in capturing semantic nuances. Experimentation with different techniques is recommended to identify the most suitable approach for specific requirements.
