# README.md
## Generate TV scripts using Tensorflow.
### Project 3 of [Deep Learning Foundation](https://www.udacity.com/course/deep-learning-nanodegree-foundation--nd101)
#### Perry Radau
Using scripts from Simpson’s cartoon (specifically Moe’s Tavern), the LSTM Recurrent Neural Network (RNN) will generate new scripts. This example is interesting because the trained model has learned to generate sentences which are semi-grammatical and semi-sensible based on statistical relationships in sequences of words, with no linguistic knowledge or encoded rules. 

The data is unlabelled as we are only interested in predicting new word sequences similar to previously found in the data.

The network demonstrates key principles of deep learning:

LSTM cells, generative networks, batching and fully connected layers.

The training error (“loss”) was calculated to be about 0.383 for 50 epochs of 26 batches, each of size 256 words.  

The training was accomplished by running the jupyter notebook on the Deep Learning platform, Floydhub.com.
