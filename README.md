# tensor_flow_digit_mnist
📌 MNIST Handwritten Digit Classifier – MLP This project implements a Multi-Layer Perceptron (MLP) model to classify handwritten digits from the MNIST dataset. The model is built using TensorFlow/Keras and trained on 60,000 images of digits (0–9), achieving high accuracy on the test set of 10,000 images.
Here’s your **GitHub description** updated with your optimized parameters:


This project implements a **Multi-Layer Perceptron (MLP)** model to classify handwritten digits from the [MNIST dataset](http://yann.lecun.com/exdb/mnist/). The model is built using **TensorFlow/Keras** and trained on 60,000 images of digits (0–9), achieving high accuracy on the test set of 10,000 images.

### 🔹 Features

* **Two fully connected hidden layers** (`n_hidden_1=256`, `n_hidden_2=128`) for rich feature learning
* **Adam optimizer** with `learning_rate=0.002` for faster convergence
* Configurable `training_steps`, `batch_size`, and progress logging
* Uses **ReLU** activation for hidden layers and **Softmax** for output
* Normalizes pixel values to `[0, 1]` for efficient training
* Achieves **>95% accuracy** on MNIST test set

### 🔹 Parameters Used

```python
learning_rate = 0.002       # Slightly higher for faster convergence
training_steps = 8000       # ~25 epochs with batch_size=128
batch_size = 128            # Smaller batch helps generalization
display_step = 200          # Log less frequently

n_hidden_1 = 256            # Increase first layer for richer features
n_hidden_2 = 128            # Smaller second layer to reduce overfitting
```

### 🔹 Dataset

* **Source**: TensorFlow/Keras `mnist` dataset
* **Shape**: 28x28 grayscale images
* **Classes**: 10 (digits 0–9)


