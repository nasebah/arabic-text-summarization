# arabic-text-summarization 📚
[![PyPI pyversions](https://img.shields.io/pypi/pyversions/tner.svg)](https://pypi.python.org/pypi/tner/)

For this task the following is used:
1. for preprossing: NLTK library
2. for text summarization two different strategies used:
   - FREQUENCY METHOD
   - Transformers

the data i used are Wikipedia articles one for [Modern Standard Arabic(MSA)](https://ar.wikipedia.org/wiki/لهجة_مصرية) and the other in [Egyptian Arabic (dialect)](https://arz.wikipedia.org/wiki/اللغه_المصريه_الحديثه)

input MSA:

input Egyptian Arabic:



1. NLTK librarye


2. TEXT SUMMARIZATION

 - TEXT SUMMARIZATION USING THE FREQUENCY METHOD
   In this method we find the frequency of all the words in our text data and store the text data and its frequency in a dictionary. After that, we tokenize our text data. The sentences which contain more high frequency words will be kept in our final summary data.

Summarization Output:


[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/googlecolab/colabtools/blob/master/notebooks/colab-github-demo.ipynb)

 - TEXT SUMMARIZATION USING Hugging Face Transformers
I used the HuggingFace transformers library. The Transformers library provides thousands of pre-trained models to perform tasks such as text summarization. the two pre-trained models that i try and worked are the following:

1. [Albert](https://huggingface.co/albert-base-v2) ⭐️: 

Summarization Output


[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/googlecolab/colabtools/blob/master/notebooks/colab-github-demo.ipynb)

2. [mBART-50](https://huggingface.co/facebook/mbart-large-50) ⭐️: 

Summarization Output


[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/googlecolab/colabtools/blob/master/notebooks/colab-github-demo.ipynb)



