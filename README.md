# Permutation-Learning-Technex
WHAT IS PERMUTATION LEARNING ?

Permutation learning is a type of machine learning that involves shuffling the order of data points to help the model learn underlying patterns in the data regardless of their order. It's useful in tasks where the order of the data is not relevant or when the order is arbitrary.
. For example, if we have a sequence of letters "ABCDEF", we can generate permutations of this sequence such as "DEFABC" or "BCDAEF". By training a model on these shuffled sequences, we can ensure that the model can recognize the same patterns in any order, regardless of the original sequence.

EXPLANATION OF THE PROJECT :

Given a randomly arranged 6*6 puzzle, we train Machine Learning Models that can solve the Puzzle by predicting the correct permutation of pieces
First, we load images from given dataset, divide each image into 36 puzzle pieces, and returns a numpy array of all the puzzle pieces for all the images in the input DataFrame.

We then create a 36x36 numpy array to one-hot encode the puzzle pieces and their positions. Each row represents a puzzle piece and each column represents a position. If a puzzle piece is in the correct position, its corresponding element in label is set to 1, otherwise it's set to 0.

Finally, we train a Convolutional Neural Network with the  preprocessed data
