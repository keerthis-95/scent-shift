ScentShift is a TensorFlow project that classifies gases from chemical sensor readings using the UCI Gas Sensor Array Drift Dataset.
The dataset contains sensor measurements collected over time, so the sensor behavior changes slowly. This is called sensor drift. The goal is to train a model that can still classify gases well even when the sensor data changes over time.

- Source: UCI Machine Learning Repository
- Dataset: Gas Sensor Array Drift Dataset
- Samples: 13,910
- Sensors: 16
- Features per sample: 128
- Classes: 6
- Batches: 10

I used a time-based split:
- Train: batches 1 to 7
- Validation: batch 8
- Test: batches 9 and 10

MODEL - simple TensorFlow neural network with dense layers and softmax output for 6-class classification.

RESULTS:
- Validation accuracy: 0.93
- Confusion matrix: included in the notebook
- Evaluation: accuracy and classification report

This project helped me practice:
- parsing raw data,
- preprocessing,
- TensorFlow model building,
- early stopping,
- evaluation with confusion matrix,
- handling data drift.

DATASET Link : https://archive.ics.uci.edu/dataset/224/gas+sensor+array+drift+dataset
