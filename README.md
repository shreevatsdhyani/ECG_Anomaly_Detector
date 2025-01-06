# ECG Anomaly Detector

An Autoencoder-based deep learning model designed to detect anomalies in ECG signals. This project leverages TensorFlow and Keras to identify irregularities in heart activity, aiding in the early detection of potential cardiac issues.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Dataset](#dataset)
- [Setup and Installation](#setup-and-installation)
- [Usage](#usage)
- [Results](#results)
- [Future Improvements](#future-improvements)
- [Contributing](#contributing)
- [License](#license)

---

## Introduction
Electrocardiograms (ECGs) are critical in monitoring cardiac activity. This project aims to automate the detection of anomalies in ECG signals using an Autoencoder model. The model learns normal ECG patterns and flags any deviations as potential anomalies.

## Features
- **Autoencoder Architecture**: Encoder-decoder-based model for effective signal reconstruction.
- **Anomaly Detection**: Differentiates between normal and anomalous ECG patterns.
- **Visualization**: Displays signal reconstructions and metrics like ROC and Precision-Recall curves.
- **Data Preprocessing**: Scales and segregates ECG signals for training and testing.

## Technologies Used
- **Programming Language**: Python
- **Frameworks**: TensorFlow, Keras
- **Libraries**:
  - NumPy, Pandas (Data Manipulation)
  - Scikit-learn (Model Evaluation)
  - Matplotlib, Seaborn, Plotly (Visualization)

## Dataset
The dataset consists of ECG signals, with labels indicating normal or anomalous readings. 
- Download the dataset from [MIT-BIH Arrhythmia Database](https://www.physionet.org/content/mitdb/).
- Preprocess data with Min-Max scaling and separate normal and anomalous signals.

## Setup and Installation
### Prerequisites
- Python 3.8+
- pip package manager

### Installation Steps
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/ecg-anomaly-detector.git
   cd ecg-anomaly-detector
   ```
2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # For Windows: venv\Scripts\activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
1. Preprocess the dataset:
   ```bash
   python preprocess_data.py
   ```
2. Train the Autoencoder model:
   ```bash
   python train_model.py
   ```
3. Evaluate the model:
   ```bash
   python evaluate_model.py
   ```
4. Visualize results:
   ```bash
   python visualize_results.py
   ```

## Results
- **Evaluation Metrics**:
  - ROC Curve: Area Under Curve (AUC)
  - Precision-Recall Curve
  - Confusion Matrix and Classification Report

- **Visualization**:
  - Reconstructed ECG signals
  - Detection thresholds and anomalies

## Future Improvements
- Integrate real-time anomaly detection capabilities.
- Expand dataset to include more diverse ECG patterns.
- Optimize model architecture for faster training and improved accuracy.
- Deploy as a web application or mobile app for broader accessibility.

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork this repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add your message here"
   ```
4. Push to the branch:
   ```bash
   git push origin feature-name
   ```
5. Open a Pull Request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
