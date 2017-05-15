# Deep Generative Networks

This code allows the creation of deep-dream like image for trained convolutional neural networks (CNNs). Images are produced by a deep generative network from a smaller dimensional feature vector. Training is achieved by standard backpropagation algorithms.
This method allows the generation of more realistic looking images than traditional activation maximization methods and gives insight into the CNN's internal representations.

The code is based on the free open-source library <a href="https://keras.io/">Keras</a> and <a href="https://www.tensorflow.org/">Tensorflow</a>. It uses a freely available implementation of the very deep convolutional network <a href="https://arxiv.org/abs/1409.1556">vgg-16</a>.

Two alternatives are possible:
 <ol>
  <li> Generation from scratch (no pretraining): Here, the training is achieved by training the weights of the entire network from an original random distribution. </li>
  <li> Generation from trained generator (with pretraining): Here, the generator network's weights are loaded from an autoencoder that has been trained on a set of images from the <a href="http://www.image-net.org/">ImageNet</a> database. This implementation creates the most realistic-looking images. </li>
</ol> 

Images generated for all of the vgg-16 classes are available in the examples folder.

