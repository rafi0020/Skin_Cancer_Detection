# Using Computer Vision for Skin Disease Diagnosis in Bangladesh

This repository provides an implementation of a **deep convolutional neural network (DCNN)** for skin disease diagnosis using the HAM10000 dataset. The proposed model enhances **interpretability and transparency** through saliency and attention maps, ensuring better clinical usability.

---

## 📄 Research Paper
**Title**: Using Computer Vision for Skin Disease Diagnosis in Bangladesh Enhancing Interpretability and Transparency in Deep Learning Models for Skin Cancer Classification  
**Authors**: Rafiul Islam, Jihad Khan Dipu, Mehedi Hasan Tusar, et al.   
[Access the Paper Here](https://doi.org/10.48550/arXiv.2501.18161)

---

## 📄 Project Overview

### Motivation
Skin cancer, particularly melanoma, is among the most prevalent cancers globally, with Bangladesh facing a significant shortage of dermatologists. Early detection is crucial for effective treatment, and this project aims to bridge the diagnostic gap using computer vision and deep learning techniques.

### Objectives
1. Develop a DCNN for classifying benign and malignant skin lesions.
2. Enhance interpretability using saliency and attention maps.
3. Compare the performance of the proposed model with existing transfer learning models like AlexNet, ResNet, VGG16, DenseNet, and MobileNet.

---

## 📊 Dataset

### HAM10000 Dataset
- **Source**: Publicly available HAM10000 dataset containing 10,015 dermoscopy images.
- **Classes**:
  - **Benign Lesions**: 6,705 images.
  - **Malignant Lesions**: 1,113 images.
- **Dataset Preparation**:
  - Noise and artifacts removed using preprocessing techniques.
  - Data augmentation applied to address class imbalance.

### Example Data Format:
| Image ID       | Diagnosis       | Benign/Malignant |
|----------------|-----------------|------------------|
| ![image](https://github.com/user-attachments/assets/10b14bdf-845c-4fd4-9a07-fcc4dddca9f9)| Melanocytic Nevi| Benign           |
| ![image](https://github.com/user-attachments/assets/9668e464-08cc-4a5f-8d7d-b7bfac3d80bf)| Melanoma        | Malignant        |

---

## 🚀 Methodology

### Key Steps:
1. **Preprocessing**:
   - Noise removal using Gaussian and median blurring.
   - Normalization and artifact elimination.
2. **Data Augmentation**:
   - Techniques: Rotation, cropping, mirroring, zooming, and color-shifting.
3. **Proposed Model**:
   - A DCNN with additional layers tailored for skin lesion classification.
   - Trained using the Adam optimizer and evaluated with a sigmoid activation for binary classification.
4. **Evaluation Metrics**:
   - Accuracy, Precision, Recall, F1-score, and AUC.

---

## 🔧 Getting Started

1. **Download the Repository**
   - Access the repository files from GitHub and save them locally.

2. **Install Dependencies**
   - Use the `requirements.txt` file to set up your Python environment.

3. **Prepare the Dataset**
   - Download the HAM10000 dataset and follow the `data/README.md` instructions to prepare it.

4. **Run the Notebook**
   - Use the `Skin_Cancer_Detection.ipynb` notebook to train and evaluate the model.

---

## 📊 Results

### Performance of Proposed DCNN Model:
- **Training Accuracy**: 96.57%
- **Testing Accuracy**: 93.16%
- **Comparison with Other Models**:
  - **DenseNet**: 90.31% Testing Accuracy
  - **MobileNet**: 88.26% Testing Accuracy
  - **Proposed DCNN**: Achieved higher accuracy and reduced execution time.

---

## 🤝 Contributions
Contributions are welcome! Open an issue or submit a pull request for suggestions or improvements.

---

## 📫 Contact
- **Email**: rafiulislam1921@gmail.com  
- **LinkedIn**: [Rafiul Islam](https://www.linkedin.com/in/rafi009)

---

## 📄 License
This repository is licensed under the Apache 2.0 License. See `LICENSE` for more details.
