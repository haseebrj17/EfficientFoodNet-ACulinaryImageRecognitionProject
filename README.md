---

# EfficientFoodNet: Culinary Image Recognition

## Overview
"EfficientFoodNet" is a deep learning project focused on classifying images of food into various categories. Utilizing TensorFlow, Keras, and the pre-trained EfficientNetB0 model, this project demonstrates the power of convolutional neural networks (CNNs) in computer vision tasks.

## Project Description
The project employs the EfficientNetB0 architecture, a state-of-the-art CNN from TensorFlow's model garden. This model is known for its efficiency and high accuracy in image classification tasks. The network is used as a feature extractor where the top layer is replaced with a new classifier tailored for our specific task — recognizing different types of food.

### Data Preparation and Augmentation
The dataset consists of images from 10 food categories, each represented by a small subset of training examples. To mitigate overfitting due to the small size of the dataset, extensive data augmentation techniques such as random flipping, rotation, zooming, and height/width shifting are applied.

### Model Training and Evaluation
Two main experiments are conducted:
1. **Model 0**: A transfer learning model using EfficientNetB0 with its weights frozen, trained on 10% of the data.
2. **Model 1 and Model 2**: These models include the data augmentation pipeline within the model itself, allowing for more dynamic learning. They are trained on 1% and 10% of the data, respectively.

Each model's performance is evaluated based on its accuracy and the loss during training and validation phases. Additionally, fine-tuning is applied to the last few layers of the base model to further enhance the model's ability to generalize.

### Tools and Libraries Used
- TensorFlow and Keras for building and training the neural network.
- Matplotlib for visualization of the data and results.
- Pandas for data manipulation and analysis.
- Google Colab for a cloud-based development environment, ensuring access to high-performance computing resources.

## Conclusion
"EfficientFoodNet" demonstrates a robust approach to food image classification, highlighting the effectiveness of transfer learning combined with real-time data augmentation. The project outlines methodologies that can be adapted to similar image recognition tasks within the culinary domain or beyond.

---
