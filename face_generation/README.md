# README.md
## DCGAN in Tensorflow for Face Generation
### Deep Convolutional Generative Adversarial Network 
### Project 5 of [Deep Learning Foundation](https://www.udacity.com/course/deep-learning-nanodegree-foundation--nd101)
#### Last update: May 30, 2017
#### Perry Radau
The project will run the DCGAN first (for testing) on the [MNIST handwritten digit dataset](http://yann.lecun.com/exdb/mnist/).  
Then it will be run on the [CelebA celebrity faces dataset](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html).  
The network demonstrates key principles of deep learning:
* generative adversarial networks (GANs) may be used to generate images from noise vectors.
* using deep convolutional layers in the discriminator and generator (i.e. DCGAN) stabilizes the network.
* dropout to regularize the generator.
* label smoothing to make the discriminator losses larger, hence the generator and discriminator are more competitive.

### Usage
To setup the requirements via Anaconda use the environment file to create a conda env called 'tensorflow':

conda env create -f environment.yml 

In the project directory run the [Jupyter notebook](http://jupyter.org/):

jupyter notebook

and select the file dlnd_face_generation.ipynb

Note that this project has fewer dependencies than those listed in that file.
The project was developed with
* Python 3.5.3
* Tensorflow 1.0.0
