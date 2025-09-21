# Brain Tumor Detection 🧠
This project implements a Convolutional Neural Network (CNN) to classify brain tumors from MRI images.  
The model is trained with TensorFlow/Keras and achieves around 88% accuracy on test data.

## Run on Google Colab
Click the badge below to open the notebook directly in Google Colab:

[![Open In Colab](https://colab.research.google.com/drive/1xmfMh0kGHdEaKBGLSpMrjHkTDFlRiRgZ?usp=sharing)


## Dataset

This project uses the **[Brain Tumor MRI Dataset](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset)** from Kaggle.  
The dataset contains MRI images divided into training and testing sets for brain tumor classification.

To use this dataset in Google Colab:

```bash
# Upload kaggle.json (YOUR Kaggle API token)
from google.colab import files
files.upload()

# Set up Kaggle credentials
!mkdir -p ~/.kaggle
!cp kaggle.json ~/.kaggle/
!chmod 600 ~/.kaggle/kaggle.json

# Download the dataset
!kaggle datasets download -d masoudnickparvar/brain-tumor-mri-dataset
!unzip brain-tumor-mri-dataset.zip -d /content/dataset
