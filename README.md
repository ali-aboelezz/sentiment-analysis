# sentiment-analysis


1- the main goal:

building a machine learning model to detect sentiment (i.e. detect if a sentence is positive or negative) using PyTorch and TorchText. This will be done on movie reviews, using the IMDb dataset We will use:

packed padded sequences
pre-trained word embeddings
different RNN architecture
bidirectional RNN
multi-layer RNN
regularization
Adam optimizer
This will allow us to achieve ~85% test accuracy.

2- the dataset
the movie reviews from the IMDb website we will get the data from the torchtext.legacy module

3- the model 

We'll be using a different RNN architecture called a Long Short-Term Memory (LSTM). Why is an LSTM better than a standard RNN? Standard RNNs suffer from the vanishing gradient problem. LSTMs overcome this by having an extra recurrent state called a cell,  𝑐  - which can be thought of as the "memory" of the LSTM - and the use use multiple gates which control the flow of information into and out of the memory.

 As well as having an RNN processing the words in the sentence from the first to the last (a forward RNN), we have a second RNN processing the words in the sentence from the last to the first (a backward RNN). At time step  𝑡 , the forward RNN is processing word  𝑥𝑡 , and the backward RNN is processing word  𝑥𝑇−𝑡+1 .
 
 4- the results
 
 we get the accuracy of 89.28% on the training phase and  valid accuracy 86.30% 
 and test accuracy 85.84%


