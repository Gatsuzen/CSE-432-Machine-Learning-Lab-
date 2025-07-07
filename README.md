<h1>Image Classification with Convolutional Neural Networks (CNN) on CIFAR-10 🖼️✨</h1>
This repository contains the code and resources for an image classification project using a Convolutional Neural Network (CNN) on the CIFAR-10 dataset.
<br>


<h2>1. Dataset 📊📁</h2>
Source: The CIFAR-10 dataset is a widely used benchmark in computer vision, conveniently available through TensorFlow's Keras API.

Although for the convinience here's the link to the dataset- https://www.cs.toronto.edu/~kriz/cifar.html

-Description: It consists of 60,000 32x32 color images across 10 distinct classes.

-Training Data: 50,000 images (32x32 pixels, 3 color channels).

-Testing Data: 10,000 images (32x32 pixels, 3 color channels).

Classes:

1. airplane ✈️
2. automobile 🚗
3. bird 🐦
4. cat 🐱
5. deer 🦌
6. dog 🐶
7. frog 🐸
8. horse 🐎
9. ship 🚢
10. truck 🚚
<br>

<h2>2. Methodology 🧠⚙️</h2>

Model: A custom-built Convolutional Neural Network (CNN) was designed for this classification task. CNNs are highly effective for image data due to their ability to automatically learn hierarchical features.

Approach:

1. Data Preprocessing: Pixel values of the images were normalized from the range [0, 255] to [0, 1] to aid model convergence.

2. CNN Architecture: The model comprises sequential layers:

   <ul>
1. Multiple Conv2D layers with relu activation for feature extraction.

2. MaxPooling2D layers for downsampling and feature robustness.

3. A Flatten layer to convert 2D feature maps into a 1D vector.

4. Dense (fully connected) layers for high-level pattern recognition.

5. A final Dense layer with softmax activation for multi-class probability prediction.
  </ul>

3. Training: The model was trained for 10 epochs.
   
4. Optimization: The adam optimizer was used, with SparseCategoricalCrossentropy as the loss function and accuracy as the primary metric.

5. Epochs: The model was trained for 10 epochs.
<br>

<h2>3. Technologies 💻🛠️</h2>

1. Python: The primary programming language used for the project.

2. TensorFlow: An open-source machine learning framework used for building and training the neural network.

3. Keras: A high-level API within TensorFlow, used for rapid prototyping and building the CNN model.

4. Matplotlib: A plotting library used for visualizing data samples and the model's training history (accuracy and loss curves).

5. NumPy: A fundamental package for numerical computing in Python, used for array operations.

---
