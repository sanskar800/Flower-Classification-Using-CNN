Project Summary:
This project aims to classify flower images into five categories (daisy, dandelion, rose, sunflower,
tulip) using deep learning techniques. I developed and compared multiple Convolutional Neural
Network (CNN) models, including a baseline model, a deeper model with regularization, and a
transfer learning approach using VGG16. The dataset, consisting of approximately 3,550 training
images, was preprocessed with data augmentation and normalization. The baseline model achieved
a test accuracy of 0.70, while the deeper model improved this to 0.79 through regularization
techniques like L2, Batch Normalization, and Dropout. Training with SGD and Adam optimizers
showed Adam converging faster with higher accuracy (0.79 vs. 0.74). Transfer learning with
VGG16 significantly outperformed all models, achieving a test accuracy of 0.89. Key findings
include the effectiveness of pre-trained models in reducing class confusion (e.g., rose-tulip) and
the trade-offs between computational cost and performance. Future work includes experimenting
with other pre-trained models and collecting more diverse data to further improve accuracy.

Dataset:
The dataset used in this project is a custom flower image dataset with five classes: daisy, dandelion,
rose, sunflower, and tulip. It contains approximately 3,582 training images, with the following
class distribution: lily (~617), lotus (~905), orchid (~637), sunflower (~586), and tulip (~837). The
test set includes 700 images (140 per class). Images were resized to 180x180 pixels for scratch
models and 224x224 for transfer learning with VGG16. Preprocessing steps included
