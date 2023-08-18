# Image-classification(cat, dog)

  This notebook based on Deep Learing/CNN.

A Convolutional Neural Network(CNN) is a Deep Learning algorithm which can take in an input image, assign importance (learnable weights and biases) to various aspects/objects in the image and be able to differentiate one from the other. The pre-processing required in a Cnn is much lower as compared to other classification algorithms. While in primitive methods filters are hand-engineered, with enough training, Cnn have the ability to learn these filters/characteristics.

# Import Libraries & Layers

Layers - Conv2D, MaxPooling2D, Dropout, Flatten, Dense

# Datasets

  There are two type of dataset. Datasets contains set of images of cats & dogs. 

  # Define dimensions of images and create a model

        1.Here we create a sequential model.

        2. Here we create the first layer by calling the .add() function on the model we created and pass the type of layer we want — a Conv2D layer. This first layer is called the input layer.

        3.activation [‘relu’]: We select an activation function also called non-linearity to be used by our neural network.

        4.Here we add a MaxPool2D layer. Its function is to reduce the spatial size of the incoming features and therefore helps reduce the number of parameters and computation in the network, thereby helping to reduce overfitting.

        5.Here we add a Flatten layer. A conv2D layers extract and learn spatial features which are then passed to a dense layer after it has been flattened. This is the work of the flatten layer.

        6.Here we add a Dropout layer with value 0.5. Dropout randomly drops some layers in a neural networks and then learns with the reduced network.0.5 means to randomly drop half of the layers.

        7.The last layer has an output size of 1 and a different activation function called sigmoid.The sigmoid is perfect for this because it takes in a set of numbers and returns a probability distribution in the range of 0 to 1.Sigmoid function at the end because we have just two classes.

# Compile and train the model

  We pass parameters to the model.compile() command.

         Loss [‘binary_crossentropy’]

         Optimizer: rmsprop

 # Making New Predictions.

   correct prediction made

        Binary classification is the task of classifying the elements of a set into two groups on the basis of a classification rule. I used simple Convolutional Neural Network and the accuracy i got is 81%.


        Thank You.
        
       
