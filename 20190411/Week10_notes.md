# Deep Learning Methods

Guest lecture, Jesse Tetreault, Solutions Architect, NVIDIA

<!-- vim-markdown-toc GFM -->

- [Deep Learning, Machine Learning, and AI](#deep-learning-machine-learning-and-ai)
   - [Artificial Intelligence](#artificial-intelligence)
   - [Machine Learning](#machine-learning)
      - [_Supervised Learning_](#supervised-learning)
      - [_Unsupervised Learning_](#unsupervised-learning)
      - [_Reinforcement Learning_](#reinforcement-learning)
   - [Deep Learning](#deep-learning)
      - [_Uses of DL_](#uses-of-dl)
- [Deep Neural Networks](#deep-neural-networks)
   - [Neural Net Basics](#neural-net-basics)
   - [Alexnet](#alexnet)
   - [Other Types](#other-types)
- [Deep Learning Aproach](#deep-learning-aproach)
   - [1. Training](#1-training)
   - [2. Inference](#2-inference)
- [Convolution](#convolution)

<!-- vim-markdown-toc -->

## Deep Learning, Machine Learning, and AI

### Artificial Intelligence

- Does something that appears to be intelligent
- Doesn't necessarily use data
- Frequently rule based (Think checkers)

### Machine Learning

- A form of AI
- No pre-defined rules
- Learn from data
- More adaptible
- Requires feature engineering, data pre-processing, etc.

#### _Supervised Learning_

- Data where you have the labels
- Can be sudivided into classification or regression

#### _Unsupervised Learning_

- Unlabelled data
- Generally sudivided into clustering or dimension reduction
- Frequently used as a pre-processingv step for supervised learning

#### _Reinforcement Learning_

- There is no data
- Environment, agent, and reward
- Analogous to Pavlov
- The tricky part is designing the correct reward function

### Deep Learning

- A form of AI
- They learn the features and classification
- Can be fed raw, unprocessed data

#### _Uses of DL_

- Detection
- Classification
- Segmentation
- Prediction
- Recommendation
- NLP

## Deep Neural Networks

### Neural Net Basics

1. Input multiplied by weight
1. All inputs sum of crossproduct
1. Passed through activation function
   - This is the key step that allows for non-linear learning
1. Repeat for as many layers as you like

- The end goal is always to achieve linearly separable data.
- Dense layers are better for classifications
- Convolutional for features
- It's very difficult to trace back to identify what features are learned where in what layers (see LIME)

### Alexnet

- The original deep net
- Something like 6 million parameters. Huge at the time, relatively simple today
- Was trained on an imaging dataset. 1 million images, 1 thousand classes

### Other Types

- Convolutional
- Recurrent
- Generative Adversarial Networks - used to generate synthetic data to expand imaging data sets - Ian Goodall
- Reinforcement Learning
- Autoencoder
- Google is working on a model that teaches itself its own architecture - ie you don't do anything but give it data.

## Deep Learning Aproach

### 1. Training

1. Design a loss function
1. Input to output
1. Backpropagate error output to input
   - Deterioration is an issue
   - Partly solved with residual layers
1. Repeat

### 2. Inference

1. Freeze weights and connections
1. Predict

## Convolution

Slide a filter over a data. This encodes a new image/matrix that encodes some feature, say edge detection.

In a neural network, a Convolutional layer gets blank convolutions and learns what they need to be



