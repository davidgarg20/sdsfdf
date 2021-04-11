```

Name - David Garg
Roll No. - 19075089
CSE (BTECH)

```

# AI Lab Task 7


##  Bilingual Dictionary Induction from Comparable Corpora


### Bilingual Dictionary

А  bilinguаl  diсtiоnаry  оr  trаnslаtiоn  diсtiоnаry  is  а  sрeсiаlized  diсtiоnаry  used  tо  trаnslаte  wоrds  оr  рhrаses  frоm  оne  lаnguаge  tо  аnоther.  Bilinguаl  diсtiоnаries  саn  be  unidireсtiоnаl,  meаning  thаt  they  list  the  meаnings  оf  wоrds  оf  оne  lаnguаge  in  аnоther,  оr  саn  be  bidireсtiоnаl,  аllоwing  trаnslаtiоn  tо  аnd  frоm  bоth  lаnguаges.  Bidireсtiоnаl  bilinguаl  diсtiоnаries  usuаlly  соnsist  оf  twо  seсtiоns,  eасh  listing  wоrds  аnd  рhrаses  оf  оne  lаnguаge  аlрhаbetiсаlly  аlоng  with  their  trаnslаtiоn.In  соntrаst  tо  the  bilinguаl  diсtiоnаry,  а  mоnоlinguаl  diсtiоnаry  defines  wоrds  аnd  рhrаses  insteаd  оf  trаnslаting  them.

## Introduction

In this task I had used Single_BLI where each source word has only one most likely translation in the target language based on the similarity measure. We have done this using two models described below:-

1. Word2vec —— treats each word in a corpus like an atomic entity and generates a vector for each word ,thus word2vec treats words as the smallest unit to train on.
2. FastText —— which is essentially an extension of the word2vec model — treats each word as composed of character n-grams. So the vector for a word is made of the sum of this character n-grams.

## Fast text and word2vec embedding
These are the two types of embeddings which we are using in our lab task. So a basic understanding of these
two is also required.
### Word2Vec :
Word2Vec is a method to construct such an embedding. It can be obtained using two methods (both
involving Neural Networks): Skip Gram and Common Bag Of Words (CBOW)
### FastText:
FastText is an open-source, free, lightweight library that allows users to learn text representations and text classifiers. It works on standard, generic hardware. Models can later be reduced in size to even fit on mobile devices.

### Folder Structure

Main Folder consists of following folders and files :-

Folders:-

Word2Vec - The Folder that contains Word2Vec files.

FastText - The Folder that contains FastText files.

Files:-

Readme - A Readme File for my AI Lab Task 7


### Word2Vec Folder:-

Consists of following things :-

model_and_embedding.txt - The File contain links of all model and embedding files.

Word2Vec.iypnb - This is the python notebook containing the step the I performed.


### FastText Folder:-

Consists of following things :-

model_and_embedding.txt - The File contain links of all model and embedding files.

FastText.iypnb - This is the python notebook containing the step the I performed.

## Procedure: 
### Word2Vec
  1.  I first downloaded the Word2Vec model dataset  .
  2. Then I unzipped the dataset.
  3. Then I preprocessed the Word2Vec training data.
  4. Then I genertated the Word2Vec models
  5. Then Dowloaded testing data for testing our bilingual model.
  6. Build bilungual model and saved it.
  7. Then I done the embedding mapping using vecmap library.
  8. Then I tested the bilungual model build.

### Word2Vec
  1.  I first downloaded the Fastext model  .
  2. Then I unzipped the FastText.
  3. Then Dowloaded testing data for testing our bilingual model.
  4. Build bilungual model and saved it.
  5. Then I done the embedding mapping using vecmap library.
  6. Then I tested the bilungual model build.

 All the commands can be found in readme file
  
  ## Result
  
 ### Using FastText
  
| Result |English to German | German to English | 
| :---: | :---: | :---: |
|Accuracy| 63.99% | 62.17% | 
|Coverage| 99.55% | 99.40% | 

### Using Word2Vec
   
 | Result |English to German | German to English | 
| :---: | :---: | :---: |
|Accuracy| 45.81% | 43.22% | 
|Coverage| 99.10% | 95.80% | 
  

### Conclusion :

Word2Vec embeddings was less efficient from Fasttext embeddings which may due to the reason we have taken leass data for training the data of word2vec whereas fastext model was prebuild.



 
 
