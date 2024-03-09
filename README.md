# Parallel CNN Training
## Abstract
Training complex models can take a significant amount of time. The purpose of our study is to train a convolutional neural network (CNN) using parallelization to reduce training time. We also train a separate CNN sequentially and compare the training time and accuracy of both models. 

## Introduction
A convolutional neural network (CNN) is a machine learning system that is mostly used for image feature recognition. An image is fed into the CNN, and it filters out features of the image (like shapes, for example) to detect patterns. A CNN uses convolution to create a convolved feature; and pooling, which downsamples the image created by the filter to use for computations. CNNs are used most commonly for image classifications or recognitions. They are also used for other forms of media, like audio processing. 
The amount of time a CNN takes to train depends on the size of the dataset, hardware used (e.g. GPU, CPU), the complexity of the network, among other factors. If all other factors remain the same, increasing the size of the dataset increases the time taken for the CNN to train, as the CNN must both load the data and process the data. 
Our solution to this problem is to distribute the workload of training the CNN across multiple threads to speed up the training time. By parallelizing data loading and processing, we hope to dramatically decrease loading times and improve data processing times by using multi-threading.

## Methodology
For our study, we use the CIFAR-10 dataset, which contains 60,000 color images in 10 classes, with 6,000 images in each class. The training dataset is composed of 50,000 of the images while the testing dataset consists of 10,000 of the images.  

To build the convolutional base of the CNN, we use the common pattern of a stack of 2D convolution and max pooling layers. Define 2D convolution and max pooling layers. The format of the CIFAR images is of shape (32, 32, 3), so we configure our CNN to process inputs of this shape. To complete our model and perform classification, we feed the last output tensor from the convolutional base into Dense layers. Talk about Dense layers here.  

To sequentially train our CNN, we optimize the categorical cross entropy loss function. Talk about loss function and optimization here.  

Describe our parallelization approach here


## Implementation
* Using the Keras API to create the model
* Insert images / code of CNN and layers
* Insert code of how we are using parallelization with the CNN

## Testing and Analysis / Results
* Time it takes to train CNN with parallelization
* Time it takes to train CNN with sequential training
    * On average, each epoch takes about 7-9 seconds to complete
* Is there a difference in accuracy between the two training methods?
* Insert images of accuracy plot

## Conclusion
## References
