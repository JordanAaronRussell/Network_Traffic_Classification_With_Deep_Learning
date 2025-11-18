# Network Traffic Classification with Deep Learning

This project explores how deep neural networks can classify different types of internet traffic using structured feature data.
The dataset includes seven categories of traffic:

Web Browsing

Chat

Streaming

Email

VoIP

Peer-to-Peer (P2P)

File Transfer (FT)

The notebook demonstrates a complete machine learning workflow—from data preparation to model design, training, evaluation, comparison, and interpretation.

## Project Contents

Network_Traffic_Classification_With_Deep_Learning.ipynb
A full Jupyter notebook containing:

Dataset loading and preparation

Multi-class neural network models

Training with sigmoid vs ReLU activations

Optimiser comparisons (SGD, RMSprop, Adam)

Binary VPN vs Non-VPN classification

Confusion matrices and ROC analysis

Restricted dataset experiments

Complete results summary and conclusion

README.md
This document.

## Project Overview

The goal of this project is to understand how deep learning models behave when classifying different types of internet traffic.
The notebook covers several experiments:

1. Baseline Multi-Class Model

A compact neural network using sigmoid activations and trained with RMSprop.

2. Non-VPN-Only Training

Examines how restricting the dataset impacts generalisation.

3. Optimiser Comparisons

Models trained with:

SGD

RMSprop

Adam

Compared using accuracy curves and confusion matrices.

4. ReLU-Based Models

Deeper architectures trained with ReLU activations to evaluate performance gains over sigmoid.

5. Binary Classification (VPN vs Non-VPN)

A sigmoid output neuron and ROC/AUC evaluation to assess separability.

6. Restricted Traffic Experiments

Models trained only on VPN or only on Non-VPN data to analyse bias, coverage, and generalisation.

## Data Access Note

This project uses a private dataset that cannot be redistributed.
For that reason, the notebook is not fully reproducible, but all code, outputs, results, and evaluations are included for transparency.

## Key Results (Summary)

Baseline models performed well across all seven traffic classes.

ReLU-based models trained with SGD converged more slowly but still produced strong results.

Adam and RMSprop delivered smoother and more stable optimisation compared to SGD.

Binary VPN vs Non-VPN classification achieved high AUC and strong separability.

Models trained only on VPN or only on Non-VPN traffic showed reduced generalisation, highlighting the importance of dataset diversity.

Confusion matrices and precision/recall plots revealed clear differences in class difficulty.

Full analysis is available in the notebook.

## Future Work

Potential improvements include:

Testing convolutional, recurrent, or transformer-style architectures

Applying SHAP/LIME for interpretability

Introducing classical ML baselines (Random Forest, SVM, XGBoost)

Performing hyperparameter tuning (learning rate, batch size, dropout)

Building a live inference demo or API

## About Me

I’m a Data Science graduate focused on machine learning and model development.
This project forms part of my growing machine learning portfolio.
