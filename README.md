# Phonics Speech Recognition Using Machine Learning
*A speech recognition project to identify English Phonics using machine learning with MFCC Extraction*


## Table of Contents
1. [Project Overview](#project-overview)
2. [Tech Stack](#tech-stack)
3. [Model Choice and Evaluation](#model-choice-and-evaluation)
6. [Setup and Installation](#setup-and-installation)
7. [Result](#results)

## Project Overview

This project is a phonics speech recognition system that leverages machine learning to classify phonics sounds from audio data. The model was trained on MFCC features extracted from audio recordings and tested on different classification algorithms to identify the most accurate model. The focus was on recognizing phonetic sounds from the English alphabet for educational purposes, particularly aimed at improving language learning.


## Tech Stack

**Programming Language**: Python

**Libraries**:
- scikit-learn 
- librosa 
- joblib 
- numpy 
- pandas 
- matplotlib 

## Model Choice and Evaluation

In the development of this project, I tested three machine learning models to determine the best fit for phonics speech classification:

1. **Support Vector Machine (SVM)**: Best-performing model with the highest accuracy, especially when working with **high-dimensional MFCC features**.
2. **Random Forest (RF)**: A strong performer, but it did not match SVM in terms of accuracy.
3. **K-Nearest Neighbors (KNN)**: Struggled with **high-dimensional data** and performed slower compared to other models.

Ultimately, **SVM** was chosen for its precision and ability to handle the feature complexity in phonics recognition.


## Setup and Installation

To run the project locally, follow these steps:

1. **Clone the Repository**  
   ```bash
   git clone https://github.com/yourusername/phonics-recognition.git
   ```

2. Install Dependencies
   ```
   pip install -r requirements.txt
   ```

3. Prepare the Data
You’ll need to have the phonics audio dataset available. Ensure you have the ``audio files`` and the necessary feature extraction scripts.

## Results

The **SVM model** outperformed **Random Forest** and **K-Nearest Neighbors** in predicting phonics sounds with the highest accuracy. Below are a few visual comparisons between **correct and incorrect predictions**:

- **Correct Prediction**:  
  - **Predicted:** 's'  
  - **Actual:** 's'
  
- **Incorrect Prediction**:  
  - **Predicted:** 'h'  
  - **Actual:** 'b'

![Phonics Prediction Comparison](phonics_comparison.png)

This shows the strength of the **SVM** model in recognizing subtle phonetic differences.




