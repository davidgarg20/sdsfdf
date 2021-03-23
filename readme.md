```

Name - David Garg
Roll No. - 19075089
CSE (BTECH)

```

# AI Lab Task 6


## Isolated Word Morphological Generation


### Morphological Analysis

The smallest meaningful word in a sentence or a phrase in any language is known as morpheme. In well-spaced sentences , Morphological Analysis(MA) is the first step in Neuro-Linguistic Programming(NLP), in which a sentence is divided into a sequence of morphemes and then we determine parts of speech of the segmented morpheme.
Morphological generation is just inverse of Morphological analysis. Morphlogical inflection Generation is the task of generating the inflected form of a given lemma corresponding to a particular lingusitic transformation. It is a mechnaism of word formation to express different grammatical categories such as tense, mood, voice , aspect , person , gender , number etc.. 


### Folder Structure

Main Folder consists of following folders and files :-

Folders:-

HINDI - The Folder that contains HINDI Language Isolated Word Morphological Generation files.
GERMAN - The Folder that contains GERMAN Language Isolated Word Morphological Generation files.
MIDDLE-HIGH-GERMAN - The Folder that contains MIDDLE-HIGH-GERMAN Language Isolated Word Morphological Generation files.
BENGALI - The Folder that contains BENGALI Language Isolated Word Morphological Generation files.

Files:-

Readme - A Readme File for my AI Lab Task 6


### HINDI Folder:-

Consists of following things :-

decoder.dict - This is encoder file for HINDI Isolated Word Morphological Generation

encoder.dict - This is decoder file for HINDI Isolated Word Morphological Generation

HINDI.iypnb - This is the python notebook containing the step the I performed.


### GERMAN Folder:-

Consists of following things :-

decoder.dict - This is encoder file for GERMAN Isolated Word Morphological Generation

encoder.dict - This is decoder file for GERMAN Isolated Word Morphological Generation

GERMAN.iypnb - This is the python notebook containing the step the I performed.


### MIDDLE-HIGH-GERMAN Folder:-

Consists of following things :-

decoder.dict - This is encoder file for MIDDLE-HIGH-GERMAN Isolated Word Morphological Generation

encoder.dict - This is decoder file for MIDDLE-HIGH-GERMAN Isolated Word Morphological Generation

MIDDLE-HIGH-GERMAN.iypnb - This is the python notebook containing the step the I performed.


### BENGALI Folder:-

Consists of following things :-

decoder.dict - This is encoder file for BENGALI Isolated Word Morphological Generation

encoder.dict - This is decoder file for BENGALI Isolated Word Morphological Generation

BENGALI.iypnb - This is the python notebook containing the step the I performed.


## Packages and Dataset :

	
 Packages that were used are - pytorch , pandas , matplotlib ,high resource hindi and german dataset, low resource middle-high-german and bengali dataset , Numpy ,random
 I used the data which can be extracted from: https://unimorph.github.io/


## Procedure: 

  1. First step is always dataset step. I first downloaded the all dataset Language from the link which was mentioned earlier.
  2. After that I trained the model using ml model using pytorch.
  3. This generated a encoder and decoder file which was used in next steps.
  4. Then I tested the model on some test data which I had already had for testing.
  5. Then I used the model for prediction by using some model data. The model predicted  the word.
  Note:- I am not mentioning the commands as commands are explained better in python Notebook.
  
  ## Result
  
   #### Hindi Result for All Features : -
   
   Feature 1: Average precision score, micro-averaged over all classes: 0.04460726393741833
   
   Feature 2: Average precision score, micro-averaged over all classes: 0.20988512556490657
   
   Feature 3: Average precision score, micro-averaged over all classes: 0.1732157497786222
   
   Feature 4: Average precision score, micro-averaged over all classes: 0.08662825608711429
   
   Feature 5: Average precision score, micro-averaged over all classes: 0.14176995763361663
   
   Feature 6: Average precision score, micro-averaged over all classes: 0.6255491012325229
   
   #### Hindi Result for All Features : -
   
   Feature 1: Average precision score, micro-averaged over all classes: 0.027397654184136627
   
   Feature 2: Average precision score, micro-averaged over all classes: 0.05063749672768177
   
   Feature 3: Average precision score, micro-averaged over all classes: 0.1527746699660005
   
   Feature 4: Average precision score, micro-averaged over all classes: 0.0693994937806469
   
   Feature 5: Average precision score, micro-averaged over all classes: 0.3611323022150249
   
   Feature 6: Average precision score, micro-averaged over all classes: 0.32827995148386574



  
  ## Motivation
  
  Now the question arises what was my motivation to do this I wanted to explore Neuro-Linguistic Programming(NLP) and I got to know that Morphological Analysis(MA) is the first step in Neuro-Linguistic Programming(NLP), in which a sentence is divided into a sequence of morphemes and then we determine parts of speech of the segmented morpheme. So I searched some ways to do that I found this CNN-RNN way best . So I did this . I learned a lot from this
  
  
