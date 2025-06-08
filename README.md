# DL_Project: Action Recognition in Tennis with ST-GCN and MMAction2
This repository contains 3 different notebooks `.ipynb`, one where the keypoints are extracted and must be the first to run, another two regarding to the two types of training methods implemented.
The project covers the full workflow: data preparation, label mapping, model training, inference, and evaluation with confusion matrix visualization.

Additionally, the repository includes two PDF documents:

- A poster created to serve as a project presentation during a poster session, which is part of the course evaluation.

- A final report corresponding to the written documentation of the project.

This repository contains three Jupyter notebooks (`.ipynb`):

1. `extract_keypoints.ipynb` → **Keypoint Extraction**  
   Extracts pose keypoints from tennis videos using MediaPipe.  
   **This notebook must be run first**, as it generates the data required for the subsequent steps.
   
2. `train_type1.ipynb` → **Training Method 1: Full Network Training**  
   Trains the ST-GCN model from scratch or with all layers unfrozen, allowing the entire network to adapt to the tennis action recognition task using the MMAction2 library.

3. `train_type2.ipynb` → **Training Method 2: Single-Layer Fine-Tuning**  
   Fine-tunes only the final layer(s) of the pre-trained ST-GCN model while keeping earlier layers frozen, focusing adaptation on the classification head for tennis actions with MMAction2.

---

## Project Overview

This project covers the full workflow for action recognition in tennis videos:

- **Data preparation:** Extraction and organization of keypoints.
- **Label mapping:** Assigning numerical labels to each action class.
- **Model training:** Training ST-GCN models with MMAction2.
- **Inference:** Generating predictions on test data.
- **Evaluation:** Visualizing performance with confusion matrices.

---

## How to Use

1. **Run the keypoint extraction notebook first** to generate the required data files.
2. **Choose and run one of the training notebooks** according to the method you wish to test.
3. **Evaluate the results** using the provided evaluation cells, which include confusion matrix visualization.

---

## Dependencies

All required Python packages and versions are specified within each notebook.

You will need:
- Python 3.x
- PyTorch
- MMAction2 and its dependencies
- MediaPipe
- scikit-learn
- matplotlib, seaborn, numpy

---

## Results

After training and evaluation, the notebooks provide performance metrics and confusion matrix plots to help analyze the model's classification accuracy.

---

## License

This project is licensed under the terms of the [MIT License](LICENSE).  
See the LICENSE file for details.[1][5][9]

---

## Authors

- Diana Santos (64478)  
- Leonor Fandinga (64481)  
- Sofia Rocha (65111)


---

## Acknowledgements

- This project was inspired by the MMAction2 library and the OpenMMLab ecosystem.
- Special thanks to the MediaPipe team for their robust pose estimation tools.
- Thanks to the open-source machine learning community for templates and best practices.
- The tennis action recognition experiments are based on the [THETIS (Three dimEnsional TennIs Shots) dataset](https://github.com/THETIS-dataset/dataset), a comprehensive 3D tennis action dataset captured with Kinect, consisting of 8374 video sequences from 55 subjects (31 beginners and 24 experts) covering 12 different tennis actions[1][2][5].
- For more information about the THETIS dataset and its structure, visit the [official GitHub repository](https://github.com/THETIS-dataset) or consult the [original publication (CVPR 2013)](https://openaccess.thecvf.com/content_cvpr_workshops_2013/W08/papers/Gourgari_THETIS_Three_Dimensional_2013_CVPR_paper.pdf).

---

## References

- MMAction2 Documentation: https://mmaction2.readthedocs.io/
- MediaPipe Pose: https://google.github.io/mediapipe/solutions/pose
- PyTorch: https://pytorch.org/
- Scikit-learn: https://scikit-learn.org/
- THETIS Dataset GitHub: https://github.com/THETIS-dataset/dataset
- THETIS Dataset Paper: https://openaccess.thecvf.com/content_cvpr_workshops_2013/W08/papers/Gourgari_THETIS_Three_Dimensional_2013_CVPR_paper.pdf
