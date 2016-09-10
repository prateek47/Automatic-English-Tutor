# Automatic-English-Tutor
Automatic Proof reading algorithm that can differentiate bad english sentences from good english sentences

Tools and skills used: python, Word2Vec, Language models, Naive Bayes.

## Objective: 
English being a defacto language used everywhere, non-english speakers face a challenge while communicating their work
effectively to their colleages in english and while, human proofreading is not always a option available to everyone, therefore,
we present a deep learning NLP proofreading algorithm that can take in any kind of article, research paper and find grammatically
or contextually bad english sentences and makes appropriate suggestions.

This is a research project aimed for text mining course in spring at University of Virginia.

## Approach: 
  We first trained a 5-gram language model, to get a better sense of context behind the article. We used 3 different 
datasets, Reuters news articles and wikipedia for good english sentences and gachon dataset for bad english dataset. So, 
when the paragraph is inserted the pretrained model learns the paragraph and then uses naive bayes to differentiate bad
from good english sentences.

  After differentiating, we use a pre trained Word2Vec model ( on the same dataset) to ingest the bad english sentences. We 
extended the functionality of word2vec from word prediction to sentence level prediction.

  Our Word2Vec model the projects the sentence in vector space and find sentences of equivalent vector representation to make 
alternative good english sentence level sugestions.

This repository have the code for Word2vec model, while the language model code is present at github.com/juanarrivillaga 
repository.
