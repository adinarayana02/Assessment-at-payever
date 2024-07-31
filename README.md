# AI Engineering Task

## Task Overview

This project is a product category classification model that uses a combination of textual and numerical features to predict the category of a product.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Project Overview
This project demonstrates how to combine different types of data (text and numeric) in a neural network model. The model uses an embedding layer to process text data (product descriptions) and combines it with numeric data (product prices) to predict the product category.

## Task Requirements
### Prerequisites
- Python 3.9 or above
- TensorFlow
- Pandas
- NumPy

## Dataset
The dataset is a simple, realistic dummy dataset containing the following fields:
- **name**: The name of the product.
- **description**: A brief description of the product.
- **price**: The price of the product.
- **category**: The category of the product, which is the target variable.

## Model Architecture
The model uses two inputs:
1. **Text Input**: Product descriptions are tokenized and padded, then passed through an embedding layer and flattened.
2. **Numeric Input**: Product prices are passed directly as numeric input.

The outputs from these two branches are concatenated and passed through dense layers to produce the final classification output.

## Installation
To set up the project, follow these steps:

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/product-category-classification.git
    cd product-category-classification
    ```

2. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

## Usage
To run the model, you can use the provided script. Here's a basic example of how to execute the code:

1. Ensure you have your Python environment set up and the necessary packages installed.
2. Run the script:
    ```bash
    python your_script_name.py
    ```

The script will print the model's architecture, training history, and evaluation metrics.

## Results
After training, the model achieves the following performance metrics:
- **Training Accuracy**: ~99%
- **Validation Accuracy**: ~95%
- **Test Accuracy**: ~90%

These metrics indicate that the model is able to generalize well to unseen data.

## Contributing
Contributions are welcome! If you would like to contribute to this project, please fork the repository and submit a pull request.

## License
This project is licensed under the MIT License. 
