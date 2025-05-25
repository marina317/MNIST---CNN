# MNIST Digit Classifier with CNN (Keras)

This project implements a simple Convolutional Neural Network (CNN) using Keras to classify handwritten digits from the [MNIST dataset](http://yann.lecun.com/exdb/mnist/).

## 🔧 Model Architecture
- **Input:** 28x28 grayscale images
- **Conv2D:** 32 filters, 5x5 kernel, ReLU activation
- **MaxPooling2D:** 2x2 pool size
- **Conv2D:** 64 filters, 5x5 kernel, ReLU activation
- **MaxPooling2D:** 2x2 pool size
- **Flatten + Dense:** 10 output classes with softmax activation

## 🧪 Dataset
- **Training samples:** 60,000
- **Test samples:** 10,000
- Labels are one-hot encoded.
- Images are normalized to range [0, 1].

## ⚙️ Training
- **Optimizer:** SGD
- **Loss:** Categorical Crossentropy
- **Batch size:** 100
- **Epochs:** 5

## 📈 Results
- Prints the test accuracy after training (~97% with current setup).

## 🚀 How to Run
```bash
pip install keras tensorflow
python mnist_cnn.py
