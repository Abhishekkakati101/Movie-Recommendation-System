# Movie-Recommendation-System

<p align = 'center' height ='500px' weidth ='200'>
<img src ='https://github.com/Abhishekkakati101/Movie-Recommendation-System/blob/main/Assets/boltz.PNG'>
</p>

Movie Recommendation System uses the Restricted Boltzmann Machine model to recommend either the customer would like the movie on the basis of ratings and reviews.



The restricted Boltzmann machine (RBM) is a probabilistic model that uses a layer of hidden binary
variables or units to model the distribution of a visible layer of variables. It has been successfully applied to problems involving high dimensional data such as images and text. In this context, two approaches are usually followed. First, an RBM is trained in an unsupervised manner to model the distribution of the inputs (possibly more than one RBM could be trained,
stacking them on top of each other. Then, the RBM is used in one of two
ways: either its hidden layer is used to preprocess the input data by replacing it with the representation given by the hidden layer, or the parameters of the RBM are used to initialize a feedforward
neural network. In both cases, the RBM is paired with some other learning algorithm (the classifier
using the preprocessed inputs or the neural network) to solve the supervised learning problem at
hand. This approach unfortunately requires one to tune both sets of hyper-parameters (those of the
RBM and of the other learning algorithm) at the same time. Moreover, since the RBM is trained in
an unsupervised manner, it is blind to the nature of the supervised task that needs to be solved and
provides no guarantees that the information extracted by its hidden layer will be useful.

