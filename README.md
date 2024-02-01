# CONVOLUTIONAL NEURAL NETWORK (CNN)
The convolution layer is the core building block of the CNN. It carries the main portion of the network’s computational load.
This layer performs a dot product between two matrices, where one matrix is the set of learnable parameters otherwise known as a kernel, and the other matrix is the restricted portion of the receptive field. 
The kernel is spatially smaller than an image but is more in-depth. 
This means that, if the image is composed of three (RGB) channels, the kernel height and width will be spatially small, but the depth extends up to all three channels.
Pooling Layer:
The pooling layer replaces the output of the network at certain locations by deriving a summary statistic of the nearby outputs. This helps in reducing the spatial size of the representation, which decreases the required amount of computation and weights. 
The pooling operation is processed on every slice of the representation individually.
Fully Connected Layer:
Neurons in this layer have full connectivity with all neurons in the preceding and succeeding layer as seen in regular FCNN.
This is why it can be computed as usual by a matrix multiplication followed by a bias effect.
The FC layer helps to map the representation between the input and the output.
Non-Linearity Layers:
Since convolution is a linear operation and images are far from linear, non-linearity layers are often placed directly after the convolutional layer to introduce non-linearity to the activation map.
There are several types of non-linear operations, the popular ones being:
1. Sigmoid    2. Tanh  3. ReLU  
