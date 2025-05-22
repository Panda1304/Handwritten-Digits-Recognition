# 🧠 Handwritten Digits Recognition

This project implements a Convolutional Neural Network (CNN) using TensorFlow and Keras to recognize handwritten digits from the MNIST dataset. The model achieves high accuracy and can predict digits from custom images.

## 📌 Overview

The goal of this project is to build a deep learning model capable of classifying handwritten digits (0-9) with high accuracy. The model is trained on the MNIST dataset and can also predict digits from external images.

## 📊 Dataset

The [MNIST dataset](https://en.wikipedia.org/wiki/MNIST_database) is a large database of handwritten digits commonly used for training image processing systems. It contains:

- 🖼️ 60,000 training images
- 🧪 10,000 testing images
- 🔳 Each image is a 28x28 grayscale image of a single digit

## 🏗️ Model Architecture

The CNN model is built using Keras' Sequential API and consists of the following layers:

1. 🧩 Convolutional Layer with ReLU activation
2. 🌀 MaxPooling Layer
3. 🚿 Dropout Layer
4. 📦 Flatten Layer
5. 🔢 Dense Layer with ReLU activation
6. 🚿 Dropout Layer
7. 🎯 Output Dense Layer with Softmax activation

🧠 The model is compiled with the Adam optimizer and categorical crossentropy loss function.

## 💾 Installation

1. *Clone the repository:*

   bash
   git clone https://github.com/Panda1304/Handwritten-Digits-Recognition.git
   cd Handwritten-Digits-Recognition
   

2. *Install the required packages:*

   bash
   pip install -r requirements.txt
   

## ⚙️ Usage

### 🏋️‍♂️ Training the Model

To train the model on the MNIST dataset:

bash
python tf_cnn.py


💾 This will train the model and save it as tf-cnn-model.h5.

### 🔍 Predicting External Images

To predict a digit from an external image:

bash
python load_model.py <path_to_image>


For example:

bash
python load_model.py assets/images/1a.jpg


📌 Ensure that the image is a clear, 28x28 grayscale image of a single digit for optimal results.

## 📈 Results

The trained model achieves an accuracy of over *99%* on the MNIST test dataset. Below is an example of the model's prediction:

![Result](result.png)

## 📝 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
