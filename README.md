# Brain Tumour Classification Using CNN

## Overview

This project implements a Convolutional Neural Network (CNN) to classify brain MRI images into different categories based on the dataset used for training. The model learns spatial features from MRI scans to identify patterns associated with different brain tumour categories.

The project demonstrates the application of deep learning and computer vision in medical image classification.

## Objectives

- Develop a CNN-based image classification model for brain MRI scans.
- Train the model on the brain MRI dataset used in the project.
- Predict the category of an input MRI image.
- Explore the application of deep learning techniques in medical image analysis.

## Dataset

The model is trained using the brain MRI dataset available for this project.

The dataset contains MRI images organized into class-specific categories. These images are used to train and evaluate the CNN model.

**Dataset details:**
- **Input:** Brain MRI images
- **Data type:** Medical images
- **Task:** Multiclass image classification
- **Preprocessing:** Image resizing, normalization, and label encoding, as implemented in the notebook
- **Data split:** As defined in the training notebook

The exact class labels and dataset distribution depend on the dataset configuration used during training.

## Model Architecture

The project uses a Convolutional Neural Network (CNN), which is designed to learn visual features directly from images.

The architecture consists of the following components, depending on the implementation:

1. **Convolutional layers:** Extract features such as edges, textures, and structural patterns.
2. **Activation functions:** Introduce non-linearity into the network.
3. **Pooling layers:** Reduce spatial dimensions while retaining important features.
4. **Flattening or feature aggregation:** Convert extracted features into a representation suitable for classification.
5. **Dense layers:** Learn relationships between the extracted features.
6. **Output layer:** Predict the class of the input MRI image.

The network is trained using labelled MRI images to minimize classification loss and improve its ability to distinguish between the dataset's categories.

## Workflow

1. Load the brain MRI dataset.
2. Preprocess the images and prepare class labels.
3. Divide the dataset into training, validation, and/or test sets as configured.
4. Define the CNN architecture.
5. Train the model using the training data.
6. Evaluate the model using the evaluation data.
7. Provide an MRI image to obtain a predicted class.

## Technologies Used

- Python
- TensorFlow/Keras or PyTorch, depending on the notebook implementation
- NumPy
- Matplotlib
- Jupyter Notebook / Google Colab

## Project Structure

```text
Brain-Tumour-Classification-using-CNN/
├── CNN_BT_DEMO.ipynb
├── Readme.md
└── README.md
```

The actual repository structure may differ depending on where the dataset, model files, and supporting scripts are stored.

## How to Run

### 1. Clone the repository

```bash
git clone https://github.com/aadubey1606/Brain-Tumour-Classification-using-CNN.git
cd Brain-Tumour-Classification-using-CNN
```

### 2. Install the dependencies

Install the libraries required by the notebook. For example, if the notebook uses TensorFlow:

```bash
pip install tensorflow numpy matplotlib jupyter
```

If it uses PyTorch, install the appropriate PyTorch version instead.

### 3. Open the notebook

You can run the project in Google Colab or locally using Jupyter Notebook.

```bash
jupyter notebook CNN_BT_DEMO.ipynb
```

### 4. Load the dataset

Ensure the dataset is available at the path expected by the notebook. Update the dataset path if necessary.

### 5. Train and test the model

Execute the notebook cells in order to preprocess the data, train the CNN, evaluate its performance, and test predictions on MRI images.

## Evaluation

Model performance should be assessed using suitable classification metrics, including:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix

Add the actual evaluation results from the completed training run before publishing them in this section.

## Limitations

- Model performance depends on the quality, diversity, and class distribution of the training dataset.
- Predictions may be affected by differences in MRI scanners, image quality, and preprocessing.
- Performance on the training dataset does not guarantee generalization to unseen clinical data.
- The model is intended for educational and research purposes and is not a substitute for professional medical diagnosis.

## Future Improvements

- Evaluate the model on an independent dataset.
- Apply data augmentation to improve generalization.
- Compare CNN performance with alternative architectures such as Vision Transformers.
- Add Grad-CAM visualizations to highlight image regions influencing predictions.
- Develop an interface for uploading MRI images and displaying predictions.

## Disclaimer

This project is intended solely for educational and research purposes. It has not been established as a clinically validated diagnostic system and must not be used to make medical decisions.


