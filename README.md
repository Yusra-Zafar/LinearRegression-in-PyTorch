# Simple Linear Regression with PyTorch

## Project Overview

This project aims to build and train a simple linear regression model to predict exam scores based on hours studied. The model is built using PyTorch, a popular deep learning framework.

## Key Libraries Used

- `torch`: For building and training the neural network.
- `torch.nn`: Neural network modules.
- `torch.optim`: Optimization algorithms.
- `numpy`: For numerical operations.
- `matplotlib.pyplot`: For data visualization.

## Code Flow

The notebook follows a structured approach:

1.  **Import Libraries**: Essential libraries are imported.
2.  **Preprocess Data**: Sample `X_train` (hours studied) and `y_train` (exam scores) are defined and converted to PyTorch tensors. A scatter plot visualizes the original data.
3.  **Build Linear Regression Model**: A custom `LinearRegression` class is defined using `nn.Module`, with a single `nn.Linear` layer.
4.  **Pick Loss Function and Optimizer**: Mean Squared Error (`nn.MSELoss`) is chosen as the loss function and Stochastic Gradient Descent (`optim.SGD`) as the optimizer.
5.  **Build Training Loop**: The model is trained over 100 epochs, iteratively performing forward pass, loss calculation, backpropagation, and weight updates. The training loss is plotted over epochs.
6.  **Evaluate Model**: The trained model's performance is evaluated by calculating the Mean Squared Error (MSE) on both the training and a separate test dataset. Visualizations show the fitted line against both training and test data.

## Results

After training, the model achieves:

-   **Training MSE**: 0.3444
-   **Test MSE**: 0.5185

The plots illustrate how the linear model fits the training and test data, providing a visual understanding of its performance.
