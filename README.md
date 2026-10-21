# Brain Tumour Classification Using CNN (ResNet-18)

## Overview

This project uses a Convolutional Neural Network (CNN), based on the ResNet-18 architecture, to classify brain MRI images into the categories supported by the trained model.

The project uses a curated brain tumour dataset hosted on Hugging Face. The trained model checkpoint is hosted separately on Hugging Face, allowing users to run the demonstration notebook without downloading the entire dataset or training the model from scratch.

The project includes a Google Colab demonstration notebook where users can load the trained model, provide a brain MRI image, and observe the model's prediction.

## Quick Start — Run the Demo

**The easiest way to test the project is through Google Colab.** No local Python environment or GPU setup is required.

### Step 1: Open the Demo Notebook

[**Open CNN Brain Tumour Classification Demo in Google Colab**](https://colab.research.google.com/github/aadubey1606/Brain-Tumour-Classification-using-CNN/blob/main/CNN_BT_DEMO.ipynb)

If the link does not open, you can access the notebook through the [GitHub repository](https://github.com/aadubey1606/Brain-Tumour-Classification-using-CNN) and open `CNN_BT_DEMO.ipynb` in Google Colab.

### Step 2: Run the Notebook

1. Open the notebook in Google Colab.
2. Select a runtime from **Runtime → Change runtime type**. A GPU is optional for inference.
3. Execute the notebook cells in order.
4. Allow the notebook to download and load the trained model checkpoint from Hugging Face.
5. Upload or provide a brain MRI image when prompted by the notebook.
6. Run the prediction cell to view the model's output.

The demo uses the pretrained checkpoint rather than requiring a complete training run.

### Step 3: Test with an MRI Image

Use an MRI image compatible with the model's expected input format. Follow the notebook's preprocessing and image-upload instructions to obtain a prediction.

For reproducible testing, use sample images from the supported dataset or other appropriately sourced MRI images.

## Project Resources

| Resource | Description |
|---|---|
| [Demo Notebook](https://colab.research.google.com/github/aadubey1606/Brain-Tumour-Classification-using-CNN/blob/main/CNN_BT_DEMO.ipynb) | Interactive demonstration in Google Colab |
| [GitHub Repository](https://github.com/aadubey1606/Brain-Tumour-Classification-using-CNN) | Source code and notebook |
| [Hugging Face Dataset](https://huggingface.co/datasets/Sohaaam/Brain_Tumour_Curated) | Curated dataset used for model training |
| [Hugging Face Model Repository](https://huggingface.co/Aayush1606/RESNET_18_FILE) | Hosted trained model checkpoint |

## Dataset

The model was trained using the curated brain MRI dataset hosted at [Sohaaam/Brain_Tumour_Curated](https://huggingface.co/datasets/Sohaaam/Brain_Tumour_Curated).

The dataset provides the image data used during model development. Keeping the dataset hosted on Hugging Face makes it easier to access and reuse without including the full collection of images in the GitHub repository.

**Dataset:** `Sohaaam/Brain_Tumour_Curated`

**Platform:** Hugging Face Datasets

## Model Architecture

The project uses **ResNet-18**, a convolutional neural network architecture based on residual learning.

Its main components include:

- Convolutional layers for extracting visual features from MRI images.
- Residual connections that support the training of deeper networks.
- Feature extraction layers that learn useful image representations.
- A classification layer that produces scores for the supported classes.

The trained checkpoint is hosted in the [Hugging Face model repository](https://huggingface.co/Aayush1606/RESNET_18_FILE) and is loaded by the demonstration notebook.

## Technologies Used

- Python
- PyTorch
- Torchvision
- Hugging Face Hub
- Hugging Face Datasets
- Google Colab
- Jupyter Notebook

## Repository Structure

```text
Brain-Tumour-Classification-using-CNN/
├── CNN_BT_DEMO.ipynb
└── README.md
```

The trained checkpoint and curated dataset are hosted separately on Hugging Face, keeping the GitHub repository lightweight.

## Running Locally

To run the project locally, clone the repository:

```bash
git clone https://github.com/aadubey1606/Brain-Tumour-Classification-using-CNN.git
cd Brain-Tumour-Classification-using-CNN
```

Install the dependencies required by the notebook and open it using Jupyter Notebook or JupyterLab.

```bash
pip install torch torchvision huggingface_hub datasets pillow matplotlib jupyter
jupyter notebook CNN_BT_DEMO.ipynb
```

Run the notebook cells in sequence. Ensure that the model-loading code points to the correct Hugging Face repository and checkpoint filename.

## Evaluation

The model should be evaluated using appropriate classification metrics, such as:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix

Insert the actual measured results from the completed evaluation here. Results should be reported with the evaluation dataset and test procedure clearly identified.

## Limitations

- Predictions depend on the training data, image preprocessing, and model generalization.
- Images from different scanners or datasets may produce different results.
- Performance on the curated dataset does not establish clinical reliability.
- The model is intended for educational and research purposes, not for independent medical diagnosis.

## Disclaimer

This project is intended for educational and research purposes only. Its predictions must not be used as a substitute for professional medical assessment or clinical diagnosis.

