```

Name - David Garg
Roll No. - 19075089
CSE (BTECH)

```

# AI Lab Task 5


## Isolated Word Morphological Analysis


### Morphological Analysis
.
Morphological Analysis study of word formation – how words are built up from smaller pieces. • Identification, analysis, and description of the structure of a given language's MORPHEMES and other linguistic units, such as root words, affixes, parts of speech, intonations and stresses, or implied context. Morphological Analysis is the process of determining the morphemes from which a given word is constructed.
For doing Morphological Analysis I used a multi-task learning CNN-RNN model combined together with the potential of task-optimized phonetic features to predict the Lemma, POS category, Gender, Number, Person, Case, and Tense-aspect-mood (TAM) of Hindi word


### Folder Structure

Main Folder consists of following folders and files :-

Folders:-

HINDI - The Folder that contains HINDI Language Morphological Analysis files.
URDU - The Folder that contains URDU Language Morphological Analysis files.

Files:-

Readme - A Readme File for my AI Lab Task 5


### HINDI Folder:-

Consists of following things :-

Graph_Outputs - In this output folder there are graph output files as feature_0(POS_curve), feature_1(gender_curve), feature_2(number_curve), feature_3(person_cuve),feature_4(case_curve), feature_5(tense-aspect-mood (TAM_curve)).

model_with_phonetic_hindi.hdf5 - This is our model file having the model weights.

Hindi.iypnb - This is the python notebook containing the step the I performed.


### URDU Folder:-

Consists of following things :-

Graph_Outputs - In this output folder there are graph output files as feature_0(POS_curve), feature_1(gender_curve), feature_2(number_curve), feature_3(person_cuve),feature_4(case_curve), feature_5(tense-aspect-mood (TAM_curve)).

model_with_phonetic_urdu.hdf5 - This is our model file having the model weights.

Urdu.iypnb - This is the python notebook containing the step the I performed.


## Packages and Dataset :

	
 Packages that were used are h5py, numpy, Keras, tensorflow, Keras-Applications, Keras-Preprocessing, PyYAML, matplotlib, scikit-learn
 I used the data which can be extracted from: http://ltrc.iiit.ac.in/hutb_release/


## Procedure: 

  1. First step is always dataset step. I first downloaded the dataset of Hindi and Urdu Language from the link which was mentioned earlier.
  2. After that I trained the model using convolutional neural network and recurrent neural networks model combined together(CNN-RNN model).
  3. This generated a model_weights model file which was used in next steps.
  4. Then I tested the model on some data which I had already had for testing.
  5. Then I used the model for prediction by using some model data. The model predicted  Lemma, POS category, Gender, Number, Person, Case, and Tense-aspect-mood (TAM).
  Note:- I am not mentioning the commands as commands are explained better in python Notebook.
  
  ## Result
  
   #### Hindi Result for All Features : -
   Average precision score, micro-averaged over all classes: 0.04460726393741833
   Average precision score, micro-averaged over all classes: 0.20988512556490657
   Average precision score, micro-averaged over all classes: 0.1732157497786222
   Average precision score, micro-averaged over all classes: 0.08662825608711429
   Average precision score, micro-averaged over all classes: 0.14176995763361663
   Average precision score, micro-averaged over all classes: 0.6255491012325229
   
   #### Hindi Result for All Features : -
   Average precision score, micro-averaged over all classes: 0.027397654184136627
   Average precision score, micro-averaged over all classes: 0.05063749672768177
   Average precision score, micro-averaged over all classes: 0.1527746699660005
   Average precision score, micro-averaged over all classes: 0.0693994937806469
   Average precision score, micro-averaged over all classes: 0.3611323022150249
   Average precision score, micro-averaged over all classes: 0.32827995148386574



  
  ## Motivation
  
  Now the question arises what was my motivation to do this I wanted to explore Neuro-Linguistic Programming(NLP) and I got to know that Morphological Analysis(MA) is the first step in Neuro-Linguistic Programming(NLP), in which a sentence is divided into a sequence of morphemes and then we determine parts of speech of the segmented morpheme. So I searched some ways to do that I found this CNN-RNN way best . So I did this . I learned a lot from this
  
  
