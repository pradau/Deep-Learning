# README.md
## Translate English to French using Tensorflow
### Project 4 of [Deep Learning Foundation](https://www.udacity.com/course/deep-learning-nanodegree-foundation--nd101)
#### Perry Radau
This deep learning neural network demonstrates an algorithm to translate English sentences into French. This is accomplished by having the network train with a corpus of English source texts and French target texts for training, but the final model (translator) could be applied to previously unseen English sentences.


The network demonstrates key principles of deep learning:

* multi-layer recurrent neural nets (RNNs) made up of LSTM cells.
* that a language can be translated without knowing any linguistics or grammar, instead relying on statistics and word order.
* representing words as vectors (embedding).
* an RNN network with dropout as a regularizer (i.e. to reduce overfitting).


The validation accuracy was determined to be at best 93% after 4 epochs of training with an optimization "loss" (cost) of 0.06.
This is a 4 layer LSTM network, with RNN size of 512, and embedding size of 25 (both encoding and decoding). 

The training was accomplished by running the jupyter notebook on the Deep Learning platform, Floydhub.com.
