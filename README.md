# MNIST Handwritten Digit Classification using TensorFlow

## Project Overview

This project implements a machine learning model to recognize and classify handwritten digits (0–9) using the MNIST dataset. A feedforward neural network was developed with TensorFlow/Keras to learn patterns from grayscale images and accurately predict the corresponding digit.

The project demonstrates the complete machine learning workflow, including data loading, preprocessing, model development, training, and performance evaluation.

---

## Dataset

The project uses the **MNIST Handwritten Digits** dataset, which contains grayscale images of handwritten digits.

* **Training Images:** 60,000
* **Testing Images:** 10,000
* **Image Size:** 28 × 28 pixels
* **Classes:** 10 (Digits 0–9)

Dataset Source:

* https://www.kaggle.com/datasets/hojjatk/mnist-dataset

---

## Technologies Used

* Python
* TensorFlow / Keras
* NumPy
* Matplotlib
* scikit-learn
* idx2numpy

---

## Data Preprocessing

The following preprocessing steps were performed before training the model:

* Loaded the original MNIST `.idx` files.
* Normalized pixel values from **0–255** to **0–1**.
* Flattened each 28 × 28 image into a 784-dimensional feature vector.
* Split the dataset into training and testing sets using the provided MNIST data.

---

## Model Architecture

The neural network consists of:

* Input Layer: 784 features
* Hidden Layer 1: 128 neurons (ReLU activation)
* Hidden Layer 2: 64 neurons (ReLU activation)
* Output Layer: 10 neurons (logits)

The model was trained using:

* Optimizer: Adam
* Loss Function: Sparse Categorical Crossentropy (`from_logits=True`)
* Evaluation Metric: Accuracy

---

## Results

The trained model was evaluated on the MNIST test dataset.

**Performance Metrics**

* Test Accuracy: **95%** *(Update this value with your final result if it changes.)*
* Confusion Matrix
* Precision
* Recall
* F1-Score

---

## Project Structure

```text
MNIST-Digit-Classifier/
│
├── MNISTDigitRecognition.ipynb
├── README.md
├── requirements.txt
├── .gitignore
└── dataset/
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/MNIST-Digit-Classifier.git
```

Navigate to the project directory:

```bash
cd MNIST-Digit-Classifier
```

Install the required libraries:

```bash
pip install -r requirements.txt
```

---

## Running the Project

1. Download the MNIST dataset from Kaggle.
2. Place the dataset files in the project directory.
3. Open the notebook.
4. Run all cells to:

   * Load the dataset
   * Preprocess the images
   * Train the neural network
   * Evaluate the model
   * Generate predictions

---

## Future Improvements

* Implement a Convolutional Neural Network (CNN) for higher accuracy.
* Perform hyperparameter tuning.
* Add model checkpointing and early stopping.
* Deploy the trained model as a web application using Flask or Streamlit.

---

## License

This project is intended for educational purposes.
