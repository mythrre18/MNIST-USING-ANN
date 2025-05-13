MNIST Digit Classification using Neural Networks
this projects uses deep learning to classify the input from the [MNIST dataset](http://yann.lecun.com/exdb/mnist/) into (0-9) digits.

Project Overview
*Dataset: 70,000 grayscale images of handwritten digits (0–9)
* Task: Multi-class classification (10 classes)
* Framework: TensorFlow + Keras +  matplot
* Model: Feedforward Neural Network with one hidden layer

Model Architecture

| Layer Type | Details                                 |
| ---------- | --------------------------------------- |
| Flatten    | Converts 28x28 images to 784-dim vector |
| Dense      | 128 units, ReLU activation              |
| Dense      | 10 units, Softmax activation            |

Optimizer: Adam
Loss Function: Categorical Crossentropy
Metrics: Accuracy
Epochs: 10
Batch Size: 32
initializer:HeNormal
 Results

| Dataset    | Accuracy |
| ---------- | -------- |
| Validation | \~97.8%    |
| Test       | \~97.6%    |


How to Run
# Step 1: Install dependencies
pip install tensorflow scikit-learn matplotlib

# Step 2: Run the script
python mnist.py

Sample Output

313/313 ━━━━━━━━━━━━━━━━━━━━ 2s 5ms/step - accuracy: 0.9728 - loss: 0.1009
Test accuracy: 0.9769

Key Concepts Covered

* Data preprocessing & normalization
* Train-validation-test split
* Categorical encoding of labels
* Model training and evaluation
* Simple model architecture for MNIST

Files
 `mnist.py`: Main script for training and evaluation

Credits
* [TensorFlow MNIST docs](https://www.tensorflow.org/datasets/catalog/mnist)
* Developed using Google Colab




