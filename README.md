# Solving_a_basic_computer_vision_problem

 Let's take a look at a scenario where we can recognize different items of clothing,
 trained from a dataset containing 10 different types.

# Model Layers of our Neural Network

Sequential:  Defines a SEQUENCE of layers in the neural network

Flatten: Flatten just takes that square of images and turns it into a 1 dimensional set.

Dense: Adds a layer of neurons

Each layer of neurons need an activation function to tell them what to do. There's lots of options, but just use these for now.

Relu effectively means "If X>0 return X, else return 0" -- so what it does it it only passes values 0 or greater to the next layer in the network.

Softmax takes a set of values, and effectively picks the biggest one, so, for example, if the output of the last layer looks
like [0.1, 0.1, 0.05, 0.1, 9.5, 0.1, 0.05, 0.05, 0.05], it saves you from fishing through it looking for the biggest value, 
and turns it into [0,0,0,0,1,0,0,0,0] -- The goal is to save a lot of coding!


# Training the neural network

Once it's done training -- we should see an accuracy value at the end of the final epoch. It might look something like
0.9098. This tells us that our neural network is about 91% accurate in classifying the training data. i.e, 
it figured out a pattern match between the image and the labels that worked 91% of the time


![](/imgs/image1.png)


![](/imgs/image2.png)


![](/imgs/image3.png)


![](/imgs/image4.png)


