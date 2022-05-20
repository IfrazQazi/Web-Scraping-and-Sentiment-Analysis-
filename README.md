# Web-Scraping-and-Sentiment-Analysis-

# Objective :

The objective of this assignment is to extract textual data articles from the given URL and perform text analysis to compute variables that are explained below.

# Data Extraction

For each of the articles, given in the input.xlsx file, extract the article text and save the extracted article in a text file with URL_ID as its file name. While extracting text, please make sure your program extracts only the article title and the article text. It should not extract the website header, footer, or anything other than the article text.

# Data Analysis
For each of the extracted texts from the article, perform textual analysis and compute variables.

# Variables
* POSITIVE SCORE
* NEGATIVE SCORE
* POLARITY SCORE
* SUBJECTIVITY SCORE
* AVG SENTENCE LENGTH
* PERCENTAGE OF COMPLEX WORDS
* FOG INDEX
* AVG NUMBER OF WORDS PER SENTENCE
* COMPLEX WORD COUNT
* WORD COUNT
* SYLLABLE PER WORD
* PERSONAL PRONOUNS
* AVG WORD LENGTH
* 
# Lets understand variables

# Sentimental Analysis
Sentimental analysis is the process of determining whether a piece of writing is positive, negative or neutral.

![image](https://user-images.githubusercontent.com/60994606/169444292-9f2a144e-6588-4afb-b7d7-f4bf14df91d6.png)


* POSITIVE SCORE

* NEGATIVE SCORE

* POLARITY SCORE:

  Polarity lies between [-1,1], -1 defines a negative sentiment and 1 defines a positive sentiment.

* SUBJECTIVITY SCORE:

  Subjectivity quantifies the amount of personal opinion and factual information contained in the text.
  The higher subjectivity means that the text contains personal opinion rather than factual information.
  
# Analysis of Readability

Analysis of Readability is calculated using the Gunning Fox index formula described below.
* Average Sentence Length = the number of words / the number of sentences

* Percentage of Complex words = the number of complex words / the number of words

* Fog Index = 0.4 * (Average Sentence Length + Percentage of Complex words)

* Fog Index :

  The fog index is commonly used to confirm that text can be read easily by the intended audience. Texts for a wide audience generally need a fog index less than 12.     Texts requiring near-universal understanding generally need an index less than 8.

# Average Number of Words Per Sentence
The formula for calculating is:

Average Number of Words Per Sentence = the total number of words / the total number of sentences

# Complex Word Count
Complex words are words in the text that contain more than two syllables.

# Word Count

We count the total cleaned words present in the text by

removing the stop words (using stopwords class of nltk package).

removing any punctuations like ? ! , . from the word before counting.

# Syllable Count Per Word :

We count the number of Syllables in each word of the text by counting the vowels present in each word. We also handle some exceptions like words ending with "es","ed" by not counting them as a syllable.

# Personal Pronouns

To calculate Personal Pronouns mentioned in the text, we use regex to find the counts of the words
“I,” “we,” “my,” “ours,” and “us”. Special care is taken so that the country name US is not included in the list.

# Average Word Length:

Average Word Length is calculated by the formula:

Sum of the total number of characters in each word/Total number of words
