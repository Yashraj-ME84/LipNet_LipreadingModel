# LipNet: Lip Reading with Deep Learning

This project adapts the method proposed in the paper ["LipNet: End-to-End Sentence-level Lipreading"](https://arxiv.org/abs/1611.01599) to build a deep learning model capable of lip reading. The model takes in video frames of a person speaking and predicts the sequence of characters being spoken. This implementation uses Python, TensorFlow, and OpenCV to process video data and train a deep learning model based on the LipNet architecture.

## Project Overview

Lip reading is a challenging task that requires understanding both spatial (visual) and temporal (time-based) information. The LipNet model uses Convolutional Neural Networks (CNNs) to extract features from individual video frames and Recurrent Neural Networks (RNNs) to model the temporal dynamics across frames.

### Key Features:
- **End-to-End Deep Learning Model**: The model directly predicts character sequences from video frames without needing intermediate steps.
- **Video Preprocessing**: Frames are extracted from the video and aligned with the corresponding speech using OpenCV.
- **Data Pipeline**: Utilizes TensorFlow’s `tf.data.Dataset` for efficient data handling and processing.
- **Model Architecture**: Combines convolutional layers (for spatial feature extraction) and recurrent layers (for temporal modeling).

## Dependencies

- TensorFlow
- OpenCV
- Imageio
- Gdown (for downloading datasets)

## Paper Reference
The methodology for this project is inspired by the paper "LipNet: End-to-End Sentence-level Lipreading" by Yannis M. Assael, Brendan Shillingford, Shimon Whiteson, and Nando de Freitas.

You can install these using the following command:

```bash
pip install -r requirements.txt



