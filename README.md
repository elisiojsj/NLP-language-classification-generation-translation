# NLP language classification, generation and translation models
This is a series of models for NLP (Natural Language Processing).

## Language classification
The objective of this project is to train a simple RNN to on words of different languages and to verify if it learned to identify the style of each language.

## Language generation
In this model we are training a simple RNN on a set of words of different languages for it to understand each one sequence patterns. After trained it's possible to generate words on each of the languages based on the learned patterns.

## Language translation
This is a English - Japanese translation model, the dataset and the code can be adapted for any other pair of languages. As the dataset file was huge we used some filters based on the English sentences. 
To tokenize Japanese words it's necessary to use [mecab-python3](https://pypi.org/project/mecab-python3/) to separate the basic structures as Japanese, contrary to European languages doesn't have space between words.
The translation model uses [LSTMs](https://colah.github.io/posts/2015-08-Understanding-LSTMs/) and [Attention](https://distill.pub/2016/augmented-rnns/)


## Dataset
The data used for language classification and generation was obtained from arcticles in wikipedia on these different languages. 
The articles were cleaned before loading to the model.
All characters were converted to ASCII.

The sentence pairs used for the language translation model were downloaded on [ManyThings.org](https://www.manythings.org/anki/) which arranged files with sentence pairs from the [Tatoeba Project](https://tatoeba.org/eng) 

