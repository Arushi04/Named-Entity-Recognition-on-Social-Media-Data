# Named-Entity-Recognition-on-Social-Media-Data
Named Entity Recognition (NER) is a sub-task of information extraction that locates and classifies named entities present in unstructured text into predefined categories like person, location, group etc. Recognizing named entities in running text is one of the first tasks in the pipeline of many NLP applications, including machine translation, text summarization, sentiment analysis and  question-answering systems. We aim to perform named entity recognition on social media data. We selected the social media dataset because currently state-of-the-art approaches for NER tasks achieves high performance on clean text but the algorithms’ performance degrades drastically as they move to the noisy datasets like that of social media domains which contains informal text with improper grammatical structure, slang vocabulary, and spelling inconsistencies.

The data has been taken from one of the challenges organized in 2017 by a workshop on Noisy User-generated Text, commonly known as W-NUT. This workshop mainly focuses on NLP applied to noisy user-generated text such as that of social media, online reviews, web forums etc. The dataset is available in CoNLL format (tab separated values), where each line contains a token and its entity class separated by a tab. As the data is coming from unstructured text from different social media platforms, we will process the data by removing entries like url, emojis, tags, numbers and replacing them by a predefined token. We plan to use a baseline model with vocabulary of train and dev set and their mapping to tag the data in the testset. We then plan to use different variations of sequential models (LSTM, Bi-directional LSTM, BiLSTMs with Conditional Random Field) to assess the performance on the test set. 


### Dataset
The dataset consists of annotated files from multiple social media platforms. The training dataset is taken from Twitter, dev dataset from YouTube and test dataset from StackExchange and Reddit. Each line of the data file contains a word and it’s entity mapping separated by a tab. 
We have six entity classes in this dataset: 
1. Person
2. Location (including GPE, facility)
3. Corporation
4. Consumer good (tangible goods, or well-defined services)
5. Creative work (song, movie, book, and so on)
6. Group (subsuming music band, sports team, and non-corporate organisations)

Dataset link: https://noisy-text.github.io/2017/emerging-rare-entities.html
