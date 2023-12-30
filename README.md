# Temperature-Prediction
Example data for Fahrenheit to Celsius temperature conversion is provided, with two sets of data: one containing 10 entries and the other containing 100 entries. These datasets are embedded within the program. The goal is to use 1) linear regression and 2) Multilayer Perceptron (MLP) with Backpropagation (BP) learning rules to identify the formula for converting Fahrenheit to Celsius.

Given the straightforward nature of the Fahrenheit to Celsius temperature conversion, it is anticipated to use a neural network architecture such as 1-N-1 or 1-N-N-1, where N represents the number of neurons in the hidden layer. The value of N can be chosen from the set {10, 20, 30, 40, 100}.

## Lab 1-1
Using the first set of example code, employ the linear regression method to determine the formula for converting Fahrenheit to Celsius temperatures.

## Lab 1-2
Using the second set of examples, with N being 10, 20, 30, 40, or 100, employ the MLP (Multilayer Perceptron) with BP (Backpropagation) method to learn a neural network for converting Fahrenheit to Celsius temperatures. Display the parameters of the model and compare the differences between different parameter values.

### Testing
Randomly test 5 sets of Fahrenheit temperatures and compare the merits and drawbacks of the two methods.

### Modification
- Through testing data, it can be observed whether the current training is overfitting. If the accuracy on the training data is high and the loss is low, it may appear that the training results are good. However, when actual testing reveals poor performance, incorporating test data to evaluate accuracy and loss becomes crucial. If the test data shows low accuracy and poor loss, it indicates that the current model is only familiar with the training data.
- When the loss is very low but the accuracy is also low, adjusting the batch size may be helpful. If the batch size is reduced, it is noticeable that the training time increases significantly. For instance, with 1000 data points, training 100 samples per batch for 10 iterations completes the training, whereas training 10 samples per batch requires 100 iterations to complete. Although the model has seen more data in the latter case, accuracy tends to improve. However, there's a possibility that with a too-small batch size, the model may not capture the relevance of the data, resulting in lower accuracy and poor loss. Therefore, adjusting the batch size requires careful attention and experimentation.
