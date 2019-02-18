# Problem and Objective

During the gasoline shortage crisis in Florida in the onset of Irma, the following kinds of tweets were observed:
* "The shelters are full, there is no gas. Tornados could happen, and storm surge is predicted. So what are people supposed to do? Irma "
* "Insane..95 percent of Florida trying to leave at one time. Roads r slammed. No gas. No hotels available. Scared to see my neighborhood after irma"
* "Gas stations out of gas, water shelves empty, stores and airports closed. Stocked up on food and wine, waiting on irma"

The natural question that arises is that can social media be used to detect gasoline shortage. In this project we explored the potential of different deep neural netwroks in detecting such tweets using Keras

# Methodology

To build the most accurate classifier we did 3 kinds of experiments:

* Testing different kinds of Classifiers
* Varying the Hyper-parameters of the most accurate classifier
* Varying the Embedding Matrix


We tested 3 different kinds of ANN’s:

* LSTM
* CNN with a Convolutional Layer
* CNN with a Convolutional and a Maxpool Layer


We found that LSTM was the best performer amongst all the classifiers as described in the result section. Hence to find the most accurate LSTM classifier, we varied the following hyper parameters:

* Number of units in the LSTM Hidden Layer 
* Dropout Ratio
* Learning Rate of Adadelta Optimizer


We also tested on three different kinds of Word Embedding:
* Self-trained Word Embeddings in Keras
* Word Embeddings from CrisisNLP’s github repository 
* Word Embedings from Glove 

# Results 
The hiegst validation accuracy is achieved for LSTM, units = 100, dropout ratio = 0.5, learning rate = 1, with the Glove embeddig matrix.
For detailed results check the attached juputer notebook.

