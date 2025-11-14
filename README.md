# NLP-Preprocessing_NER_Pronoun_Ambiguity
📌 Project Overview
This repository contains a single Google Colab Notebook that solves both NLP programming tasks:
Q1: Preprocessing text (Tokenization → Stopword Removal → Lemmatization → Keep Only Nouns & Verbs)
Q2: Named Entity Recognition (NER) + Pronoun Ambiguity Detection

✅ Q1 – Text Preprocessing Pipeline (NLTK)
Input sentence:
John enjoys playing football while Mary loves reading books in the library.

✔ Steps implemented:
Tokenization using word_tokenize
Stopword removal using NLTK stopword list
Lemmatization using WordNetLemmatizer
POS tagging using pos_tag
Keeping only nouns & verbs and printing results

✔ Output printed in 4 parts:
Segmented tokens
Tokens after stopword removal
Lemmatized tokens
Final output (nouns + verbs, lemmatized)
Works cleanly in Google Colab with:

import nltk
nltk.download('punkt')
nltk.download('punkt_tab')
nltk.download('averaged_perceptron_tagger')
nltk.download('wordnet')
nltk.download('stopwords')

✅ Q2 – Named Entity Recognition + Pronoun Ambiguity (spaCy)
Input sentence:
Chris met Alex at Apple headquarters in California. He told him about the new iPhone launch.

✔ NER extracts:
PERSON
ORG
GPE

✔ Pronoun Ambiguity Detection:
If the sentence contains pronouns such as:
he, she, they, him, her, them

the code prints:
Warning: Possible pronoun ambiguity detected!

✔ spaCy model used:
en_core_web_sm

🚀 How to Run (Google Colab)

Open the notebook in Google Colab.
Run the setup cell (installs nltk, spacy, and downloads required models).
Run Q1 cell to view all four preprocessing stages.
Run Q2 cell to see NER results + pronoun ambiguity warning.

🧠 Technologies Used

Python 3
Google Colab
NLTK (Tokenization, stopwords, POS tagging, lemmatization)
spaCy (NER, model en_core_web_sm)
