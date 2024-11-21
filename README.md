# Human Activity Recognition using Kernelized SVM

This project aims to classify human activities using image data and kernelized Support Vector Machines (SVMs). The work explores various feature extraction techniques and preprocessing methods to achieve effective classification.

## Team Members
- Akshet Patial (ECE, IIITD)
- Shivam Kumar (CSE, IIITD)
- Shreeram Kumar Singh (CSE, IIITD)
- Raghav Sakhuja (CSAM, IIITD)
- Harshit Giri (ECE, IIITD)

## Abstract
Human Activity Recognition (HAR) involves analyzing image data to assign labels to specific activities. This project focuses on recognizing 15 distinct activities from labeled images using kernelized SVM. Feature extraction and preprocessing techniques such as HOG, SIFT, LBP, and color histograms were utilized to enhance classification accuracy.

## Data Overview
The dataset contains:
- 15 activity classes (e.g., cycling, running, clapping, etc.)
- 800 images per class, with varying dimensions.

Preprocessing steps included resizing images to uniform dimensions and applying filters such as Sobel, Canny, and Gaussian Blur.

## Key Features
1. **Color Histograms**: Effective for identifying activities with distinct color compositions.
2. **HOG (Histogram of Oriented Gradients)**: Used for edge and gradient detection.
3. **LBP (Local Binary Patterns)**: Captures variations in lighting.
4. **SIFT (Scale-Invariant Feature Transform)**: Identifies robust keypoints.

## Model and Kernels
- Multiple SVM kernels were tested: RBF, Polynomial, Laplacian, Sigmoid, and Chi-Square.
- Final model used PCA for dimensionality reduction and RBF kernel for classification.
- GridSearchCV optimized hyperparameters such as `C=1` and `gamma='scale'`.

## Results
- Achieved a maximum classification accuracy of **35%** using combined features (HOG, LBP, SIFT, and Color Histogram).
- Enhanced feature extraction with VGG16 for improved separability.

## Challenges
- High overlap in the dataset, leading to poor separability in feature space.
- Noise in background and varying image resolutions posed preprocessing difficulties.

## Conclusion
The project highlights the complexities of human activity recognition using image data. While traditional SVM methods demonstrated moderate performance, integrating advanced feature extraction techniques like VGG16 shows promise for future improvements.

## References
A list of references and resources used in the project can be found in the [Report](./Report_GRP7.pdf).

---

