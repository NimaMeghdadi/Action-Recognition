# Human Action Recognition with CNN-LSTM

This repository contains an implementation of a Human Action Recognition system using a CNN-LSTM model. The project aims to classify human actions in video sequences by leveraging the strengths of both convolutional neural networks (CNNs) and long short-term memory networks (LSTMs). The CNN-LSTM model allows us to efficiently capture spatial and temporal patterns in video data, leading to more accurate action recognition.

[Kaggle](https://www.kaggle.com/code/nimameghdadi/human-action-recognition-with-cnn-lstm)
## Overview

Human action recognition is an essential task in video analysis, used widely in surveillance, video retrieval, human-computer interaction, and sports analysis. This notebook demonstrates a CNN-LSTM approach, where:
- CNN layers extract spatial features from each frame in the video sequence.
- LSTM layers process the temporal sequence of these features to capture the action's motion dynamics.

## Why Use a CNN-LSTM Model?

1. **Spatial-Temporal Pattern Recognition**: Human actions involve both spatial information (position and orientation of body parts) and temporal information (sequence of movements over time). CNN-LSTM models excel at capturing these patterns, making them suitable for tasks like action recognition, where both dimensions are crucial.

2. **Feature Extraction**: CNN layers are effective at extracting important spatial features from each frame, such as edges and textures, which are fundamental for identifying different actions. LSTM layers then take these frame-wise features as input to learn the temporal dependencies across frames.

3. **Efficient Memory Usage**: LSTM networks are optimized for handling sequential data by keeping track of dependencies between time steps, which is necessary for understanding sequences in videos without requiring excessive memory resources.

4. **Improved Accuracy**: Compared to traditional 2D CNNs, the CNN-LSTM model can lead to better accuracy in action recognition tasks because it considers the sequential nature of the data, which is often lost in purely spatial models.

## Files

- `human-action-recognition-with-cnn-lstm.ipynb`: The main notebook file containing the code for data preprocessing, model definition, training, and evaluation.

## Dependencies

Ensure you have the following Python libraries installed:
- TensorFlow / Keras
- NumPy
- Matplotlib
- OpenCV (for video processing)
- This project is based on the Kaggle environment if you want to run it properly I recommend running it in Kaggle.

- You should run main code first and use extera code for saving time ex.model images and labels can be save.
- 
Install the dependencies with:
```bash
pip install tensorflow numpy matplotlib opencv-python
```

## Usage

Data Preparation: Load your dataset, preprocess the video frames, and split them into training and testing sets.

Training the Model: Run the notebook to train the CNN-LSTM model. Adjust hyperparameters as needed for optimal performance.

Evaluation: Use the trained model to predict actions on test videos and evaluate the results based on accuracy or other suitable metrics.

## Results
The notebook includes visualization of training metrics and examples of model predictions on test videos. You can modify and adapt the code to test on custom datasets or integrate into larger projects requiring action recognition capabilities.






