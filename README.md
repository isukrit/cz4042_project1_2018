# CZ4042 Project 1, Classification and Regression (2018)
Project 1 material with starter codes and dataset for students taking Prof. Jagath Rajapakse's course CZ4042 (Neural Networks and Deep Learning) for undergraduates at SCSE, NTU. 

LandSat satellite dataset from: https://archive.ics.uci.edu/ml/datasets/Statlog+(Landsat+Satellite)
California Housing Dataset from: http://www.dcc.fc.up.pt/~ltorgo/Regression/cal_housing.html

Project description can be found in the file project1.pdf

FAQs:

1) Do you prefer any particular Python library for coding? Are there any penalty/extra marks for any library? 

Answer: To simply answer your question, 'no', we don't favor any particular library while marking the assignments. You can use any of Tensorflow/Theano/Pytorch or any other Python library. Project 1 involves simple neural network models and it is a great opportunity for you to learn to build neural networks using these libraries. You will learn something new and you can use this knowledge to build complex neural network models. You will have to use the above mentioned libraries for Project 2, anyway.

2) Do I need to build the network manually or is it fine if I use higher level API like Keras?

Answer: We would prefer that you build the network manually. Although, using higher level APIs is easier and it gets the job done (as well), but it usually leaves you with an incomplete understanding of the working of the different neural network layers, the relationship between their outputs and inputs, their weights, etc. 

3) It's stated that we need to use 5-fold cross-validation in part B, but, it's not stated how we should choose the output from the 5 models? Should we average the error from each of k folds or choose the output corresponding to the best fold?

Answer: You should take the average of the k folds. To understand why, consider the scenario where you divided the data for training and validation in such a way that the validation data contained 'simpler' samples and therefore may be easier to predict (which will give you a high validation accuracy/low error). To avoid this, you evaluate the model on all the folds, basically all the training data by using k-fold CV. 

