# EyeBallExpert: Eye-Tracking Expertise Classifier

**Author**: Carl Mann

This project uses a neural network to classify synthetic eye-tracking data into "novice" (0) and "expert" (1) categories. It generates 500 samples with features like fixation duration, saccade length, pupil diameter, and gaze coordinates, then trains a simple feedforward network using PyTorch, achieving ~90% test accuracy.

## Project Overview
EyeBallExpert aims to leverage synthetic eye-tracking data to classify users based on their expertise levels. By analyzing realistic metrics, the model provides insights that can be applied in fields such as psychology, marketing, and user experience research. This initial version uses synthetic data, with plans to expand to real-world datasets.

## Features
- Synthetic dataset generation with realistic eye-tracking metrics (e.g., fixation duration: 200-600ms).
- Simple feedforward neural network with one hidden layer (5 inputs → 10 hidden → 2 outputs, ReLU activation).
- Data preprocessing: normalization (mean=0, std=1) and 80/20 train-test split.
- Training with Adam optimizer (learning rate 0.01) over 50 epochs.

## Requirements
- Python 3.10+
- NumPy (`pip install numpy`)
- PyTorch (`pip install torch`)
- Scikit-learn (`pip install scikit-learn`)
- Matplotlib (`pip install matplotlib`)

## Installation
Clone the repository and install the required packages:
```bash
git clone https://github.com/todare/eyeBallExpert.git
cd eyeBallExpert
pip install -r requirements.txt  # See optional requirements.txt below
```
# Run the notebook
jupyter notebook eyeBallExpert.ipynb

## Results
Test Accuracy: ~90%
Train Accuracy: ~94%
Label Balance: 124 experts (1) out of 500 samples (~25%).

## Future Improvements
Incorporate real eye-tracking data for validation.
Experiment with deeper neural networks or hyperparameter tuning.
Add k-fold cross-validation for more robust evaluation.

## License
This project is unlicensed (public domain). Feel free to use, modify, or distribute it as you wish!


