# Aromanian Translation Project

## Overview

This project facilitates the translation of texts between Aromanian and various other languages, including Romanian, English, Spanish, and French. The workflow is structured around notebooks for cleaning text data, training translation models, and executing translations.

## Project Workflow

### Text Cleaning

- **`aromanian_text_cleaning.ipynb`**: This notebook focuses on preparing the text data for model training by performing cleaning operations such as punctuation normalization, non-printing character removal, and case normalization. While this preprocessing step is vital for quality model training, **users working with the dataset provided in the `/dataset` folder can skip this notebook, as the texts have already been preprocessed**.

### Model Training

- **`aromanian_translation_model_training.ipynb`**: The cornerstone of the project, this notebook is responsible for training the T5 models to translate texts between Aromanian and other languages. **This notebook must be run first** to generate the models necessary for the translation tasks.

### Translation Execution

- **`aromanian_translation_execution.ipynb`**: Leveraging the models generated in the previous step, this notebook executes the translation tasks. It includes a logistic regression model for language detection to ensure the correct translation model is applied based on the input text's language. **Ensure the translation model training notebook has been executed and the models are saved before running this notebook**.

## Setup

Ensure your environment is equipped to run Jupyter notebooks with Python 3.8 or newer. Install all necessary dependencies as listed in the project's requirements file for smooth operation of the notebooks.

## Usage

1. **Optional**: Execute the `aromanian_text_cleaning.ipynb` notebook if you wish to preprocess additional texts or explore the preprocessing steps. This step can be skipped if using the preprocessed dataset.
2. Run the `aromanian_translation_model_training.ipynb` notebook to train the translation models.
3. Proceed with the `aromanian_translation_execution.ipynb` for performing translations and language detection with the trained models.

## Contributing

Contributions to enhance the project are welcome. Please feel free to suggest improvements or add new features through issues or pull requests.

## License

This project is available under the MIT License. For more information, see the LICENSE file.
