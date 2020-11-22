# Backpropagation-SoftMax

# nn_modules.py
- Linear neural network module
  - Implement a Linear module with fprop and bprop functions
  - Module which implements a linear layer
  - initialize the parameters
  - feed-forward propagation 
  - backpropagation

- Softmax Implementation
  - Implement a SoftMax module with fprop and bprop functions

- Cross Entropy Loss Function Implementation
  - Implement a CrossEntropy module with fprop and bprop functions

- Tanh acitivation function Implementation
  - Implement module a Tanh acitivation function

- Log Cross Entropy Loss Function Implementation
  - Implement Log-Cross-Entropy-Loss

- Log Softmax Implementation
  - Implement Log-Softmax-Module
  
# model.py :
- Model providing functionality for training and testing a generic stack of NNModules
  - Initialize all modules
  - Run forward-propagation through the entire module stack
  - Backpropagation through the complete module stack
  - Run parameter update step for all model parameters
  - Run initialization for all the modules
  
  
# Side Node:
Download the dataset from the following URL: https://omnomnom.vision.rwth-aachen.de/data/mnist.tgz.

In the Training loop is using the following network architecture: Linear(28 ∗ 28; 10), SoftMax and the CrossEntropy criterion. Run the training for 100 epochs using a learning-rate λ = 0:1 and a batch-size of 600 and you should reach 750 errors on the validation-set.

# Hint:
Without mini-batching,it needs to reduce the learning-rate to λ = 0:01 to avoid numerical problems.


You may play with more difficult datasets by downloading CIFAR10 and CIFAR100 from the following URLs:
- https://omnomnom.vision.rwth-aachen.de/data/cifar10.tgz
- https://omnomnom.vision.rwth-aachen.de/data/cifar100.tgz


Train a deeper network on the MNIST dataset. For example, the following network architecture: Linear(28 ∗ 28; 200), Tanh, Linear(200; 10), SoftMax should get you
down to about 290 errors on the validation-set.
