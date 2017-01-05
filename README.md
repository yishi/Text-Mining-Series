# Text-Mining-Series

Several days ago, I discover a new package about text mining in R, **text2vec**, this package is great, I use this package and other packages to predict the defect name from the defect description text, this idea is similar to sentiment analysis, just change response variable Y values from positive/negative to defect name1/2/3/...

Below is a flowchart about text mining.

text data  
  |  
**segmentation**（for chinese text）jiebaR package  
  |  
transform to structural data, such as matrix, use text2vec package, English text could split the sentence to word in this package, which is similar to segmentation  
1. **data clean**  
first of all, delete stop words  
second, choose the number of the word to make vector, n-gram  
third, delete very common and very unusual terms  
fourth, whether to use hashing trick, which could shorten the run time when there have large collections of documents  
fifth, make a document-term matrix  
2. **transform document-term matrix**  
normalization：decrease the influence of the lengths of the documents  
tf-idf：increase the weight of terms which are specific and decrease the weight for terms used in most documents    
|  
use **model**, such as sentiment analysis, use classification model, to predict positive or negative

Below is my R and Python code:

**Sentiment Analysis and related**
[Text Mining Series 1.1: Sentiment Analysis in Movie Review Dataset in English by R]
(https://github.com/yishi/my_R_code/blob/master/sentiment%20analysis%20for%20English%20text)

[Text Mining Series 1.2: Predict Defect Name From Defect Description Text in Chinese by R]
(https://github.com/yishi/my_R_code/blob/master/predict%20defect%20name%20for%20Chinese%20text)

[Text Mining Series 1.3: Predict Defect Name From Defect Description Text in Chinese by Python](http://nbviewer.jupyter.org/github/yishi/Text-Mining-Series/blob/master/Text_mining_series_1.ipynb)

**Spell Checker**
[Text Mining Series 2.1: Make a Spell Checker for English Text by Python](http://nbviewer.jupyter.org/github/yishi/Text-Mining-Series/blob/master/Text_mining_series_2.ipynb)

[Text Mining Series 2.2: Make a Spell Checker for English and Chinese Text by R](https://github.com/yishi/my_R_code/blob/master/spell%20checker%20for%20English%20and%20Chinese%20Text)


