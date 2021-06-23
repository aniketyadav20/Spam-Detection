
[![LinkedIn][linkedin-shield]][linkedin-url]

# Spam Detection

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project
      </a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project
Spam filters detect unsolicited, unwanted, and virus-infested email (called spam) and stop it from getting into email inboxes. Internet Service Providers (ISPs) use spam filters to make sure they aren’t distributing spam. Small- to medium- sized businesses (SMBs) also use spam filters to protect their employees and networks.

Spam filters are applied to both inbound email (email entering the network) and outbound email (email leaving the network). ISPs use both methods to protect their customers. SMBs typically focus on inbound filters.

There are many spam filtering solutions available. They can be hosted in the “cloud,” on computer servers, or integrated into email software such as Microsoft Outlook.

<p align="center">
<img src="https://lionbridge.ai/wp-content/uploads/2020/08/2020-08-20_nlp_spam-detection.jpg"
 alt="Logo" width="500" height="300">
</p>

### Built With
We use Natural Language Toolkit and other processing libraries.
Here are some term you know before proceeding -
* [String Slicing](https://www.w3schools.com/python/gloss_python_string_slice.asp#:~:text=%E2%9D%AE%20Python%20Glossary-,Slicing%20Strings,a%20part%20of%20the%20string.) 
* [Tokenization](https://www.analyticsvidhya.com/blog/2020/05/what-is-tokenization-nlp/#:~:text=Tokenization%20is%20a%20common%20task%20in%20Natural%20Language%20Processing%20(NLP).&text=Tokens%20are%20the%20building%20blocks,words%2C%20characters%2C%20or%20subwords.)
* [Contraction](https://www.geeksforgeeks.org/nlp-expand-contractions-in-text-processing/)
* [REgex](https://www.w3schools.com/python/python_regex.asp)
* [Stopwords](https://www.tutorialspoint.com/python_text_processing/python_remove_stopwords.htm#:~:text=Stopwords%20are%20the%20English%20words,this%20in%20corpus%20named%20corpus.)
* [Lemmatization](https://www.geeksforgeeks.org/python-lemmatization-with-nltk/)
* [TF-IDF](https://medium.com/analytics-vidhya/tf-idf-term-frequency-technique-easiest-explanation-for-text-classification-in-nlp-with-code-8ca3912e58c3)
* [Principal Component Analysis](https://www.upgrad.com/blog/pca-in-machine-learning/#:~:text=PCA%20is%20an%20unsupervised%20statistical,different%20variables%20%26%20then%20coupling%20them.)
* [Naive Bayes](https://scikit-learn.org/stable/modules/naive_bayes.html)
* [Corpus](https://www.geeksforgeeks.org/nlp-custom-corpus/)



<!-- GETTING STARTED -->
## Getting Started

### Prerequisites
* Any python Compiler (except google colab)

### Installation

1. Import packages
   ```sh
   import pandas as pd
   import numpy as np
   from nltk.tokenize import word_tokenize
   from nltk.corpus import stopwords
   import re
   import nltk
   from contractions import contractions_dict
   from nltk.corpus import stopwords
   from spacy.lang.en.stop_words import STOP_WORDS
   from itertools import filterfalse
   from nltk import pos_tag
   from nltk.stem import WordNetLemmatizer
   from nltk.corpus import wordnet
   from sklearn.feature_extraction.text import TfidfVectorizer
   from sklearn.decomposition import PCA
   from sklearn.naive_bayes import GaussianNB
   from sklearn.metrics import classification_report
   import spacy
   ```



<!-- USAGE EXAMPLES -->
## Usage
The spam filter you choose for your business use depends largely on the amount of email you and your employees receive daily. It also depends on the types of emails sent and received, and your company’s needs and preferences. A business that needs tight security controls may opt for a permission-based filter, while a content filter may be more useful for a business whose employees receive articles and newsletters via email.



<!-- ROADMAP -->
## Roadmap

Install and import all the libraries.
1. Initially we read the dataset email.csv.
2. Then we remove the first useless initial words.
3. And then we allply Tokenization.
4. NOw, we convert all data in lower-case because for compiler A(capital) and a(small) is different.
5. Then we remove Contraction i.e. I'll is I will.
6. Apply regex on the data to remove unnecessary waste words,numbers and symbols.
7. Now, apply Stopwords to remove meaningless words.
8. Now, apply parts of speech tags on the data for Lemmatization.
9. To apply Tf-IDF initially we have to join all the rows and make it like a collection of paragraph called Corpus
10. Apply Tf-Idf to make a matrix.
11. Now, we apply PCA because we have data in proper format.
12. We only take 500 principal components.
13. Then we apply Naive bayes model from Sklearn and from this we get good accuracy.

Here you go! This was a simple way to detect spam mails and happiness😉.
<p align="center">
<img src="https://img.devrant.com/devrant/rant/r_462432_ZzKQZ.gif"
 alt="Logo" width="350" height="275">
</p>

## Contact

Aniket Yadav - [Medium](https://aniketyadavv.medium.com/) - [Gmail](https://yadavaniket0820gmail.com/)
<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/aniket-yadav-2008/
