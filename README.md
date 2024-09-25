# Melanoma Detection Using Custom CNN
> A convolutional neural network-based solution to detect melanoma and other skin cancer types from images, aiming to assist dermatologists with early detection and diagnosis.

## Table of Contents
* [General Information](#general-information)
* [Conclusions](#conclusions)
* [Technologies Used](#technologies-used)
* [Acknowledgements](#acknowledgements)
* [Contact](#contact)

## General Information
- This project focuses on developing a deep learning-based model to classify images of skin cancer into nine different categories, including melanoma, which accounts for 75% of skin cancer deaths.
- **Business Problem**: Early detection of melanoma is critical, and a solution that can automate image classification can assist dermatologists in making quicker, more accurate diagnoses, potentially saving lives.
- **Dataset**: The dataset used is derived from the International Skin Imaging Collaboration (ISIC) and contains 2357 images classified into 9 categories:
  - Actinic keratosis
  - Basal cell carcinoma
  - Dermatofibroma
  - Melanoma
  - Nevus
  - Pigmented benign keratosis
  - Seborrheic keratosis
  - Squamous cell carcinoma
  - Vascular lesion

## Conclusions
- **Initial Model**: The initial CNN model trained on the original dataset showed signs of overfitting, as the validation accuracy was much lower than training accuracy.
- **Data Augmentation**: Applying data augmentation techniques (random flip, rotation, zoom) helped reduce overfitting by generating more varied training images.
- **Class Imbalance**: An analysis of the class distribution showed an imbalance, with some classes having significantly fewer samples. This was addressed using the `Augmentor` library to balance the dataset.
- **Final Model**: After handling class imbalance and applying augmentation, the model's performance improved, achieving better generalization on the validation set.

## Technologies Used
- Python - 3.7
- TensorFlow - 2.6
- Keras - 2.6
- Augmentor - 0.2.8
- Matplotlib - 3.4.3
- Numpy - 1.21.2

## Acknowledgements
- This project was inspired by the International Skin Imaging Collaboration (ISIC) and their efforts to standardize skin cancer imaging data.
- The project framework was built based on [this tutorial](https://www.tensorflow.org/tutorials/images/classification).
- Special thanks to open-source contributors of the TensorFlow, Keras, and Augmentor libraries.

## Contact
Created by [@SMRizwanFaisal](https://github.com/SMRizwanFaisal) - feel free to reach out!
