# OSCC_LymphNode_Met_DLmodel_Codes
For project: Detection of Lymph Node Metastasis in Oral Squamous Cell Carcinoma Using Deep Learning on Histopathology Images
Python-based deep learning pipeline approach for detecting lymph node metastasis in OSCC using image classification approach and standard microscopic images without dependency on whole slide imaging

**Diclaimer: Data availability statement:**
The in-house dataset (patches and images) cannot be disclosed publicly due to institutional data protection policies and confidentiality constraints.
The python script used for patch generation, stain normalization, and training of convolutional neural network models using transfer learning approach has been shared in a GitHub repository which can be accessed using the following link.
Use of any code / weights / fine-tuned model / image data is strictly prohibited for commercial use.
## Overview
This repository contains scripts for patch generation, stain normalization, geometric data augmentation, and CNN-based model training/validation using a transfer learning approach.

## Contents
- `Patch_Generation_From_Microscopic_Images.ipynb` – Generates patches (256x256) from microscopic images.
- `Functional_Stain_Normalization.ipynb` – Applies Reinhard stain normalization for color consistency.
- `Data_augmentation_geometric.ipynb` – Performs rotations and flips to increase dataset variability.
- `Common_training_and_Validation_script_for_CNN.ipynb` – Trains and validates CNN models (e.g., Xception) on the processed data.


## Usage
**1. Clone this repository:**
   ```bash
   git clone https://github.com/username/OSCC_LymphNode_Met_DLmodel_Codes.git
   cd OSCC_LymphNode_Met_DLmodel_Codes

**   2. **##Create a conda virtual environment and install the following libraries using:****
 requirements_LN_Met_OSCC.txt
Use : pip install -r requirements_LN_Met_OSCC.txt


3. Run the codes sequrentially to generate patches from microscopic images, manually classify them into Normal and Meta, then perform Stain normalization and data augmentation. Then run the common training script and modify according to the selected CNN architecture. Model training is done using transfer learning approach.

