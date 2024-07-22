# Natural Language Processing - Project

In this project I compare different NLP techniques for two documents. 

## Data Preprocessing
I cleaned and prepared the text data. This includes tokenization, removing stopwords, and applying stemming/lemmatization. These steps help make the text data ready for analysis.

## Feature Extraction
I transformed the text data into numerical representations. I used methods like Bag of Words (BoW), TF-IDF, and word embeddings (Word2Vec, GloVe). These techniques convert text into formats that machine learning models can understand.

## Sentiment Analysis
I analyzed the sentiment of text using different approaches. I started with rule-based methods, then moved on to machine learning models, and finally used deep learning models.

## Topic Modeling
I uncovered hidden themes in a collection of documents. I used LDA and NMF for this. These methods help in identifying the main topics discussed in the text data.

## Text Classification
I categorized text into predefined classes using Naive Bayes, SVM, and deep learning models. Each model has its own advantages depending on the complexity of the text data.

## Named Entity Recognition (NER)
I identified and classified named entities in the text using spaCy and NLTK. SpaCy provides a straightforward API for NER, while NLTK offers more customization options.

## Results
The best method for similarity check is: Enhanced Preprocessed TF-IDF + Cosine Similarity with a result of 0.9802


<img width="363" alt="Screenshot 2024-07-22 at 6 26 43 PM" src="https://github.com/user-attachments/assets/8987b4aa-594a-457e-aa8e-9f3e1813c1cf">




<img width="1103" alt="Screenshot 2024-07-22 at 6 18 19 PM" src="https://github.com/user-attachments/assets/3eaa09d2-c999-43f9-b33d-ed30857883f3">


The enhanced preprocessing steps, including thorough cleaning, tokenization, and lemmatization, ensured that the text data was in its most informative form. This preprocessing step reduces noise and highlights the most important features in the text.

TF-IDF (Term Frequency-Inverse Document Frequency) does not only considers the frequency of terms within a document but also adjusts for the importance of terms across the entire dataset. This helps in emphasizing unique terms that are more relevant for similarity checks.

Cosine similarity measures the cosine of the angle between two vectors, which in this case are the TF-IDF representations of documents. This method is particularly effective for text data as it accounts for the direction of the vectors, thereby providing a robust measure of similarity that is less affected by the document length.

Combining Strengths: By combining enhanced preprocessing with TF-IDF and cosine similarity, this method leverages the strengths of both the preprocessing steps and the feature extraction technique. This results in a more accurate and reliable similarity measurement.

<img width="1029" alt="Screenshot 2024-07-22 at 6 23 25 PM" src="https://github.com/user-attachments/assets/8377d7e5-39e8-41ad-8143-82c2af6b8518">

<img width="1005" alt="Screenshot 2024-07-22 at 6 24 06 PM" src="https://github.com/user-attachments/assets/0d6aa8c5-18ab-4874-ade0-888e4b8fc02e">


Compared to the other methods:

Jaccard Similarity only measures the overlap between sets, which can miss important contextual information.
Bag of Words + Cosine Similarity (Radians) does not account for term importance, making it less effective for capturing the true similarity between texts.
Doc2Vec + Cosine Similarity is a strong method but can be less effective if not properly tuned or if the dataset is small.
