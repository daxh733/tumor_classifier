# Brain Tumor Classification Project

This project aims to classify brain tumors from medical imaging data using a deep learning model. The goal is to accurately identify different types of brain tumors, potentially assisting in medical diagnosis.

## Project Overview

This repository contains the code, trained model, evaluation results, and data source information for a brain tumor classification project. The project involves:

* **Data Preprocessing:** Preparing medical images for training.
* **Model Building:** Developing a convolutional neural network (CNN) using TensorFlow/Keras.
* **Training:** Training the model on a labeled dataset of brain tumor images.
* **Evaluation:** Assessing the model's performance using metrics like accuracy, precision, recall, and F1-score.

## Repository Contents

* **`_results_files/`:** This directory contains visualization files generated during the project, including:
    * `confusion_matrix.png`: A visual representation of the model's classification performance.
    * `accuracy_plot.png`: A plot showing the training and validation accuracy over epochs.
    * Other relevant plots or visualizations.
* **`Data.txt`:** This file contains a link to the dataset used for this project.
* **`Model_1.h5`:** This file is the saved, trained deep learning model in the HDF5 format. It can be loaded and used for making predictions on new brain scan images.
* **`README.md`:** This file (the one you are currently reading) provides an overview of the project and its contents.

## Data Source

The dataset used for training and evaluating this brain tumor classification model can be found at the following link:

[**https://www.kaggle.com/datasets/thomasdubail/brain-tumors-256x256**]

Please refer to the dataset's documentation for details on its structure, licensing, and usage guidelines.

## Model

The trained deep learning model is saved in the `Model_1.h5` file. This model can be loaded using TensorFlow/Keras:

```python
from tensorflow.keras.models import load_model

loaded_model = load_model('Model_1.h5')
