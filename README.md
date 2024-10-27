# Cotton Disease Detection Using CNN

This project uses a Convolutional Neural Network (CNN) to detect various diseases in cotton plants by analyzing leaf images. It aims to help farmers and agricultural experts identify and respond to cotton diseases quickly.

## Dataset
The dataset includes images of cotton leaves affected by different diseases, organized into three folders:
- **train/**: for training the model
- **val/**: for validating the model
- **test/**: for evaluating the model's performance

## Data Preprocessing
Data preprocessing involves:
- Rescaling pixel values to be between 0 and 1
- Applying augmentations like rotation, width shift, and brightness changes to make the model more robust

## Model Architecture
The CNN model consists of:
- Several convolutional layers followed by max pooling
- Flattening the output
- Dense layers for classification


## Transfer Learning with VGG16
In addition to the custom model, transfer learning is applied using the VGG16 model. The VGG16 model is modified to classify our specific disease classes.

## Training the Model
The model is trained with:
- Early stopping to avoid overfitting
- Categorical crossentropy loss function
- Adam optimizer
- Metrics monitored: accuracy

## Results
After training, the model's loss and accuracy for both training and validation sets are plotted to visualize performance.

## Evaluation
The model is evaluated on the test dataset to check its accuracy and other performance metrics.

## How to Use
To use the model for predicting cotton leaf diseases:
1. Load the trained model.
2. Preprocess the new image.
3. Use the model to predict the disease class.

## Conclusion
This project demonstrates how deep learning can be used to identify diseases in crops effectively. By leveraging CNNs and transfer learning, we can create a reliable tool for farmers to monitor and manage crop health.
