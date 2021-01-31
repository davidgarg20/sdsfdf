
###########

AI Lab Task 2

###########


#####

Commands

#######

### Command to train data:
crf_learn <template file> <train file> <model file name to be given>

### Command to test data:
crf_test -m <model file> <test file> > output.txt 
 
- (Here, > used for storing the result after testing of data in result file)

### Command to accuracy:
python3 accuracy.py > output.txt

- Accuracy will be stored in output.txt file.


###########

Folder Structure

###########


Main Folder consists of following folders and files :-

Folders:-

Chunking - The Folder that contains chunking files.
POS_Tagging - The Folder that contains POS_tagging files.
NER - The Folder that contains Named Entity Recognition files.

Files:-

Readme - A Readme File for my AI Lab Task 2


-----Chunking Folder:-

Consists of following sub-folders :-

Chunking_1 
Chunking_2
Chunking_3
Chunking_4
Chunking_5


A Chunking_{i} folder components as follows :-

model file :- The file that conatins model build after training data.
template file :- A Template file that contains template that i used for Chunking.
result.txt file :- It is the file that contains result that I got after test my model on the test.
output.txt :- It contains the output that we got on testing the data.



-----POS_Tagging Folder:-

Consists of following sub-folders :-

POS_Tagging_1 
POS_Tagging_2
POS_Tagging_3
POS_Tagging_4
POS_Tagging_5


A POS_Tagging_{i} folder components as follows :-

model file :- The file that conatins model build after training data.
template file :- A Template file that contains template that i used for POS_Tagging.
result.txt file :- It is the file that contains result that I got after test my model on the test.
output.txt :- It contains the output that we got on testing the data.



-----NER Folder:-

Consists of following sub-folders :-

English Folder :- It conatins my crf analysis on English Language Database

NER_English1
NER_English2
NER_English3
NER_English4
NER_English5


A NER_English{i} folder components as follows :-

model file :- The file that conatins model build after training data.
template file :- A Template file that contains template that i used for NER.
result.txt file :- It is the file that contains result that I got after test my model on the test.
output.txt :- It contains the output that we got on testing the data.


Spanish Folder :- It conatins my crf analysis on English Language Database

NER_Spanish1
NER_Spanish2
NER_Spanish3


A NER_Spanish{i} folder components as follows :-

model file :- The file that conatins model build after training data.
template file :- A Template file that contains template that i used for NER.
result.txt file :- It is the file that contains result that I got after test my model on the test.
output.txt :- It contains the output that we got on testing the data.




Now I going to discuss about the chunking :-

Chunking is a process of extracting phrases from unstructured text. Chunking works on top of POS tagging, it uses POS-tags as input and provides chunks as output. Chunking is very important when you want to extract information from text.
In chunking I have tried five templates which are diffrent and anaysed the accuracy that I got on these templates.
Dataset -
The dataset is extracted from the provided CoNLL shared task 2000. 

Chunking_1 Template:-

In this template 1 have used the default template as provided by the CoNLL shared task 2000.

Chunking_2 Template:-

In this template 2 I have used a minimum no of features and window size. In this template I have got the minimal accuracy.

Chunking_3 Template:-

In the template 3 I have increased the no of features then previous one as a result my accuracy increased.

Chunking_4 Template:-

In the template 4 I have changed a little bit from default template like I am also taking 3rd previous word in consideration which was not taken in consideration in default template but I observed that the acccuracy nearly remain the same which gave ne the idea considering more previous anf after words affects accuracy to the limited extent.

Chunking_5 Template:-

In the template 5 I have just added a line a feature keep the after words and previous words same to the default template and in this I observed that the accuracy are almost same as default template accuracy.


Following are the results that I got :-

#Result -------------------------
Accuracy                 :  96.06146312634556
Correctly tagged words   :  45512
Incorrectly tagged words :  1866
Total words              :  47378
Total sentences          :  2013

#Result -------------------------
Accuracy                 :  93.96753699052283 %
Correctly tagged words   :  44519
Incorrectly tagged words :  2858
Total words              :  47377
Total sentences          :  2012

#Result -------------------------
Accuracy                 :  95.54002997234946
Correctly tagged words   :  45264
Incorrectly tagged words :  2113
Total words              :  47377
Total sentences          :  2012

#Result -------------------------
Accuracy                 :  95.70466682145344
Correctly tagged words   :  45342
Incorrectly tagged words :  2035
Total words              :  47377
Total sentences          :  2012

#Result -------------------------
Accuracy                 :  96.05293707917343
Correctly tagged words   :  45507
Incorrectly tagged words :  1870
Total words              :  47377
Total sentences          :  2012



Now I going to discuss about the POS_Tagging :-

######

Part of Speech tagging.

######
It is a process of converting a sentence to forms – list of words, list of tuples (where each tuple is having a form (word, tag)). The tag in case of is a part-of-speech tag, and signifies whether the word is a noun, adjective, verb, and so on.
Data Set

The Data Set is extracted from the Chunking Data Set using the following command-
	awk '(print  $1,$2)' filename

POS_Tagging_1:-

In the first template I took minimal feature set consided only using three token feature of zeroth token feature next word token feature and previous word token feature to get the accuracy.

POS_Tagging_2:-

In the second template I have increased the window size to analyse its effect.

POS_Tagging_3:-

In the third template I have used token feature along with POS .

POS_Tagging_4:-

In the fourth template I have used another different set of features to understand the feature working more effectively.

POS_Tagging_5:-

In the fifth template I have used the features same as template 3 but in the diffent order I observed that order of features also makes effect on accuracy.

Following are the results that I got :-

#Result -------------------------
Accuracy                 :  93.6403740211495
Correctly tagged words   :  44364
Incorrectly tagged words :  3013
Total words              :  47377
Total sentences          :  2012

#Result -------------------------
Accuracy                 :  92.92272621736285
Correctly tagged words   :  44024
Incorrectly tagged words :  3353
Total words              :  47377
Total sentences          :  2012

#Result -------------------------
Accuracy                 :  93.5137302910695
Correctly tagged words   :  44304
Incorrectly tagged words :  3073
Total words              :  47377
Total sentences          :  2012

#Result -------------------------
Accuracy                 :  93.37231145914684
Correctly tagged words   :  44237
Incorrectly tagged words :  3140
Total words              :  47377
Total sentences          :  2012

#Result -------------------------
Accuracy                 :  93.27310720391752
Correctly tagged words   :  44190
Incorrectly tagged words :  3187
Total words              :  47377
Total sentences          :  2012

Now I going to discuss about the NER :-

Named Entity Recognition.
Named entity recognition (NER) is a natural language processing (NLP) technique that automatically identifies named entities in a text and classifies them into predefined categories. Entities can be names of people, organizations, locations, times, quantities, monetary values, percentages, and more.I have used the test and train data for english and spanish language. 
Note –

The dataset is extracted from the provided CoNLL NER shared task 2003. 
I have used kaggale to get the spnaish dataset. 


Following are the results that I got :-


NER English Templates :-

NER_English1 :- 

In the template 1 I have used four set of fetures containing 25+ features .

NER English2 :-

In this template I have increased the no of fetue set and window sizes I have tried maximum feature set that I was able to think in this template.

NER English3 :-

In this template I have reduced the no of fetures and POS from the previous template to understand the effect more betterly.

NER English4 :-

In this template I have considered the word , POS , sub-POS , word/POS , prev/POS as the feature set to get the results.

NER_English5 :-

In this template I have considered the word , POS , sub-POS , word/POS , prev/POS along with the window of two words as the feature set to get the results.



NER Spanish Templates :-

NER_Spanish1 :-

In this template I have considered the word , POS , sub-POS , word/POS , prev/POS as the feature set to get the results.

NER_Spanish2 :-

In this template I have considered using more high set of feature set to get more analysis of feature.

NER_Spanish3 :-

In this template I have used the window of next and previous two words and I have also used word POS combination as the features.


NER English Database Results:-

#Result -------------------------
Accuracy                 :  96.71953158323316
Correctly tagged words   :  49886
Incorrectly tagged words :  1692
Total words              :  51578
Total sentences          :  3466


#Result -------------------------
Accuracy                 :  96.6574896273605
Correctly tagged words   :  49854
Incorrectly tagged words :  1724
Total words              :  51578
Total sentences          :  3466


#Result -------------------------
Accuracy                 :  96.68075536081275
Correctly tagged words   :  49866
Incorrectly tagged words :  1712
Total words              :  51578
Total sentences          :  3466

#Result -------------------------
Accuracy                 :  95.41858932102835
Correctly tagged words   :  49215
Incorrectly tagged words :  2363
Total words              :  51578
Total sentences          :  3466

#Result -------------------------
Accuracy                 :  96.62065221606112
Correctly tagged words   :  49835
Incorrectly tagged words :  1743
Total words              :  51578
Total sentences          :  3466


NER Spanish Database Results:-

#Result -------------------------
Accuracy                 :  93.86467131492924
Correctly tagged words   :  49676
Incorrectly tagged words :  3247
Total words              :  52923
Total sentences          :  1915

#Result -------------------------
Accuracy                 :  95.97733491161004
Correctly tagged words   :  49460
Incorrectly tagged words :  2073
Total words              :  51533
Total sentences          :  1517

#Result -------------------------
Accuracy                 :  95.5872935788718
Correctly tagged words   :  49259
Incorrectly tagged words :  2274
Total words              :  51533
Total sentences          :  1517



Motivation :- 

My main motivation of trying different templates by studying the different research papers and by studying about chunking pos-tagging and named entity. After studying these I want to observe how a feture effect the result so I tried different templates and got different accuracy nearly everytime . 

Observation:-
I got to more about chunking and pos tagging and ner through trying the templates. I really a lot after trying these templates.I got to know that we need to use features very carefully using a lot of fetures is not the only meausure to increase accuracy . A lot of unrequired feature cause overfitting and decrease the result . Also we need to take in the consider all the major features they all contribute to accuracy. In one tempalte I also chnged the order of feature keeping th features same in that template template the reult I got was different . Similarly I used the same template on different datasets of NER I got accuracy a considerably different from one. So I noted if we are getting a accuracy on a particular datasets then we will get the same accuracy on the other datasets. The accuracy of the template also depends on the datasets.  


Precision F measure etc details about results is given in result.txt files.


Hoping that I performed my Lab Task in the best way that I could .




