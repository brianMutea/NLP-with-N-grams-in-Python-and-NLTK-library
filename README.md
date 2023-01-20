# NLP-with-N-grams-in-Python-and-NLTK-library

N-grams, therefore, are a type of statistical language model used in Natural Language Processing (NLP) to predict the possibility 
of a sequence of words. An n-gram is a contiguous series of n items from a given text sample where "n" is the number of items in the sequence.

# Classification of n-grams
We have several classifications of n-grams, depending on the number that n represents. The most commonly used n-grams are:

* An n-gram of size 2, N = 1, is a unigram
* An n-gram of size 2, N = 2, is a bigram.
* An n-gram of size 3, N = 3, is a trigram.

An n-gram can be of any length, N, and different types of n-grams are suitable for different applications.

We can quickly and easily generate n-grams with the ngrams function available in the `nltk.util module`. 

Use the following sentence for instance:

"Natural Language Processing using N-grams is incredibly awesome."

## Code

```from nltk.util import ngrams 

def generate_n_grams(text, ngram=1):
    unigrams = ngrams(sentence.split(), n)
    for item in unigrams:
        return item

text = "Natural Language Processing using N-grams is incredibly awesome."```

Generate bigrams Set the ngram parameter value to 2, 
    change this value for trigrams and so on

generate_n_grams(text, 2) 

Results:
```('Natural', 'Language')
('Language', 'Processing')
('Processing', 'using')
('using', 'N-grams')
('N-grams', 'is')
('is', 'incredibly')
('incredibly', 'awesome.') ```


See full notebook
