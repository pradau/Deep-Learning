# README.md
## Translate English to French using Tensorflow
### Project 4 of [Deep Learning Foundation](https://www.udacity.com/course/deep-learning-nanodegree-foundation--nd101)
#### Perry Radau
Using a corpus of English source texts and French target texts for training, the LSTM Recurrent Neural Network (RNN) will translate new English sentences into French. 


The data is unlabelled as we are only interested in predicting new word sequences similar to previously found in the data.

The network demonstrates key principles of deep learning:

* multi-layer recurrent neural nets (RNNs) made up of LSTM cells.
* that a language can be translated without knowing any linguistics or grammar, instead relying on statistics and word order.
* representing words as vectors (embedding).
* an RNN network with dropout as a regularizer (i.e. to reduce overfitting).


The validation accuracy was determined to be at best 93% after 4 epochs of training with an optimization "loss" (cost) of 0.06.
This network has a 4 layer LSTM network, with RNN size of 512, and embedding size of 25 (both encoding and decoding). 

The training was accomplished by running the jupyter notebook on the Deep Learning platform, Floydhub.com.
