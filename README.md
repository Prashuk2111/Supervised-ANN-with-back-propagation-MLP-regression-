# Supervised-ANN-with-back-propagation-MLP-regression

Using a feedforward back-propagation neural network that contains a single hidden layer (with a
variable number of hidden nodes each having an activation function of the logistic form), investigate
the outcome of the neural network for the following mappings:

𝑓1(𝑥) = 𝑥 ∗ sin(6𝜋𝑥) ∗ exp(−𝑥2) 𝑤ℎ𝑒𝑟𝑒 𝑥 ∈ [−1, 1]
𝑓2(𝑥) = exp(−𝑥2) ∗ arctan(𝑥) ∗ sin(4𝜋𝑥) 𝑤ℎ𝑒𝑟𝑒 𝑥 ∈ [−2, 2]

For each function, create three sets of input/output data, one for training and validation and one
for testing. These will be random values within the interval of the variable x). You can choose the
ratio as 80% of the data for training (including validation) and 20% of the data for testing. We will
use 10- fold cross validation approach, which means that the training set will be divided into 90%
training and 10% for validation.

a: We need to create a 4 by 4 grid of 16 models assessments for each function. Each model
𝑀𝑖,𝑗 (i, j th entry of the grid) has i as number of data set (training and testing) and j as the number
of hidden nodes in the neural network model. i takes the following values: i = {10, 40,80,200}data
points, while j takes the following values: j = {2,10, 40,100} hidden nodes. For each 𝑀𝑖,𝑗, apply 10-
fold cross validation (and repeat the process 5 times by shuffling the data generated randomly) and
get error average for training and validation. For each model and each 10-fold cross validation, use
early stopping criteria to make sure the validation error and the training error are both small and to
avoid overfitting. Please see lecture slides on model selection and K-fold cross validation. Generate
a grid (table) with entries corresponding to each model 𝑀𝑖,𝑗 , where the entries have the best
training and validation errors obtained for that model (using early stopping criteria).

b: Make qualitative and quantitative deductions in light of these simulations and find
the best model that has acceptable bias (complex enough model) and an acceptable variance (no
overfitting). Apply the full training data set to this model, and then apply the testing data (which the
system never saw and draw the original functions and the best model obtained through neural
network prediction.
