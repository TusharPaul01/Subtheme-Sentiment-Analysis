**Methodology & Explanation :**

Keyword Extraction using KeyBERT:
● Utilised the KeyBERT library to extract key themes or keywords from a given sentence.
● Configured the model with parameters such as top_n for the number of keywords, and
keyphrase_ngram_range to determine the number of keywords in each sub-theme.
Sentiment Analysis Model Setup:
● Loaded the sentiment analysis model and tokenizer using the AutoTokenizer and
TFAutoModelForSequenceClassification from the transformers library.
● Specifically used the 'nlptown/bert-base-multilingual-uncased-sentiment' model.
Sentiment Analysis Pipeline:
● Created a sentiment analysis pipeline using the loaded model and tokenizer.
● Iterated through each extracted keyword from the KeyBERT results.
Sentiment Labelling and Scoring:
● Predicted sentiment labels and scores for each keyword using the sentiment analysis
pipeline.
● Mapped sentiment labels to binary categories: "Positive" or "Negative" based on the
provided star ratings.
Storage and Visualization:
● Stored sentiment labels and scores in lists (sentiment_labels and sentiment_scores).
● Utilised the lists for further analysis or visualisation.
Analysis and Visualization:
● Used matplotlib and seaborn for data visualisation.
● Plotted a bar chart to visualise the sentiment analysis results for each keyword, indicating
whether the sentiment is positive or negative.
_Final Output:_
● Displayed the subthemes/ keywords & its sentiment, to check whether it is positive or
negative. (as mentioned in the task)
● Displayed the bar chart for sentiment analysis of keywords to aid in understanding the
overall sentiment associated with the extracted themes.

**My Approach :**
The approach I've implemented requires minimal computational power and delivers output
with minimal latency. It involves utilising both the KeyBERT and BERT models to achieve
effective results.

_Why the KeyBERT model ?_
KeyBERT is an open-source Python library for keyword extraction that leverages the power
of transformer models like BERT. It helps you automatically identify the most relevant
keywords and phrases within a text document.

Functionality:
● Extracts keywords and keyphrases: KeyBERT analyzes your text and extracts the
most important and informative words and phrases that capture the document's
essence.

● Uses transformer models: It relies on powerful transformer models like BERT to
understand the context and relationships between words in the document, leading to
more accurate keyword extraction.
● Flexible: It supports various embedding models like Sentence-Transformers, Flair,
Spacy, and Gensim, allowing you to customize the extraction process.
Benefits:
● Improved information retrieval: By identifying key terms, KeyBERT helps users
find relevant information within documents more efficiently.
● Enhanced text summarization: Extracted keywords can be used to create concise
and informative summaries of longer documents.

_Why BERT model ?_
BERT, which stands for Bidirectional Encoder Representations from Transformers, is a
natural language processing (NLP) model developed by Google. It belongs to the
Transformer architecture family and is pre-trained on large amounts of textual data to
understand the contextual relationships between words in a sentence.
BERT has been widely used in various NLP tasks, including sentiment analysis. Sentiment
analysis is the process of determining the sentiment or emotional tone expressed in a piece of
text, whether it's positive, negative, or neutral.
BERT model is then used for sentiment analysis by classifying the sentiment of a given text.
The model outputs probabilities for each sentiment class, and the class with the highest
probability is considered the predicted sentiment.
