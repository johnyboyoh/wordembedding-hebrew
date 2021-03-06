Word Embedding - Hebrew
============================

#### The Code for https://www.oreilly.com/learning/capturing-semantic-meanings-using-deep-learning

##### Note: This code works for Hebrew, but it should work on any other language.

1. Download hebrew dataset from wikipedia
   - Go to: https://dumps.wikimedia.org/hewiki/latest/
   - Download `hewiki-latest-pages-articles.xml.bz2`
2. `pip install --upgrade gensim` (https://radimrehurek.com/gensim/install.html)
3. Run create_corpus.py: `python create_corpus.py`
    - It will create `wiki.he.text`

####  Word2Vec
- Train (inp = "wiki.he.text", out_model = "wiki.he.word2vec.model")

####  FastText
`pip install fasttext`

- Train (inp = "wiki.he.text", out_model = "wiki.he.fasttext.model", alg = "skipgram")

#### Test

Testing specific Hebrew analogies like:

> פריז + גרמניה - צרפת = ברלין

> גבר + מלכה - מלך = אישה

