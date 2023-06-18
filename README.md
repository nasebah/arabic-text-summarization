# arabic-text-summarization 📚
[![PyPI pyversions](https://img.shields.io/pypi/pyversions/tner.svg)](https://pypi.python.org/pypi/tner/)

For this task the following is used:
1. for text preprossing: NLTK library
2. for text summarization two different strategies used:
   - Frequency Method
   - Transformers

The data that I used are two Wikipedia articles one for [Modern Standard Arabic(MSA)](https://ar.wikipedia.org/wiki/لهجة_مصرية) and the other in [Egyptian Arabic (dialect)](https://arz.wikipedia.org/wiki/اللغه_المصريه_الحديثه)

Here is what the input data (MSA) looks like:
![alt text](images/mbart_input_MSA.png)


And here is  the input data  for Egyptian Arabic:
![alt text](images/mbart_input_egy.png)




1. Text Preprocessing
there is many nlp .........

the main two are: **NLTK and sPacy**
because 
but I choose NLTK

 - **NLTK library**
I used NLTK library to remove HTML tags, punctuations, and symbols from text. Also I used to define stop words.

2. Text Summarization

 - **Text Summarization Using the Frequency Method**
   In this method, we first find the frequency of all the words in our text data. We do this by creating a dictionary where each word is associated with its frequency. Once we have the frequency dictionary, we tokenize our text data. Finally, we select the sentences that contain the most high-frequency words and store them in our final summary data.

Here is the output of the Summarization of MSA Wikipedia Page. It is a 111 words summary:

![alt text](images/msa_output_freq.png)


[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1J4BvJBUsQZYoMCHsGR8-zYgEPQ4_Huu_?usp=sharing)

 - **Text Summarization Using Hugging Face Transformers**
I used the HuggingFace transformers library. The Transformers library provides thousands of pre-trained models to perform tasks such as text summarization. the two pre-trained models that i try and worked are the following:

1. [Albert](https://huggingface.co/albert-base-v2) ⭐️: 

Summarization Output. It is a 55 words summary:

![alt text](images/albert_output.png)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1J5p72_I7IbZNHFkrzUKh2DMfAapSPDQU?usp=sharing)

2. [mBART-50](https://huggingface.co/facebook/mbart-large-50) ⭐️: 

Summarization Output. It is a 59 words summary:

![alt text](images/mbart_output_msa.png)

I have noticed that the mBART-50 model only outputs the first words of a text based on the maximum length specified.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1odB49lxv9dqipToxO4ww6eTqqCTv18eG?usp=sharing)



