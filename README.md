# Neural-network-from-scratch
Making my own neural network because my brain's doesn't work :( 
We will be using Mnist dataset, problem we will be tackling is digit classification (handwritten digits)

Each image is 28x28 so 784 pixels overall

Every pixel has a value between 0 and 255 (255 being fully white 0 being black)
We have "m" images

So we can make it into a matrix of m rows(m images) and 784 cols
We transpose the matrix
Now there are 784 rows and m cols
So each col is an example 

Our goal is to take an image, do some processing and predict what the number is, with our neural network

We will build a simple 2-layer neural network

Zeroth input layer has 784 nodes, First is a hidden layer of 10 units and second is an output of 10 units from 0-9

There are 3 parts to build this NN

1- Forward propogation 
A0-Input layer
Z1- applying weights to A0 + biases
Activation functions - Tanh, sigmoid, ReLU(if x is negative its 0, ow its x) 
A1 - ReLU applied to Z1
Changes the function from linear makes it more complex
When you move to the second layer, it adds a layer of complexity

From layer 1 to layer 2, similar calc
Z2 = weights to A1 + bias
Activation function - softmax activation function since it is output layer, this gives us the probability.


2) Backwards Propogation -
We start with prediction and subtract the actual labels from them, the remainder is our Cost function

