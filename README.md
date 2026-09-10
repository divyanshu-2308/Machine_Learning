🔢 Handwritten Digit Recognition from Scratch

A neural network built from scratch using Python and NumPy to recognize handwritten digits from the MNIST dataset.

The main purpose of this project is to understand how a neural network actually learns — by implementing the core concepts manually instead of relying on deep-learning frameworks such as TensorFlow or PyTorch.

⸻

📌 Overview

The model takes an image of a handwritten digit as input and predicts which digit it represents.

Handwritten Image → Neural Network → Prediction (0–9)

MNIST is a classic dataset for image classification consisting of grayscale images of handwritten digits.

* Classes: 10 (0–9)
* Image size: 28 × 28
* Input features: 784 pixels
* Task: Multi-class classification

⸻

🧠 How It Works

Each 28 × 28 image is converted into numerical data and passed through the neural network.

The training process follows the basic neural-network learning cycle:

Input Image
    ↓
Preprocessing
    ↓
Forward Propagation
    ↓
Prediction
    ↓
Loss Calculation
    ↓
Backpropagation
    ↓
Gradient Calculation
    ↓
Parameter Update
    ↓
Repeat

Forward Propagation

Each layer performs a linear transformation followed by an activation function:

Z = W·X + b
A = activation(Z)

where:

* X → input/features
* W → weights
* b → bias
* Z → weighted input
* A → activation/output

Backpropagation

After calculating the loss, gradients are propagated backward through the network.

The parameters are then updated using gradient descent:

W = W - η(dW)
b = b - η(db)

where η represents the learning rate.

By repeating this process, the network gradually learns patterns that distinguish one handwritten digit from another.

⸻

✨ Features

* Neural network implementation from scratch
* MNIST image preprocessing
* Forward propagation
* Activation functions
* Loss calculation
* Backpropagation
* Gradient-based parameter updates
* Handwritten digit classification
* Model evaluation and prediction

⸻

🛠️ Tech Stack

Technology	Purpose
Python	Core programming language
NumPy	Numerical operations and neural-network calculations
Matplotlib	Data and prediction visualization
Jupyter Notebook	Development and experimentation
MNIST	Handwritten digit dataset

The core neural-network logic is implemented manually rather than using a pre-built TensorFlow or PyTorch model.

⸻

📂 Project Structure

Digit_Recognition/
│
├── digit.ipynb
│   └── Neural network implementation, training and testing
│
├── mnist-png/
│   └── MNIST dataset
│
└── README.md
    └── Project documentation

⸻

🚀 Getting Started

1. Clone the repository

git clone https://github.com/divyanshu-2308/Machine_Learning.git

2. Navigate to the project

cd Machine_Learning/Digit_Recognition

3. Install the required packages

pip install numpy matplotlib jupyter

4. Start Jupyter Notebook

jupyter notebook

Open digit.ipynb and run the cells sequentially.

⸻

📈 Model Training

During training, the network repeatedly:

1. Performs forward propagation
2. Generates predictions
3. Calculates the loss
4. Computes gradients using backpropagation
5. Updates weights and biases
6. Repeats the process on the training data

The goal is to minimize the loss while improving the model’s ability to correctly classify unseen handwritten digits.

⸻

🎯 Prediction

Once trained, the model can classify an input image into one of ten possible classes:

Input
  ↓
┌─────────────────────┐
│   Neural Network    │
└─────────────────────┘
  ↓
[0 1 2 3 4 5 6 7 8 9]
  ↓
Predicted Digit

⸻

💡 What I Learned

This project helped me develop a deeper understanding of:

* How neural networks process data
* How images are represented numerically
* Weights and biases
* Activation functions
* Forward propagation
* Loss functions
* Gradient descent
* Backpropagation
* Parameter optimization
* Multi-class classification

Building these components manually helped me understand what happens behind the abstractions provided by modern deep-learning frameworks.

⸻

🔮 Future Improvements

* Experiment with different network architectures
* Compare different activation functions
* Experiment with optimizers
* Add training loss and accuracy graphs
* Test on custom handwritten images
* Build an interactive digit-drawing interface
* Compare the implementation with TensorFlow/PyTorch
* Deploy the trained model as a web application

⸻

👨‍💻 Author

Divyanshu Shekhar

GitHub — @divyanshu-2308

⸻

⭐ Like the Project?

If you found this project useful or interesting, consider giving the repository a ⭐.