# Brain-Metastases-Multimodal-project

This repository contains the implementation of a machine learning project that applies Convolutional Neural Networks (CNNs) combined with Multinomial Logistic Regression and autoencoders to classify primary tumor types responsible for brain metastases from MRI scans. The project aims to enhance diagnostic accuracy and provide reliable insights into the origins of brain metastases.

## Description
Brain metastases (BM) significantly impact clinical outcomes in cancer patients, necessitating early and accurate identification for effective treatment planning. This project utilizes a multimodal approach, integrating CNNs for MRI image analysis and Multinomial Logistic Regression (MLR) for clinical data evaluation, to classify the primary tumor types. By incorporating autoencoders for dimensionality reduction, the model improves efficiency and mitigates overfitting, offering a robust tool for precise diagnosis.

## Dataset
The project makes use of the Pretreat-MetsToBrain-Masks dataset, which features MRI scans and clinical history from Yale New Haven Health. This dataset includes multiple imaging modalities such as T1 weighted, T1 post-gadolinium, T2 weighted, and FLAIR sequences. It also provides annotations with manual segmentations of brain metastases. Additionally, the dataset contains extensive clinical data, including demographic information, smoking history, and the presence of extranodal metastasis, among other details.

## Methodology
### Data Preprocessing

- Standardization, normalization, and data augmentation techniques are applied to enhance the quality and variability of the training data. Expert-annotated masks are used to train the segmentation model, ensuring high-quality training labels.
### Model Design and Training

- CNNs are utilized for extracting intricate features from MRI images, while MLR processes clinical data to predict primary tumor types.
- Integrated for dimensionality reduction to optimize model performance and prevent overfitting.
- The model is trained using specific regularization techniques to enhance generalization.
### Evaluation and Validation

- Performance metrics include accuracy, sensitivity, specificity, and additional classification quality indicators.
- Collaboration with oncologists and radiologists to validate the model's effectiveness and practical utility in clinical environments.
