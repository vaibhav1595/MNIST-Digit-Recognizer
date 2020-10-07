# MNIST-Digit-Recognizer

<p align="center"><img width="500" height="250" src="https://neurohive.io/wp-content/uploads/2019/05/Screenshot-from-2019-05-29-21-23-47.png"></p>

- Developed a Convolutional Neural Network to Classify Handwritten Digits with an accuracy of **99.12%**
- Engineered the training, validation (15% of training set) and test datasets into 28 x 28 x 1 pixels
- Performed pixel normalization to make the model learn better (from [0,255] to [0,1])
- Generated Sequential Model with 3 Convolutional Blocks, each block consists of 2 Conv2D layers with LeakyRelU activation layers, then the MaxPool2D layer (to reduce the size of the image), and finally the Dropout layer (to drop the few activation nodes while training). And then, after the flatten layer, the dense layers and a Output layer with sigmoid activation were formed
- Compiled the model by selecting Adam as an Optimizer, and sparse_categorical_crossentropy as a loss fucntion (because target values are integer not one-hot vector)
