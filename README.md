# Integration of Neural Network-Based Symbolic Regression in Deep Learning for Scientific Discovery

This repository is the official PyTorch implementation of the EQL network described in
[Integration of Neural Network-Based Symbolic Regression in Deep Learning for Scientific Discovery](https://arxiv.org/abs/1912.04825)

Symbolic regression, in which a model discovers an analytical equation describing a dataset as opposed to finding 
the weights of pre-defined features, is normally implemented using genetic programming.
Here, we demonstrate symbolic regression using neural networks,
which allows symbolic regression to be performed using gradient-based optimization techniques,
i.e., backpropagation.
It can be integrated with other deep learning architectures, allowing for end-to-end training of a system that produces
interpretable and generalizable results. 

This repository implements symbolic regression with neural networks using PyTorch.
The TensorFlow 1 version can be found at [this repository](https://github.com/samuelkim314/DeepSymReg),
which also implements the experiments found in the above paper.

## Requirements

* Python 3
* PyTorch
* NumPy
* Scipy
* Sympy
* Matplotlib (optional)

All dependencies are in [requirements.txt](requirements.txt). 
To install required packages, you can simply run the following code in your shell.
```
pip install -r requirements.txt
```

### Quick Start

Run
```batch
python benchmark_accuracy_l12.py
```
or
```batch
python benchmark_accuracy_l0.py
```
to test the symbolic regression network on various synthetic benchmarking tests. 
The two commands implement the architecture using smoothed L0.5 and relaxed L0 regularization, respectively.

### Authors
Samuel Kim, Ileana Rugina, Amber Li

### Contributing
If you'd like to contribute, or have any suggestions for these guidelines, 
you can contact Samuel Kim at samkim (at) mit (dot) edu or open an issue on this GitHub repository.

All content in this repository is licensed under the MIT license.