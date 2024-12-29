# NYBG Image Classification Model

This repository contains the machine learning model developed for the New York Botanical Garden (NYBG) Kaggle competition, as part of the Spring 2024 AI Studio program by Break Through Tech AI. The model classifies plant specimen images into distinct categories, enabling researchers to filter out non-standard images and curate usable datasets for biodiversity research.

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Model](#model)
- [Installation](#installation)
- [Usage](#usage)

## Overview

The NYBG challenge involves classifying images into categories such as:
- **Animal specimens** (non-standard)
- **Biocultural specimens** (non-standard)
- **Microscope slides** (non-standard)
- **Ordinary pressed specimens** (standard)

This project supports global biodiversity studies by automating the filtering of non-standard images, saving researchers significant time and effort.

## Dataset

The dataset used for training and testing the model is provided by NYBG via Kaggle. It contains a diverse set of images representing the above categories. [Learn more about the dataset here](https://www.kaggle.com/competitions/bttai-nybg-2024/data).

## Model

The model employs a convolutional neural network (CNN) architecture, fine-tuned for multi-class image classification. Key features include:
- High accuracy in distinguishing between standard and non-standard images.
- Scalability for deployment in real-world scenarios.

The main model implementation and troubleshooting steps can be found in the Jupyter notebook: [`model-troubleshooting.ipynb`](model-troubleshooting.ipynb).

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/felicengie/NYBG-Machine-Learning.git
   cd NYBG-Machine-Learning
   ```

2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

To train the model:
```bash
python train.py
```

To evaluate the model:
```bash
python evaluate.py
```

To use the trained model for predictions:
```bash
python predict.py --input <path_to_image>
```
