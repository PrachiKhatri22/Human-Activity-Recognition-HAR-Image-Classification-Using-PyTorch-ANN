# Human-Activity-Recognition-HAR-Image-Classification-Using-PyTorch-ANN

## Overview
This project is aimed at classifying images into three categories: Catch, Clap, and Hammering. The model is built using a neural network (NN) classifier with early stopping to prevent overfitting and improve generalization. The dataset is split into training and testing sets, with transformations applied to resize images to 64x64 pixels and convert them to tensors. The model is trained using a cross-entropy loss function and an SGD optimizer.

## Technologies Used 
- Python 3.x
- PyTorch
- NumPy
- Matplotlib

## Dataset
The dataset consists of images from three categories:

- Catch
- Clap
- Hammering

These images are organized into folders for training and testing. The training data is used to train the neural network, while the testing data is used to evaluate the model's performance.

## Output
<img width="219" alt="image" src="https://github.com/user-attachments/assets/29b0b222-a85c-4593-b609-756dc2aacf2c" />


## Key Features
- Image Preprocessing: Images are resized to 64x64 pixels and converted into tensor format for model input.
- Early Stopping: The EarlyStoppingCriterion class monitors validation loss, and the training process is stopped early if no improvement is observed over a specified number of epochs (patience).
- Model Architecture: The model consists of several fully connected layers with ReLU activation and batch normalization.
- Training and Testing: The training process includes calculating the training loss, training accuracy, and test accuracy. Results are plotted to visualize the model's performance.


## Data Preparation
The images are resized to 64x64 pixels, and the pixel values are normalized. The dataset is split into training and testing sets with an 80-20 ratio using the splitfolders library.

## Model Architecture
The model is a fully connected neural network with the following layers:

- Input Layer: Linear transformation to 1024 units
- Hidden Layers: 4 fully connected layers with ReLU activation and batch normalization
- Output Layer: A linear layer with 3 units (one for each class)

## Output:
<img width="605" alt="image" src="https://github.com/user-attachments/assets/ba6f38eb-0c42-4ece-9e24-ae755df31acb" />


## Early Stopping
An early stopping mechanism is implemented to prevent overfitting. If the validation loss does not improve for a specified number of epochs (patience), the training stops early.

## Training and Testing
The model is trained for a maximum of 10 epochs. The training loss and accuracy are printed at the end of each epoch, along with the test accuracy.
The early stopping mechanism will stop the training once the validation loss stops improving.

<img width="531" alt="image" src="https://github.com/user-attachments/assets/da93c3c6-be68-4909-9d29-96343a4bf424" />

## Visualizations
The training and test accuracy, as well as the training loss, are plotted after the training process completes.

## Results
Sample results from the training:

## Plotting and Visualizing the performance:
Displays the training loss per epoch.

## Epoch-wise Training Loss & Accuracy
![image](https://github.com/user-attachments/assets/e0094bc3-e05f-43cb-9b5d-b697e4e1ed49)

## Results
The model achieved a training accuracy of 96.83% and a test accuracy of 96.88%, with the test accuracy slightly exceeding the training accuracy. This can be attributed to the use of regularization techniques like early stopping, which helped prevent overfitting and allowed the model to generalize better to the test set. Overall, the model performs well, demonstrating robust generalization and effective image classification.



