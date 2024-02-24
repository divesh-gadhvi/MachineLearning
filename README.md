# Speech Emotion Recognition Using MLP Classifier

## Table of Contents
1. [Introduction](#introduction)
2. [Proposed Methodology](#proposed-methodology)
    - [A. Proposed System](#a-proposed-system)
    - [B. Feature Extraction](#b-feature-extraction)
    - [C. Testing and Training Data](#c-testing-and-training-data)
    - [D. Multilayer Perceptron Classifier (MLP)](#d-multilayer-perceptron-classifier-mlp)
    - [E. Music Recommendation](#e-music-recommendation)
3. [Conclusion and Results](#conclusion-and-results)

## Introduction
This project focuses on analyzing emotional speech using the RAVDESS dataset, which consists of audio files with emotional expressions. The dataset contains 24 professional actors vocalizing lexically-matched statements in a neutral North American accent across 8 different emotions. We aim to develop a system that accurately identifies speech emotions through feature extraction and classification.

## Proposed Methodology
### A. Proposed System
We employ an MLP Classifier along with sound file and feature extraction libraries to recognize human emotions accurately from speech data.

### B. Feature Extraction
Feature extraction involves extracting MelFrequency Cepstral Coefficients (MFCCs), Mel spectrograms, and Chroma features from sound files using the 'librosa' library. These features capture spectral characteristics and pitch content, aiding in emotion recognition.

### C. Testing and Training Data
We split the dataset into training and testing sets and use a 75-25 ratio for training and testing, respectively. The MLP Classifier is trained on the training data and evaluated on the testing data for emotion classification.

### D. Multilayer Perceptron Classifier (MLP)
The MLP Classifier is a feedforward artificial neural network capable of learning nonlinear relationships between input and output data. It consists of multiple layers of artificial neurons, including an input layer, one or more hidden layers, and an output layer.

### E. Music Recommendation
Once emotions are predicted, the system utilizes the Spotify API and the 'spotipy' library to recommend music playlists based on the identified emotion.

## Conclusion and Results
Through experimentation, we explored the effect of different parameters on classification accuracy. A lighter CNN design with a 75% training data ratio yielded better results for ten-class classification, achieving an accuracy range of 50%-70%. The deeper CNN model performed well for binary classification tasks. Music playlists were recommended based on predicted emotions using the Spotify API.
