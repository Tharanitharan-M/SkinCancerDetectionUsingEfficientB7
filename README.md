# Skin Cancer Detection and Classification using Convolutional Neural Networks

## Overview
This project applies deep learning techniques, specifically **Convolutional Neural Networks (CNNs)**, to automate the detection and classification of skin cancer. Using the **EfficientNet-B7** architecture and additional metadata (such as age, anatomical site, and gender), the model assists healthcare professionals in making early and accurate skin cancer diagnoses.

## Key Features
- **Automated Detection**: Capable of detecting and classifying multiple skin cancer types.
- **Base Model**: Utilizes **EfficientNet-B7** for image feature extraction, a state-of-the-art CNN architecture.
- **Incorporation of Metadata**: Uses additional data (age, anatomical site, gender) to improve classification performance.
- **Multi-Class Classification**: Classifies skin lesions into 9 categories.

## Dataset
- **Source**: Kaggle ISIC 2019 Dataset.
- **Total Images**: Approximately 25,000 images.
- **Categories**:
  - Basal Cell Carcinoma
  - Squamous Cell Carcinoma
  - Melanoma
  - Melanocytic Nevus
  - Actinic Keratosis
  - Benign Keratosis
  - Dermatofibroma
  - Vascular Lesion
  - Normal Skin

## Methodology

### Image Preprocessing
- **Image Resizing**: Resized to 380x380 pixels.
- **Data Augmentation**: Includes horizontal and vertical flipping, random rotation.
- **Normalization**: Applied using ImageNet mean and standard deviation values.

### Metadata Preprocessing
- **Label Encoding**: Encoded categorical metadata values.
- **Standardization**: Standardized numerical metadata values to improve model performance.

### Model Architecture
- **Base Model**: **EfficientNet-B7** used for image feature extraction.
- **Custom Architecture**: 
  - CNN for image feature extraction.
  - Sequential network for metadata processing.
  - Combined features for final classification.

## Performance
- **Validation Accuracy**: 84.29%.
- **Low Overfitting**: The model generalizes well to unseen data.
- **Multi-Label Classification**: Capable of classifying images into multiple categories simultaneously.

## Key Contributions
- Demonstrated the effectiveness of combining deep learning with metadata for medical image classification.
- Improved the accuracy of skin cancer detection using advanced CNN techniques.
- Showcased the potential of AI in transforming medical imaging diagnostics.

## Limitations and Future Work
- **Class Imbalances**: Future work will address class imbalances within the dataset.
- **Model Interpretability**: Work will focus on improving the interpretability of the model to assist healthcare professionals in decision-making.
- **Dataset Expansion**: Efforts will be made to expand the diversity of the dataset to better represent real-world scenarios.
- **Clinical Validation**: The model requires further validation in clinical settings to confirm its effectiveness in practical use.

## References
- **World Health Organization**: For providing guidelines on skin cancer classification.
- **ISIC 2019 Dataset**: [Kaggle Link](https://www.kaggle.com/c/isic-2019)
