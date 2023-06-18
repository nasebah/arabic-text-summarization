# arabic-text-summarization 📚
[![PyPI pyversions](https://img.shields.io/pypi/pyversions/tner.svg)](https://pypi.python.org/pypi/tner/)

For this task the following is used:
1. for preprossing: NLTK library
2. for text summarization two different strategies used:
   - Frequency Method
   - Transformers

the data i used are Wikipedia articles one for [Modern Standard Arabic(MSA)](https://ar.wikipedia.org/wiki/لهجة_مصرية) and the other in [Egyptian Arabic (dialect)](https://arz.wikipedia.org/wiki/اللغه_المصريه_الحديثه)

Here is what the input data (MSA) looks like:
![alt text](images/mbart_input_MSA.png)


And here is  the input data  for Egyptian Arabic:
![alt text](images/mbart_input_MSA.png)




1. NLTK library


2. Text Summarization

 - Text Summarization Using the Frequency Method
   In this method we find the frequency of all the words in our text data and store the text data and its frequency in a dictionary. After that, we tokenize our text data. The sentences which contain more high frequency words will be kept in our final summary data.

Here is the output of the Summarization of MSA Wikipedia Page. It is a 100 words summary:


[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/googlecolab/colabtools/blob/master/notebooks/colab-github-demo.ipynb)

 - Text Summarization Using Hugging Face Transformers
I used the HuggingFace transformers library. The Transformers library provides thousands of pre-trained models to perform tasks such as text summarization. the two pre-trained models that i try and worked are the following:

1. [Albert](https://huggingface.co/albert-base-v2) ⭐️: 

Summarization Output:


[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/googlecolab/colabtools/blob/master/notebooks/colab-github-demo.ipynb)

2. [mBART-50](https://huggingface.co/facebook/mbart-large-50) ⭐️: 

Summarization Output:

![alt text](images/mbart_output_msa.png)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1odB49lxv9dqipToxO4ww6eTqqCTv18eG?usp=sharing)



