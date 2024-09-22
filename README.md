# Seizure Detection Using Machine Learning

## Project Overview
This project focuses on detecting seizures from EEG (electroencephalogram) data using machine learning techniques. The primary goal is to create a reliable model that can classify segments of EEG data as either seizure or non-seizure events.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Data](#data)
- [Modeling](#modeling)
- [Results](#results)

## Installation
To run this project, you'll need to install the necessary libraries. You can create a new Conda environment and install the dependencies using the following commands:

```bash
conda create --name seizure_detection python=3.x
conda activate seizure_detection
pip install -r requirements.txt
```

## Usage

To use the seizure detection model, run the following command in your terminal:

bash
```bash
python main.ipynb
```

## Data

[Dataset](https://www.kaggle.com/datasets/adibadea/chbmitseizuredataset)

## Modeling

This project utilizes a CNN architecture defined as follows:

    Input Layer: Accepts EEG signal data.
    Convolutional Layers: Three Conv1D layers with increasing filter sizes to extract features from the data.
    Pooling Layers: MaxPooling1D layers to reduce dimensionality.
    Dense Layers: A fully connected layer followed by a dropout layer for regularization.
    Output Layer: A dense layer with a softmax activation function to classify between seizure and non-seizure events.


## Results

The model achieved an accuracy of 95% on the test set. The confusion matrix and classification report are as follows:

![confusion Matrix](images/confusion.png?raw=true "confusion Matrix")

![Reciver Operating Charecteristics](images/roc.png?raw=true "Reciver Operating Charecteristics")
