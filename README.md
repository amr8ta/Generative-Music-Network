# Generative Music Network

## Introduction
It is often said that music transcends geographical boundaries and language barriers, a form of expression that is both methodical and laced with emotion. It is a reflection of an artist’s creative and technical ingenuity. With our project, we aim to use machine learning algorithms to attempt to quantify, computationally assess and imitate this timeless medium of art and expression.

The first part of our project deals with the classification of audio samples into genres using audio features extracted from .wav files. With this, we compare the performance of two models– a K- nearest neighbour classifier (K-NN) classifier, and a convolutional neural network (CNN).

The second part involves building a generative model using an LSTM network architecture to produce music. With this segment of our project, we investigate two questions

1. How musically sound and meaningful is the composition of the generated audio samples?
2. What is the extent of the influence of the characteristics of the training data on the music it generates vis-à-vis its genre?

## Data
We used the GTZAN dataset for our project. It consists of 1000 audio tracks, each 30 seconds long. It is a collection of 10 genres, each represented by 100 tracks. The tracks are all 22050 Hz Mono 16-bit audio files in . wav format. It is the most-used public dataset for evaluation in machine listening research for music genre recognition (MGR).

## Model Evaluation
### Methodology
A key parameter to be considered while evaluating the output of our generative model was musical aesthetic. Further, we were interested in assessing how well characteristics of the training dataset were reflected in the music generated vis-à-vis its genre.

To address both of these points, our approach to evaluate the model was to conduct a survey using six of our generated audio samples. We asked the 32 respondents to assign an appropriate genre to each sample and to rate it on a scale from 1 to 10, where

- a 1 rating would mean "no shape or detail; completely random noise"
- a 5 rating would mean "musically plausible"
- a 10 rating would mean "expressive, idiomatic musical shaping and detail"

### Performance Analysis
Overall, the samples received an average rating of **6.17 ± 2.30**.

Additionally, **32.81%** of the respondents’ assigned genre to audio samples corresponded to the genre of its respective training data, with the highest being **78.1%** for Sample 4 (hip hop) and the lowest being **3.1%** for Sample 5 (rock), indicating that the training data’s characteristics has a perceptible influence on its generated audio sample.
