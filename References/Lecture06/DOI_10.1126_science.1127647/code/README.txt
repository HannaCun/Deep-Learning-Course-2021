% Code provided by Ruslan Salakhutdinov and Geoff Hinton
%
% Permission is granted for anyone to copy, use, modify, or distribute this
% program and accompanying programs and documents for any purpose, provided
% this copyright notice is retained and prominently displayed, along with
% a note saying that the original programs are available from our
% web page.
% The programs and documents are distributed without any warranty, express or
% implied.  As the programs were written for research purposes only, they have
% not been tested to the degree that would be advisable in any important
% application.  All use of these programs is entirely at the user's own risk.

How to make it work:

   1. Create a separate directory and download all these files into the same directory
   2. Download from http://yann.lecun.com/exdb/mnist the following 4 files:
          * train-images-idx3-ubyte.gz train-labels-idx1-ubyte.gz
          * t10k-images-idx3-ubyte.gz t10k-labels-idx1-ubyte.gz 
   3. Unzip these 4 files by executing:
          * gunzip train-images-idx3-ubyte.gz
          * gunzip train-labels-idx1-ubyte.gz
          * gunzip t10k-images-idx3-ubyte.gz
          * gunzip t10k-labels-idx1-ubyte.gz 
   4. Download Conjugate Gradient code minimize.m available at 
     http://www.kyb.tuebingen.mpg.de/bs/people/carl/code/minimize/
   5. Download the following 9 files for training an autoencoder:
          * mnistdeepauto.m Main file for training deep autoencoder
          * converter.m Converts raw MNIST digits into matlab format
          * rbm.m Training RBM with binary hidden and visible units
          * rbmhidlinear.m Training RBM with Gaussian hidden and binary visible units
          * backprop.m Backpropagation for fine-tuning an autoencoder
          * CG_MNIST.m Conjugate Gradient optimization
          * makebatches.m Creates minibatches for RBM training
          * mnistdisp.m Displays progress during fine-tuning stage 
          * README.txt  
   6. Run mnistdeepauto.m in matlab.
   7. Make sure you have enough space to store the entire MNIST dataset on your disk. 
      You can also set various parameters in the code, such as maximum number of epochs, 
      learning rates, network architecture, etc. 

