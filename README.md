# Aromanian Translation Project

## Overview

This project aims to bridge language barriers through the translation of texts between Aromanian and several major languages, including Romanian, English, Spanish, and French. The project workflow includes notebooks for text preprocessing, model training, and the execution of translation tasks.

## Project Workflow

### Text Preprocessing

- **[aromanian] text preprocess.ipynb**: This notebook is dedicated to the cleaning and normalization of text data. It performs essential preprocessing steps such as punctuation normalization, removal of non-printing characters, and text lowercasing to prepare the data for model training. While this step is crucial for preparing high-quality datasets for training, **it's important to note that you are not required to run this notebook if you're using the dataset provided in the `/dataset` folder**, as the text has already been preprocessed and is ready for use.

### Step 1: Model Translation

- **[aromanian] model translation.ipynb**: The first essential step in the project workflow involves fine-tuning a T5 model for translating between Aromanian and other languages. This notebook must be executed first to generate the translation models that will be used in subsequent steps.

### Step 2: Model of Everything (MOE)

- **[aromanian] moe.ipynb**: After the translation models have been trained and saved, this notebook leverages those models for translation tasks. It also incorporates a logistic regression model for detecting the language of the input text, ensuring the selection of an appropriate translation model. Make sure the model translation notebook has been executed and the models saved before proceeding with this notebook.

## Setup

To participate in this project, ensure your environment is set up to run Jupyter notebooks with Python 3.8 or later. Install all required dependencies as listed in the project's requirements file to ensure smooth execution of the notebooks.

## Usage

1. **Optional**: Run the `[aromanian] text preprocess.ipynb` notebook if you wish to preprocess additional texts or understand the preprocessing steps. This step can be skipped if using the provided dataset.
2. Execute the `[aromanian] model translation.ipynb` notebook to train and save the translation models.
3. Proceed with the `[aromanian] moe.ipynb` notebook for translation and language detection tasks using the previously saved models.
