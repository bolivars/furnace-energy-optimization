# Artificial Intelligence for Energy Optimization in Steel Rolling
This is my master's thesis GitHub repository.

## Introduction
Wire rod steel rolling is a highly complex metallurgical process involving numerous phases. One of the most critical is the heating phase, where steel billets (semi-finished steel products) undergo various heating treatments in an induction furnace. These heating treatments enable their subsequent shaping and determine the quality of the final product.

This research focuses on introducing a novel methodology that integrates finite element modeling, machine learning, and reinforcement learning to optimize energy consumption during the heating phase of wire rod steel rolling. Specifically, the proposed methodology consists of three major phases. In the first phase, a finite element digital twin of the induction furnace has been developed to accurately simulate the heating process of the billets. In the second phase, two machine learning models based on convolutional and/or recurrent neural networks have been implemented. These models are capable of predicting the temperature profiles of the billets at the induction furnace's exit with satisfactory precision. Finally, in the third phase, a reinforcement learning framework based on deep Q-learning has been proposed to identify heating patterns that reduce the energy consumption of the furnace. 

These goals have been accomplished using real-world data provided by Global Steel Wire, a steelmaker located in Cantabria (Spain). This data mainly comprises multivariate time series related to the instantaneous power of the furnace's inductors and the advance of the billets in the furnace.

## Repository Structure
The structure of this repository is as follows:

* `data`: this folder includes all the data utilized in this project, encompassing both the raw and preprocessed versions of the data.
  
* `code`: this folder includes all the scripts developed for this project. It specifically consists of the following subdirectories:

    - `1-preprocessing`: this directory contains the scripts used for data preprocessing.

    - `2-finite-element-model`: this directory includes the script developed in PyMAPDL that implements the finite element model and performs simulations. It also includes scripts (along with some summary datasets) that allow comparing the simulations with temperature profiles recorded by the outlet pyrometer.

    - `3-machine-learning-models`: this directory contains the scripts that implement machine learning models based on neural networks, namely, the one-dimensional convolutional and convolutional-recurrent models. Additionally, it contains the obtained models in HDF5 format and some of the graphs used in the thesis.

    - `4-energy-optimization`: this directory includes everything related to the RL framework. In particular, it includes the script used for training the agent (DQN), the obtained models, as well as some graphs used in the thesis. It also includes the scripts where the learnt decision-making policy is applied to the heating patterns of billets currently used by GSW.

* `requirements.txt`: this file lists all packages and Python libraries on which the various notebooks depend. It provides an overview of the required dependencies for running the notebooks successfully. By setting up an environment with these packages, ensuring they match the specified versions, you will be able to run the code without encountering any issues.
