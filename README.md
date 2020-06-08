# Spider-Species-Recognition-Using-Convolutional-Neural-Network

Problem Statement:
	Recognizing species of spider using Convolutional Neural Network.

Images:
Training set: Redback spider: 396 images, Tarantula spider: 1059 images
Testing set: Redback spider: 99 images, Tarantula spider: 268 images

Convolutional Neural Network:
A Convolutional Neural Network (CNN) architecture has three main parts:
1.	A convolutional layer that extracts features from a source image. Convolution helps with blurring, sharpening, edge detection,     noise reduction, or other operations that can help the machine to learn specific characteristics of an image.
2.	A pooling layer that reduces the image dimensionality without losing important features or patterns.
3.	A fully connected layer also known as the dense layer, in which the results of the convolutional layers are fed through one or more neural layers to generate a prediction.
4.	In between the convolutional layer and the fully connected layer, there is a ‘Flatten’ layer. Flattening transforms a two-dimensional matrix of features into a vector that can be fed into a fully connected neural network classifier.

Steps:
1.	Import the required libraries from keras package.
2.	The first Convolutional layer uses 64 nodes, while the second uses 32, and ‘kernel’ or filter size for both is 3 squared pixels.
3.	Create the first Convolutional layer and pooling layer.
4.	Create a second convolutional layer and pooling layer.
5.	Then create a Flattening layer and finally a Fully Connected layer.
6.	Then we will Compile Convolutional Neural Network  providing three parameters:
•	Optimizer – use the ‘adam’ optimize which adjusts learning rate throughout training .
•	Loss function – use a ‘binary_crossentropy’ loss function.
•	Metrics – use the ‘accuracy’ metric to get an accuracy score when the model runs on the validation set.
7.	Then we will Fit Convolutional Neural Network to Images of different species of spiders.
8.	Then we will define the training and testing set of images.
9.	Then we will Train the model using the keras fit() function, providing the training data, target data, and the number of epochs the experiment should run (the number of times training should be repeated on the data).
10.	Before predicting we will check the indices for each species.
11.	Then we will predict the species of spider by feeding it with a new image that is not used for training.

Conclusion:
	The above model recognizes both the species of spider properly even if a new image is fed with an accuracy of (99%).
