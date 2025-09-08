# Age Estimation Based on Human Voice

This project uses machine learning to estimate a person's age group based on features extracted from their voice. The core of this project is a Jupyter Notebook (`Age Estimation based on Human Voice.ipynb`) that walks through the data preprocessing, feature extraction, model training, and evaluation steps.



## Overview

The goal of this project is to build and train a model that can predict an individual's age by analyzing their speech. We extract various acoustic features from audio clips and use them to train a classifier to distinguish between different age brackets (e.g., teens, twenties, thirties, etc.).

---

## Dataset

The model was trained on the **Common Voice Dataset** by Mozilla. This is a large, publicly available dataset of voice samples. For this project, we specifically used the age and gender labels to train our model.

You can access the dataset here: [Mozilla Common Voice](https://commonvoice.mozilla.org/en/datasets)

---

## Features

To classify the audio files, we extracted several key acoustic features from the raw audio signals. The primary features used are:

* **Mel-Frequency Cepstral Coefficients (MFCCs):** These coefficients represent the short-term power spectrum of a sound and are widely used in audio processing.
* **Chroma Features:** These represent the tonal content of the audio.
* **Mel Spectrogram:** A spectrogram where the frequencies are converted to the mel scale.
* **Zero-Crossing Rate:** The rate at which the signal changes from positive to zero to negative.
* **Pitch (Fundamental Frequency):** The perceived lowness or highness of a tone.

---

## Model

This project implements a **Convolutional Neural Network (CNN)** for the classification task. CNNs are highly effective at finding patterns in data like spectrograms. The model architecture consists of several convolutional layers, pooling layers, and dense layers to learn the relationship between the audio features and the corresponding age groups.

---

## Installation

To run this project, you'll need to have Python 3 installed. You can clone the repository and install the necessary dependencies using `pip`.

```bash
# Clone the repository
git clone [https://github.com/SaiNihal2622/Age-Estimation-based-on-Human-Voice.git](https://github.com/SaiNihal2622/Age-Estimation-based-on-Human-Voice.git)
cd Age-Estimation-based-on-Human-Voice

# Install the required libraries
pip install -r requirements.txt
