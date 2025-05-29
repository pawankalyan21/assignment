# assignment
1.Tensor Manipulations & Reshaping (TensorFlow)
This mini-project demonstrates how to manipulate tensors in TensorFlow using reshaping, transposing, and broadcasting techniques.
Objective:Perform basic tensor operations using TensorFlow.
Steps:

1. **Create a random tensor** of shape `(4, 6)`.
2. **Print its rank** and **shape** using TensorFlow functions.
3. **Reshape** the tensor into shape `(2, 3, 4)`.
4. **Transpose** it to shape `(3, 2, 4)`.
5. **Broadcast and add** a smaller tensor of shape `(1, 4)` to the larger tensor.
6. **Explain broadcasting** in TensorFlow.
7.
   Expected Output:

- Print the **rank** and **shape** of the tensor before and after reshaping and transposing.
- Print the **final tensor shape** after broadcasting and addition.
-
  Broadcasting in TensorFlow:

Broadcasting is a method TensorFlow uses to perform element-wise operations on tensors of different shapes. TensorFlow automatically **expands dimensions with size `1`** to match the corresponding dimension of the larger tensor, enabling arithmetic operations without explicitly reshaping the smaller tensor.

 How to Run

```bash
python task1_tensor_manipulations.py

output:
       Original Tensor Shape: (4, 6)
Rank: 2
Reshaped Tensor Shape: (2, 3, 4)
Transposed Tensor Shape: (3, 2, 4)
Broadcasted and Added Tensor Shape: (3, 2, 4)



   2. Loss Functions & Hyperparameter Tuning (TensorFlow)

This project demonstrates how to compute and compare two commonly used loss functions in machine learning — Mean Squared Error (MSE) and Categorical Cross-Entropy (CCE). It also shows how slight changes in model predictions affect these loss values.

 Task Overview
Objective:Implement and analyze loss functions in TensorFlow and visualize their behavior using Matplotlib.

 Steps:

1. Define **true labels** (`y_true`) and **predicted outputs** (`y_pred`).
2. Compute:
   - **Mean Squared Error (MSE)**
   - **Categorical Cross-Entropy (CCE)**
3. Slightly change the predictions and **observe how loss values change**.
4. Use **Matplotlib** to plot a **bar chart** comparing the losses for different prediction sets.

Expected Output

- Printed loss values for different predictions.
- A bar chart visualizing and comparing MSE and CCE for each prediction.

 Sample Output

Losses for y_pred_1
MSE: 0.0050
CCE: 0.1625

Losses for y_pred_2
MSE: 0.0533
CCE: 0.5108


3.Train a Neural Network & Log to TensorBoard

This project trains a simple neural network using the MNIST dataset and logs training metrics to TensorBoard for interactive visualization.
 Task Overview

### Objective:
Train a basic feedforward neural network on the MNIST dataset and visualize its performance using **TensorBoard**.

### Steps:

1. **Load and preprocess** the MNIST dataset (normalize pixel values).
2. **Define and compile** a simple neural network using TensorFlow/Keras.
3. Train the model for **5 epochs** while logging metrics to TensorBoard.
4. **Launch TensorBoard** and analyze trends in loss and accuracy over epochs.
Expected Outcome

- The model will train for **5 epochs**.
- Logs will be saved in the `"logs/fit/"` directory.
- TensorBoard will show:
  - 📈 Training vs Validation Accuracy
  - 📉 Training vs Validation Loss

 Directory Structure

├── task3_mnist_training_tensorboard.py
├── logs/
│ └── fit/
└── README.md


Once the training completes, launch TensorBoard:

bash
Copy
Edit
tensorboard --logdir=logs/fit

Then open your browser and go to: http://localhost:6006

