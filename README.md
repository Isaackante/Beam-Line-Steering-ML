Overview 

Description: The goal of this project aims to use a neural network to model and optimize beam steering in the Linac to Undulator (LTU) section of the LCLS to minimize beam offsets at the BPMs. 
The neural network will represent a function mapping the following inputs to the output beam

Inputs:

● Quadrupole magnet strengths (k1, k2, ..., kN)
● Corrector magnet settings (c1, c2, ..., cM)
● Beam energy (E)
Output:
● Beam position monitor (BPM) offsets (x1, x2, ..., xP)

Model Architecture:

MyModel is a neural network implemented in PyTorch for a regression task. The model architecture is designed with multiple hidden layers to capture complex patterns in the input data. The network consists of fully connected (linear) layers with Rectified Linear Unit (ReLU) activation functions between them.

Training:

The model is trained using the mean squared error (MSE) loss function. The training process includes a custom training step, validation step, and validation epoch end functions to monitor the training progress. The training_step and validation_step functions compute the loss for each batch, and validation_epoch_end calculates the average loss for the entire validation set. During training, the model reports the mean squared error (MSE) loss and the root mean squared error (RMSE) loss at the end of each epoch.

Model Performance: 

After training the MyModel neural network, it's important to assess its performance on unseen data to ensure its generalization ability. The model evaluation metrics used for this regression task are Mean Absolute Error (MAE), Mean Squared Error (MSE), and Root Mean Squared Error (RMSE). MAE represents the average absolute difference between the predicted and true values. MSE measures the average squared difference between predicted and true values. RMSE is the square root of the MSE and provides a measure of the average magnitude of the errors. These evaluation metrics provide a comprehensive view of how well the model is performing on the test or validation set. When interpreting these metrics, consider the scale of your target variable to understand the practical implications of the errors.

Maintainer: Isaac Kante 
Email: Isaackante@gmail.com 
LinkedIn: www.linkedin.com/in/isaac-kante-474b48204
