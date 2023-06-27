# Artificial Intelligence for Energy Optimization in Steel Rolling

This is my master's thesis GitHub repository.

## Master's Thesis Abstract
Wire rod steel rolling is a highly complex metallurgical process involving numerous phases. One of the most critical is the heating phase, where steel billets (semi-finished steel products) undergo various heating treatments in an induction furnace. These heating treatments enable their subsequent shaping and determine the quality of the final product.

This research focuses on introducing a novel methodology that integrates finite element modeling, machine learning, and reinforcement learning to optimize energy consumption during the heating phase of wire rod steel rolling. Specifically, the proposed methodology consists of three major phases. In the first phase, a finite element digital twin of the induction furnace has been developed to accurately simulate the heating process of the billets. In the second phase, two machine learning models based on convolutional and/or recurrent neural networks have been implemented. These models are capable of predicting the temperature profiles of the billets at the induction furnace's exit with satisfactory precision. Finally, in the third phase, a reinforcement learning framework based on deep Q-learning has been proposed to identify heating patterns that reduce the energy consumption of the furnace. 

These goals have been accomplished using real-world data provided by Global Steel Wire, a steelmaker located in Cantabria (Spain). This data mainly comprises multivariate time series related to the instantaneous power of the furnace's inductors and the advance of the billets in the furnace.

## Repository Structure
The structure of this repository is as follows:

* `data`: this folder comprises all the data utilized in this project, encompassing both the raw and preprocessed versions of the data. It also includes the simulations carried out with the finite element model.
* `code` includes all 
