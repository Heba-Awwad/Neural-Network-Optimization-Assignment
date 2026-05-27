# Neural-Network-Optimization-Assignment
Neural Network Optimization

<img width="934" height="181" alt="image" src="https://github.com/user-attachments/assets/6a92899a-b1b3-4299-a4f0-cdfff5e3b56b" />







Figure shows a neural network with one hidden layer, the input layer, and the output layer. α∗ is the matrix of weights from the inputs to the hidden layer and β∗ is the matrix of weights from the hidden layer to the output layer. α∗j,i represents the weight going to the node zj in the hidden layer from the node xi in the input layer, and β∗ is defined similarly. We will use a ReLU activation function for the hidden layer and a softmax for the output layer. The bias vectors αb, βb are defined such that the jth value of αb (which we denote αj,b) is the bias value for aj and the kth value of βb is the bias value for bk.
Write a program to fit your neural network, then answer the following questions. For these questions, use the small dataset given in your Moodle course page (small_train.csv and small_validation.csv) and the following values for the hyperparameters unless otherwise specified:

<img width="470" height="172" alt="image" src="https://github.com/user-attachments/assets/d88750e1-c3aa-4d3a-ae23-8d0600701f63" />

1.
Hidden Units: Train a single hidden layer neural network using the hyperparameters mentioned in the table above, except for the number of hidden units which should vary among 5, 20, 50, 100, and 200. Run the optimization for 100 epochs each time.
1.1.
Plot the average training cross-entropy (sum of the cross-entropy terms over the training dataset divided by the total number of training examples) of the final epoch on the y-axis vs number of hidden units on the x-axis. In the same figure, plot the average validation cross-entropy. The x-axis should be the number of hidden units, the y-axis should be average cross-entropy loss, and there should be one curve for validation loss and one curve for train loss.
1.2.
Examine and comment on the plots of training and validation cross-entropy. What problem arises with too few hidden units, and why does it happen?
2.
Weight Initialization:
2.1.
Initialize α and β to zero and print them out after the first few updates.
2.2.
Compare the values across rows and columns in α and β. Describe the observed behavior and explain why this may happen
3.
Adding a Hidden Layer: Now, try adding another hidden layer to your neural network. The hyperparameters for the model should be the same as the table above, except for learning rate. The 2 hidden layers should both have a dimension of 50, and your learning rate should be 0.003. Run the optimization for 100 epochs. Remember that adding another hidden layer means you should add both a linear layer and a sigmoid layer in your code.
3.1.
We want to compare the performance of this model with our 1 hidden layer model. So, create a plot with the following 4 lines. Plot the average training and validation cross-entropy loss for a 1 hidden layer model, using the same learning rate of 0.003 and a hidden dimension of 50. Additionally, plot the average training and validation cross-entropy loss for the 2 hidden layer model on the same figure. The x-axis should be epoch number, the y-axis should be average cross-entropy loss, and there should be
four total curves: training loss and validation loss for the 1 hidden layer model, and training loss and validation loss for the 2 hidden layer model.
3.2.
Examine and comment on the difference in performance between the two model. What happens when you add an additional hidden layer? Why do you think this is happening? Frame your answer in terms of model complexity and overfitting/underfitting.
4.
Activation Function: Train two single hidden layer neural networks, one using a ReLU activation function and another using a sigmoid activation function on the hidden layer. The single hidden layer in the two models should both have a dimension of 50, and your learning rate should be 0.003. Run the optimization for 100 epochs.
4.1.
Compare the convergence of the two models by plotting the following 4 lines on the same graph. Plot the average training and validation cross-entropy loss for the model with a ReLU activation and the model with a sigmoid activation.
4.2.
Examine and comment on the difference in convergence between the two models. Which activation function allows the model to converge faster and why?
5.
Adding a Hidden Layer and Activation Function: Now, try adding another hidden layer to both of the above neural networks. The hyperparameters for the models should be the same as above, and one neutral network should use ReLU and another should use sigmoid as their activation functions. Remember that adding another hidden layer means you should add both a linear layer and a ReLU/sigmoid layer in your code.
5.1.
Plot the average training and validation cross-entropy loss for the model with a ReLU activation and the model with a sigmoid activation.
5.2.
Examine and comment on the difference in convergence between the two models (the 1-hidden-layer model vs the 2-hidden-layer model) across both activation functions. Did this effect become more or less or equally as severe as the number of hidden layers increases?
