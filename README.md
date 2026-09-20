
# 🧠 MNIST Handwritten Digit Classification

A simple deep learning project that uses **TensorFlow and Keras** to recognize handwritten digits (0–9) from the MNIST dataset.

The project builds and trains a neural network, evaluates its performance, visualizes training results, and compares a standard model with a Dropout model.

## 📌 Project Overview

Handwritten digit recognition is a classification problem in which a machine learning model identifies digits from images.

This project uses the MNIST dataset to train a neural network that predicts the digit represented by a handwritten image.

## 🎯 Objectives

- Load and explore the MNIST dataset.
- Build and train a neural network using TensorFlow/Keras.
- Evaluate the model using test accuracy.
- Visualize training and validation accuracy and loss.
- Compare actual and predicted labels for 5 test images.
- Experiment with Dropout and compare model performance.

## 📊 Dataset

The project uses the **MNIST handwritten digit dataset**, available directly through TensorFlow/Keras.

| Dataset | Number of Images |
|---|---:|
| Training | 60,000 |
| Testing | 10,000 |
| Image Size | 28 × 28 pixels |
| Classes | 10 (digits 0–9) |

Each image is a grayscale image containing a handwritten digit.

## 🛠️ Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Jupyter Notebook

## 🧠 Model Architecture

The original neural network uses the following architecture:

```text
Input Image (28 × 28)
        ↓
     Flatten
        ↓
 Dense Layer (128 neurons)
 Activation: ReLU
        ↓
 Dense Layer (10 neurons)
 Activation: Softmax
        ↓
 Predicted Digit (0–9)
```

### Model Configuration

| Parameter | Value |
|---|---|
| Optimizer | Adam |
| Loss Function | Sparse Categorical Crossentropy |
| Metric | Accuracy |
| Epochs | 10 |
| Batch Size | 32 |
| Validation Split | 20% |

## ⚙️ Project Workflow

1. Load the MNIST dataset.
2. Explore dataset dimensions and class distribution.
3. Display sample handwritten digit images.
4. Normalize pixel values from 0–255 to 0–1.
5. Build and compile the neural network.
6. Train the model using the training dataset.
7. Evaluate the model on the test dataset.
8. Visualize training and validation accuracy and loss.
9. Predict digits for 5 test images.
10. Add Dropout and compare the experimental model.

## 🧪 Experiment: Dropout

An experiment is performed by adding a Dropout layer to the original neural network.

**Original model:**

```text
Flatten → Dense(128, ReLU) → Dense(10, Softmax)
```

**Dropout model:**

```text
Flatten → Dense(128, ReLU)
        → Dropout(0.2)
        → Dense(10, Softmax)
```

The Dropout layer randomly disables 20% of the hidden-layer neurons during training. This experiment investigates whether Dropout helps reduce overfitting.

Both models are trained for 10 epochs and evaluated using test accuracy and validation performance.

## 📈 Visualizations

The notebook includes:

- Sample MNIST handwritten digit images.
- Training vs. validation accuracy.
- Training vs. validation loss.
- Actual vs. predicted labels for 5 test images.
- Original vs. Dropout model validation accuracy.
- Original vs. Dropout model validation loss.

## 📂 Project Structure

```text
MNIST---HANDWRITTEN--DIGIT-CLASSIFICATION/
│
├── MNIST_Handwritten_digit_Classification.ipynb
└── README.md
```

## 🚀 How to Run the Project

### Option 1: Google Colab

1. Open [Google Colab](https://colab.research.google.com/).
2. Upload the Jupyter Notebook from this repository.
3. Run the notebook cells sequentially.
4. View the model evaluation, predictions, and visualizations.

### Option 2: Run Locally

**1. Clone the repository**

```bash
git clone https://github.com/pavan-1818/MNIST---HANDWRITTEN--DIGIT-CLASSIFICATION.git
```

**2. Navigate to the project folder**

```bash
cd MNIST---HANDWRITTEN--DIGIT-CLASSIFICATION
```

**3. Install the required libraries**

```bash
pip install tensorflow numpy matplotlib jupyter
```

**4. Launch Jupyter Notebook**

```bash
jupyter notebook
```

**5. Open and run**

Open `MNIST_Handwritten_digit_Classification.ipynb` and run all cells.

The MNIST dataset will be downloaded automatically by TensorFlow when needed.

## 📋 Results

The notebook prints the following results after training:

- Original model test loss and accuracy.
- Dropout model test loss and accuracy.
- Best validation accuracy for both models.
- Actual and predicted labels for 5 test images.
- Correct or incorrect prediction status for each sample.

**Note:** Run the notebook to obtain the actual accuracy values. Results may vary depending on the training environment and execution.

## 🔮 Future Improvements

- Test different numbers of hidden-layer neurons.
- Experiment with different activation functions.
- Build a Convolutional Neural Network (CNN).
- Create a web application using Streamlit.
- Allow users to upload their own handwritten digit images.

## 👨‍💻 Author

**R. Pall Pavan**

B.Tech Information Technology  
Rai Technology University, Bengaluru

- GitHub: [pavan-1818](https://github.com/pavan-1818)
- LinkedIn: [R. Pall Pavan](https://www.linkedin.com/in/r-pall-pavan-www876bb636b/)

## 📜 License

This project is intended for educational and learning purposes.
