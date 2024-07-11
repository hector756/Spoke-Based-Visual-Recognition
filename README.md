# Spoke-Based-Visual-Recognition
Classifying images is a complex problem in the field of computer vision. Training a deep learning model is computationally expensive and time consuming. It is often tackled by using convolutional neural networks (CNNs). However, for privacy concerns, sending complete images for classification is undesirable. The project proposes a method for multiclass image classification by generating a 1D array representation of an image using a subset of pixels sampled via the Bressenham's Line Algorithm.

To visualize spokes, a file Spoke Visualizer is also provided along with image on which it is created.

It involves data pre-processing, convolutional neural network creation and training it over newly created dataset. Data augmentation and regularization techniques are used reduce problem of overfitting. For demonstration purpose datasets like SVHN and CIFAR10 have been used. Most part in code about what that part it does is mentioned alongside in svhn.ipynb file. Similar operations have been performed too on CIFAR10 dataset.

Without using any hyper-parameter tuning method (like grid search), the above method produces 88.39% accuracy in SVHN dataset and 68.57% accuracy in CIFAR10 dataset. One can implement grid search for improved accuracy.

Dataset:

SVHN dataset: This dataset can be accessed from svhn_data folder via the below G-drive link. It contains image data and their labels in form of numpy arrays.
CIFAR10: This dataset can be easily loaded from keras.datasets from Tensorflow library.
Link for SVHN dataset: https://drive.google.com/drive/folders/1UvoPyBupHa9e4YbZsVHwKu_ijeUw_oV4?usp=sharing
