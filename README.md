# DL_Project
This repository contains 3 different notebooks .ipynb, one where the keypoints are extracted and must be the first to run, another two regarding to the two types of training methods implemented.
The project covers the full workflow: data preparation, label mapping, model training, inference, and evaluation with confusion matrix visualization.

This repository contains three Jupyter notebooks (.ipynb):

1. Keypoint Extraction:
Extracts pose keypoints from tennis videos using MediaPipe. This notebook must be run first, as it generates the data required for the subsequent steps.

2. Training Methods:
Implements two different training strategies for action recognition using the ST-GCN model with the MMAction2 library. Each notebook explores a different fine-tuning or training approach.

Project Overview
This project covers the full workflow for action recognition in tennis videos:

Data preparation: Extraction and organization of keypoints.

Label mapping: Assigning numerical labels to each action class.

Model training: Training ST-GCN models with MMAction2.

Inference: Generating predictions on test data.

Evaluation: Visualizing performance with confusion matrices.

How to Use
Run the keypoint extraction notebook first to generate the required data files.

Choose and run one of the training notebooks according to the method you wish to test.

Evaluate the results using the provided evaluation cells, which include confusion matrix visualization.

Dependencies
All required Python packages and versions are specified within each notebook.
You will need:

Python 3.x

PyTorch

MMAction2 and its dependencies

MediaPipe

scikit-learn

matplotlib, seaborn, numpy

Results
After training and evaluation, the notebooks provide performance metrics and confusion matrix plots to help analyze the model's classification accuracy.
