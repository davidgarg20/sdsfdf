

# AI Lab Task 4


## Named Entity Recognition , Part of Speech Tagging And Chunking Using RNN and Bidirectional LSTM


### Folder Structure



Main Folder consists of following folders and files :-

Folders:-

Chunking - The Folder that contains chunking files.
POS - The Folder that contains POS files.
NER - The Folder that contains Named Entity Recognition files.

Files:-

Readme - A Readme File for my AI Lab Task 2


### Chunking Folder:-

Consists of following sub-folders :-

RNN - Contains the code and model of chunking using RNN
BILSTM - Contains the code and model of chunking using BILSTM

A RNN folder components as follows :-

chunk_rnn_model.pb file :- The file that conatins model build after training data using BILSTM.
Chunking_RNN.ipynb :- The python notebook conataining results and output using RNN.

A BILSTM folder components as follows :-

chunk_bilstm_model.pb file :- The file that conatins model build after training data using BILSTM.
Chunking_BILSTM.ipynb :- The python notebook conataining results and output using BILSTM.


### POS Folder:-

Consists of following sub-folders :-

RNN - Contains the code and model of POS using RNN
BILSTM - Contains the code and model of POS using BILSTM

A RNN folder components as follows :-

pos_rnn_model.pb file :- The file that conatins model build after training data using BILSTM.
POS_RNN.ipynb :- The python notebook conataining results and output using RNN.

A BILSTM folder components as follows :-

pos_bilstm_model.pb file :- The file that conatins model build after training data using BILSTM.
POS_BILSTM.ipynb :- The python notebook conataining results and output using BILSTM.


### NER Folder:-

Consists of following sub-folders :-

RNN - Contains the code and model of NER using RNN
BILSTM - Contains the code and model of NER using BILSTM

A RNN folder components as follows :-

ner_rnn_model.pb file :- The file that conatins model build after training data using BILSTM.
NER_RNN.ipynb :- The python notebook conataining results and output using RNN.

A BILSTM folder components as follows :-

ner_bilstm_model.pb file :- The file that conatins model build after training data using BILSTM.
NER_BILSTM.ipynb :- The python notebook conataining results and output using BILSTM.


### Chunking

Now I going to discuss about the chunking :-

Chunking is a process of extracting phrases from unstructured text. Chunking works on top of POS tagging, it uses POS-tags as input and provides chunks as output. Chunking is very important when you want to extract information from text.
In chunking I have tried five templates which are diffrent and anaysed the accuracy that I got on these templates.
Dataset -
The dataset is extracted from the provided CoNLL shared task 2000. 

RESULTS:-

RNN:-

Loss: 0.05606793239712715,
Accuracy: 0.9818012714385986

BILSTM:-

Loss: 0.050343357026576996,
Accuracy: 0.9845889806747437


### POS

Now I going to discuss about the POS :-

######

Part of Speech tagging.

######
It is a process of converting a sentence to forms – list of words, list of tuples (where each tuple is having a form (word, tag)). The tag in case of is a part-of-speech tag, and signifies whether the word is a noun, adjective, verb, and so on.
Data Set
The dataset is extracted from the provided CoNLL shared task 2000. 


RESULTS:-

RNN:-

Loss: 0.19767414033412933,
Accuracy: 0.9499671459197998

BILSTM:-

Loss: 0.02280944027006626,
Accuracy: 0.9929704070091248


### NER

Now I going to discuss about the NER :-

Named Entity Recognition.
Named entity recognition (NER) is a natural language processing (NLP) technique that automatically identifies named entities in a text and classifies them into predefined categories. Entities can be names of people, organizations, locations, times, quantities, monetary values, percentages, and more.I have used the test and train data for english and spanish language. 
Note –
The dataset is extracted from the provided CoNLL NER shared task 2003. 

RESULTS:-

RNN:-

Loss: 0.08923179656267166,
Accuracy: 0.9825273752212524

BILSTM:-

Loss: 0.019738825038075447,
Accuracy: 0.9945396184921265


### RNN

Recurrent Neural Network is a generalization of feedforward neural network that has an internal memory. RNN is recurrent in nature as it performs the same function for every input of data while the output of the current input depends on the past one computation. After producing the output, it is copied and sent back into the recurrent network. For making a decision, it considers the current input and the output that it has learned from the previous input.

##### Advantages of Recurrent Neural Network

    RNN can model sequence of data so that each sample can be assumed to be dependent on previous ones
    Recurrent neural network are even used with convolutional layers to extend the effective pixel neighbourhood.

##### Disadvantages of Recurrent Neural Network

    Gradient vanishing and exploding problems.
    Training an RNN is a very difficult task.
    
### LSTM

Long Short-Term Memory (LSTM) networks are a modified version of recurrent neural networks, which makes it easier to remember past data in memory. The vanishing gradient problem of RNN is resolved here. LSTM is well-suited to classify, process and predict time series given time lags of unknown duration. It trains the model by using back-propagation.



Hoping that I performed my Lab Task in the best way that I could .
