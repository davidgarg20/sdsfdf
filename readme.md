```

Name - David Garg
Roll No. - 19075089
CSE (BTECH)

```

# AI Lab Task 7


##  Bilingual Dictionary Induction from Comparable Corpora


### Bilingual Dictionary

А  bilinguаl  diсtiоnаry  оr  trаnslаtiоn  diсtiоnаry  is  а  sрeсiаlized  diсtiоnаry  used  tо  trаnslаte  wоrds  оr  рhrаses  frоm  оne  lаnguаge  tо  аnоther.  Bilinguаl  diсtiоnаries  саn  be  unidireсtiоnаl,  meаning  thаt  they  list  the  meаnings  оf  wоrds  оf  оne  lаnguаge  in  аnоther,  оr  саn  be  bidireсtiоnаl,  аllоwing  trаnslаtiоn  tо  аnd  frоm  bоth  lаnguаges.  Bidireсtiоnаl  bilinguаl  diсtiоnаries  usuаlly  соnsist  оf  twо  seсtiоns,  eасh  listing  wоrds  аnd  рhrаses  оf  оne  lаnguаge  аlрhаbetiсаlly  аlоng  with  their  trаnslаtiоn.In  соntrаst  tо  the  bilinguаl  diсtiоnаry,  а  mоnоlinguаl  diсtiоnаry  defines  wоrds  аnd  рhrаses  insteаd  оf  trаnslаting  them.

## About Task

The task is Bilingual Dictionary Induction from Comparable Corpora. the task


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


## Packages and Dataset :

	
 Packages that were used are - pytorch , pandas , matplotlib ,high resource hindi and german dataset, low resource middle-high-german and bengali dataset , Numpy ,random
 I used the data which can be extracted from: https://unimorph.github.io/


## Procedure: 

  1. First step is always dataset step. I first downloaded the all dataset Language from the link which was mentioned earlier.
  2. After that I trained the  encoder-decoder model modified by a custom trainer that trains only with the target language resources after aspecific threshold..
  3. This generated a encoder and decoder file which was used in next steps.
  4. Then I tested the model on some test data which I had already had for testing.
  5. Then I used the model for prediction by using some model data. The model predicted  the word.
  Note:- I am not mentioning the commands as commands are explained better in python Notebook.
  
  
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
  

 
 
 
