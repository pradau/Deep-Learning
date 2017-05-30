# README.md
## DCGAN in Tensorflow for Face Generation
### Deep Convolutional Generative Adversarial Network 
### Project 5 of [Deep Learning Foundation](https://www.udacity.com/course/deep-learning-nanodegree-foundation--nd101)
#### Last update: May 30, 2017
#### Perry Radau
1 The project will run the DCGAN first (for testing) on the [MNIST handwritten digit dataset](http://yann.lecun.com/exdb/mnist/).  
In effect this will generate "fake" images of handwritten numbers (1 to 10) that could pass as images from real handwriting.

2 Then it will be run on the [CelebA celebrity faces dataset](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html).  
The effect is that from a vector of noise intensities the DCGAN is able to generate faces that could pass as real (but low-res)
images of celebrity face photos.

The network demonstrates key principles of deep learning:
* generative adversarial networks (GANs) may be used to generate images from noise vectors by competing discriminator and generator networks.
* it does this by a transfer of information from the discriminator network that classifies real images of the desired type to the generator network.
* the GAN operates by the generator learning which of its generated ("fake") images are able to trick the discriminator into 
classifying them as true ("real").
* the discriminator and generator learn in tandem to improve at their respective tasks. If either one learns too much faster
than the other the DCGAN will fail. Ideally the two networks train so that they reach an equilibrium. 
i.e. their loss vs training steps graph has both approaching a flat line where neither has a loss that explodes or goes to zero.
* using deep convolutional layers in both the discriminator and generator improves the results, especially for the faces.
* dropout to regularize the generator.
* label smoothing to make the discriminator losses larger, hence the generator and discriminator are more competitive.
* generating the noise vector from sampling a Gaussian distribution (instead of uniform) is demonstrated.

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

### References
#### Key paper:

[Unsupervised Representation Learning with DCGANs by Radford,Metz, Chintala](https://arxiv.org/abs/1511.06434)

#### Key github implementation in tensorflow:

[Taehoon Kim a.k.a. carpedm20](https://github.com/carpedm20/DCGAN-tensorflow)

#### How to train a GAN: Tips and Tricks

[Soumith Chintala a.k.a. soumith](https://github.com/soumith/ganhacks)
