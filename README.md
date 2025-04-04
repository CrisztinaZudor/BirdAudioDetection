# Automatic Bird Detection in Audio Recordings

This project presents a method for detecting and classifying bird sounds using Convolutional Neural Networks (CNN). The primary focus is on preprocessing audio signals and extracting Mel-Frequency Cepstral Coefficients (MFCC) features, followed by classification using a CNN model. The performance of the model is evaluated based on accuracy and loss metrics, demonstrating its effectiveness in recognizing bird sounds.

## Project Overview

The project aims to assist ornithologists, ecologists, and bird-watching enthusiasts in monitoring bird populations and studying their behaviors through automated audio recognition. The challenge lies in accurately identifying bird sounds amid noisy recordings from various environments, necessitating advanced technological solutions.

## Methodology

The methodology involves several key processes:

- **Data Preprocessing:** Audio signals are preprocessed to extract relevant features, which are then transformed into spectrograms for input into the CNN model.
- **Feature Extraction:** We utilize MFCC for transforming audio frequency spectra into the cepstral domain, which mimics human-like hearing perceptions.
- **CNN Model:** The CNN architecture is designed to classify preprocessed audio signals effectively. It includes layers for convolution, pooling, and dropout to prevent overfitting, followed by dense layers for final classification.

## Dataset

The Freefield1010 dataset is used, consisting of 7,690 audio recordings, each lasting 10 seconds. This dataset provides a standardized collection of audio samples, suitable for training and testing our model. Each recording is in mono channel, with a sampling frequency of 44.1 kHz and 16-bit PCM encoding.

## Libraries and Tools

The following libraries and tools are integral to the project:

- **NumPy:** For handling numerical operations.
- **Pandas:** For data manipulation and I/O operations.
- **Librosa:** For audio signal processing.
- **TensorFlow & Keras:** For building and training the CNN model.
- **Matplotlib & Seaborn:** For data visualization.
- **IPython.display:** For audio playback in notebooks.

## How to Run the Code

### Running the Code in Google Colab
You can easily run the code in Google Colab with the following steps:
1. **Open in Colab**: Navigate to the `BirdAudioDetection.ipynb` notebook in this repository. You will find an "Open in Colab" button at the top of the notebook. Click this button to open the notebook directly in Google Colab.
2. **Running the Notebook**: Once the notebook is open in Google Colab, you can execute the code:
    - Run all cells in sequence by clicking on `Runtime` in the menu bar, then selecting `Run all`.
    - Alternatively, run each cell individually by clicking the play button on the left side of each code cell.
    - 
### Running Locally
If you prefer to run the notebook locally:
1. **Download the Notebook**: Click on `BirdAudioDetection.ipynb` in the GitHub repository and download it by clicking on `Raw`, then right-clicking and choosing "Save as" to download the file to your local machine.
2. **Upload to Colab**: Go to [Google Colab](https://colab.research.google.com/), and select `Upload notebook` from the `File` menu to upload the downloaded `.ipynb` file.
3. **Run the Notebook**: Follow the same steps as above to run the notebook cells sequentially or individually.
