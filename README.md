# Deep Knowledge Tracing with AWS Neuron

This repository implements Deep Knowledge Tracing (DKT) using PyTorch and AWS Inferentia2 for efficient inference on SageMaker.

## Overview

Deep Knowledge Tracing is a machine learning method that models student knowledge over time. This implementation uses AWS Neuron SDK for optimized inference on AWS Inferentia2 accelerators.

In this repository, [ASSISTment2009](https://sites.google.com/site/assistmentsdata/home/assistment-2009-2010-data) "skill-builder" dataset are used. You need to download the dataset on the following path:

```
datasets/ASSIST2009/
```

## Features

- Implementation of DKT model using PyTorch
- AWS Neuron optimization for Inferentia2
- Support for ASSIST2009 dataset
- Real-time inference monitoring

## Requirements

- Python 3.8+
- PyTorch 1.12+
- torch-neuronx
- numpy
- pandas
- scikit-learn

## Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/dkt-neuronx.git
cd dkt-neuronx
```

## Usage
run `dkt_model.ipynb` or `dkt_model_ko.ipynb`(Korean) on SageMaker Notebook instance (inf2 or trn1).

## Model Architecture

The DKT model uses LSTM to trace student knowledge states:
- Input embedding layer
- LSTM layer
- Output layer with sigmoid activation

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.