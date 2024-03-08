# Parallel CNN Training
## Abstract
Training complex models can take a significant amount of time. The purpose of our study is to train a convolutional neural network (CNN) using parallelization to reduce training time. We also train a separate CNN sequentially and compare the training time and accuracy of both models. 

## Introduction


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
