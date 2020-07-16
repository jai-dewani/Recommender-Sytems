# Recommender System
This was our 6th Sem mini project in which we learned about different types of Recommender systems and implemented some of them with the help of different blogs and tutorials. Till now we have implemented two types
- Content Based Filtering 
- Deep Learning 

We also created a algorithm which takes in set of sentences and creates a knowledge graph using them.

You can find the three notebooks in the [Notebooks folder](Notebooks/) or if you want directly run them, use these links
- [Link to Python Notebook containing Content Based Filtering Recommendation Model](https://www.kaggle.com/jaidewani/movie-recommender)

- [Link to Python Notebook containing Deep Learning Recommendation Model and Knowledge Graph](https://colab.research.google.com/drive/18BmT8GlQvKxwOivdIO_JxABRVroIQhl1?usp=sharing)

Both the notebook have the relevant data and steps already in-place to be run as it is except *The Knowledge Graph section*. It has two sections

- Taking raw data and creating well formated data which requires StanforNLP Parsor which we weren't able to install on either notebooks, so one can follow these steps to install it locally and run the code provided locally to create similar results

	Steps to install Stanford Tagger, NER, Tokenizer and Parser:

	- Make sure java is installed (version 1.8+)
	- Download & extract the stanford NER package http://nlp.stanford.edu/software/CRF-NER.shtml
	- Download & extract the stanford POS tagger package http://nlp.stanford.edu/software/tagger.shtml
	- Download & extract the stanford Parser package: http://nlp.stanford.edu/software/lex-parser.shtml
	- Add the directories containing stanford-postagger.jar, stanford-ner.jar and stanford-parser.jar to the CLASSPATH environment variable
	- Point the STANFORD_MODELS environment variable to the directory containing the stanford tokenizer models, stanford pos models, stanford ner models, stanford parser models e.g (arabic.tagger, arabic-train.tagger, chinese-distsim.tagger,stanford-parser-x.x.x-models.jar ...)
	- e.g. export STANFORD_MODELS=/usr/share/stanford-postagger-full-2015-01-30/models:/usr/share/stanford-ner-2015-04-20/classifier
	- Source for the above steps: https://github.com/nltk/nltk/wiki/Installing-Third-Party-Software#stanford-tagger-ner-tokenizer-and-parser

- Taking Processed data and creating results
	
	The triples file contains processed data for reviews of "Batman: The Dark Knight".
	One can upload it to Google colab's file instance to use this data to genrate similar output as presented in our report

TODOs
- Creating a Flask application to use the reccomender system created using Content Based Filtering 
- Create a Collaborative Filtering Fecommender Systems

Contributors: 
- [Jai Kumar Dewani](https://github.com/jai-dewani)
- [Utkarsh Raj Singh](https://github.com/utkarsh-raj)
