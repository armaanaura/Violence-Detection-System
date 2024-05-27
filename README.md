# Violence-Detection-System

This repository contains the code for a Violence Detection System developed using an LSTM-based deep learning model. The system is designed to classify video clips as either violent or non-violent with high accuracy.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Training](#training)
- [Evaluation](#evaluation)
- [Results](#results)
- [Usage](#usage)
- [Installation](#installation)
- [Contributing](#contributing)
- [License](#license)

## Introduction
The Violence Detection System leverages the power of deep learning to analyze video content and classify it into violent and non-violent categories. This project utilizes an LSTM (Long Short-Term Memory) network to capture temporal patterns in video sequences, providing accurate classification results.

## Dataset
The model was trained and tested on the Kaggle 2000 Videos dataset, which contains a balanced collection of violent and non-violent video clips. The dataset is preprocessed and padded to ensure uniform input shapes for the LSTM model.

## Model Architecture
The model consists of:
- An LSTM layer to capture temporal features.
- Dropout layers to prevent overfitting.
- Dense layers with a sigmoid activation function for binary classification.

## Training
The model was trained using the Adam optimizer and binary cross-entropy loss function. It was trained for 30 epochs with a batch size of 32, achieving a high level of accuracy.

## Evaluation
The model was evaluated on a separate validation set, achieving a 97% accuracy rate. Various evaluation metrics such as accuracy, precision, recall, F1 score, ROC curve, and AUC were used to assess the model's performance.

## Results
The system demonstrates a robust performance with the following metrics:
- **Accuracy**: 97%
- **Precision**: High
- **Recall**: High
- **F1 Score**: High
- **AUC**: Near 1

## Usage
To use the Violence Detection System:
1. Clone this repository.
2. Install the required dependencies.
3. Run the provided scripts to preprocess data, train the model, and evaluate its performance.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/violence-detection-system.git
   cd violence-detection-system
   ```
2. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Download the Kaggle 2000 Videos dataset and place it in the appropriate directory.

4. Run the preprocessing script:
   ```bash
   python preprocess.py
   ```

5. Train the model:
   ```bash
   python train.py
   ```

6. Evaluate the model:
   ```bash
   python evaluate.py
   ```

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
