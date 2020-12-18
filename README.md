# ConvolutionNN
Convolution Neural Network

# Choice of Activation Function -


## Hidden Layer 

***ReLu*** is a preferred choice for all hidden layers because -

 * Its derivative is 1 as long as z is positive and 0 when z is negative.
 * Will be advantageous in terms of speed (computationally inexpensive).
 
In some cases, leaky rely can be used just to avoid exact zero derivatives but its 2nd choice after Relu.
Both **sigmoid** and **tanh** functions are not suitable for hidden layers because if z is very large or very small, the slope of the function becomes very small which slows down the gradient descent which can be visualized in the below video. Rectified linear unit (


**Note:** For deep learning models, it is advisable to start experiments with ***ReLU***.


## Output layer

 * For ***binary classification***, ***sigmoid function*** is a good choice because the actual output value ‘Y’ is either 0 or 1 so it makes sense for predicted output value to be a number between 0 and 1.
 * For non-classification problems such as ***prediction of housing prices,linear activation function*** is more preferable.
 * ***Softmax Function*** is used in output layer of deep learning models, especially when it is necessary to classify ***more than two***.


### General Rule - 
  *  For deep learning models, it is advisable to start experiments with ReLU.
  *  Softmax is usually used in output layers.

