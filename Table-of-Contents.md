#Table of Contents

#Python Machine Learning

##Table of Contents
*Python Machine Learning
*Credits
*Foreword
*About the Author
*About the Reviewers
*www.PacktPub.com

##Preface
####What this book covers
####What you need for this book
####Who this book is for
####Conventions
####Reader feedback
####Customer support
##1. Giving Computers the Ability to Learn from Data
####Building intelligent machines to transform data into knowledge
####The three different types of machine learning
#####Making predictions about the future with supervised learning
#####Solving interactive problems with reinforcement learning
#####Discovering hidden structures with unsupervised learning
####An introduction to the basic terminology and notations
####A roadmap for building machine learning systems
####Using Python for machine learning
####Summary
##2. Training Machine Learning Algorithms for Classification
Artificial neurons – a brief glimpse into the early history of machine learning
Implementing a perceptron learning algorithm in Python
Adaptive linear neurons and the convergence of learning
Minimizing cost functions with gradient descent
Implementing an Adaptive Linear Neuron in Python
Large scale machine learning and stochastic gradient descent
Summary
3. A Tour of Machine Learning Classifiers Using Scikit-learn
Choosing a classification algorithm
First steps with scikit-learn
Training a perceptron via scikit-learn
Modeling class probabilities via logistic regression
Logistic regression intuition and conditional probabilities
Learning the weights of the logistic cost function
Training a logistic regression model with scikit-learn
Tackling overfitting via regularization
Maximum margin classification with support vector machines
Solving nonlinear problems using a kernel SVM
Decision tree learning
Maximizing information gain – getting the most bang for the buck
Building a decision tree
Combining weak to strong learners via random forests
K-nearest neighbors – a lazy learning algorithm
Summary
4. Building Good Training Sets – Data Preprocessing
Dealing with missing data
Handling categorical data
Partitioning a dataset in training and test sets
Bringing features onto the same scale
Selecting meaningful features
Sparse solutions with L1 regularization
Sequential feature selection algorithms
Assessing feature importance with random forests
Summary
5. Compressing Data via Dimensionality Reduction
Unsupervised dimensionality reduction via principal component analysis
Total and explained variance
Feature transformation
Principal component analysis in scikit-learn
Supervised data compression via linear discriminant analysis
Computing the scatter matrices
Selecting linear discriminants for the new feature subspace
Projecting samples onto the new feature space
LDA via scikit-learn
Using kernel principal component analysis for nonlinear mappings
Kernel functions and the kernel trick
Implementing a kernel principal component analysis in Python
Projecting new data points
Kernel principal component analysis in scikit-learn
Summary
6. Learning Best Practices for Model Evaluation and Hyperparameter Tuning
Streamlining workflows with pipelines
Using k-fold cross-validation to assess model performance
The holdout method
K-fold cross-validation
Debugging algorithms with learning and validation curves
Diagnosing bias and variance problems with learning curves
Addressing overfitting and underfitting with validation curves
Fine-tuning machine learning models via grid search
Looking at different performance evaluation metrics
Reading a confusion matrix
Optimizing the precision and recall of a classification model
Plotting a receiver operating characteristic
The scoring metrics for multiclass classification
Summary
7. Combining Different Models for Ensemble Learning
Learning with ensembles
Implementing a simple majority vote classifier
Evaluating and tuning the ensemble classifier
Bagging – building an ensemble of classifiers from bootstrap samples
Leveraging weak learners via adaptive boosting
Summary
8. Applying Machine Learning to Sentiment Analysis
Obtaining the IMDb movie review dataset
Introducing the bag-of-words model
Transforming words into feature vectors
Assessing word relevancy via term frequency-inverse document frequency
Cleaning text data
Processing documents into tokens
Training a logistic regression model for document classification
Working with bigger data – online algorithms and out-of-core learning
Summary
9. Embedding a Machine Learning Model into a Web Application
Serializing fitted scikit-learn estimators
Setting up a SQLite database for data storage
Developing a web application with Flask
Our first Flask web application
Form validation and rendering
Turning the movie classifier into a web application
Deploying the web application to a public server
Summary
10. Predicting Continuous Target Variables with Regression Analysis
Introducing a simple linear regression model
Exploring the Housing Dataset
Implementing an ordinary least squares linear regression model
Solving regression for regression parameters with gradient descent
Estimating the coefficient of a regression model via scikit-learn
Fitting a robust regression model using RANSAC
Evaluating the performance of linear regression models
Using regularized methods for regression
Turning a linear regression model into a curve – polynomial regression
Modeling nonlinear relationships in the Housing Dataset
Dealing with nonlinear relationships using random forests
Decision tree regression
Random forest regression
Summary
11. Working with Unlabeled Data – Clustering Analysis
Grouping objects by similarity using k-means
K-means++
Hard versus soft clustering
Using the elbow method to find the optimal number of clusters
Quantifying the quality of clustering via silhouette plots
Organizing clusters as a hierarchical tree
Performing hierarchical clustering on a distance matrix
Attaching dendrograms to a heat map
Applying agglomerative clustering via scikit-learn
Locating regions of high density via DBSCAN
Summary
12. Training Artificial Neural Networks for Image Recognition
Modeling complex functions with artificial neural networks
Single-layer neural network recap
Introducing the multi-layer neural network architecture
Activating a neural network via forward propagation
Classifying handwritten digits
Obtaining the MNIST dataset
Implementing a multi-layer perceptron
Training an artificial neural network
Developing your intuition for backpropagation
Debugging neural networks with gradient checking
Convergence in neural networks
Other neural network architectures
A few last words about neural network implementation
Summary
13. Parallelizing Neural Network Training with Theano
Building, compiling, and running expressions with Theano
What is Theano?
First steps with Theano
Configuring Theano
Working with array structures
Wrapping things up – a linear regression example
Choosing activation functions for feedforward neural networks
Logistic function recap
Estimating probabilities in multi-class classification via the softmax function
Broadening the output spectrum by using a hyperbolic tangent
Training neural networks efficiently using Keras
Summary
Index