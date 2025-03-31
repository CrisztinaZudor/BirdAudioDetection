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

You can easily run the code in Google Colab by following these steps:

1. **Download the Dataset**:  
   Download both of the following files from [this Kaggle link](https://www.kaggle.com/datasets/langatfestus/bird-audio-detection):
   - `ff1010bird_metadata.csv` — contains metadata for the audio samples.
   - `ff1010bird_wav` — a folder containing all the audio `.wav` files used in the project.

2. **Open in Colab**:  
   Navigate to the `BirdDetection.ipynb` notebook in this repository. Click on the "Open in Colab" button at the top of the notebook to launch it in Google Colab.

3. **Upload the Files**:  
   Before running the notebook, upload both:
   - `ff1010bird_metadata.csv`
   - The **entire** `ff1010bird_wav` folder  
   to your Colab session using the file upload feature (accessible from the left sidebar under the Files tab).

4. **Run the Notebook**:  
   Once everything is uploaded and the notebook is open:
   - Click on `Runtime` > `Run all` to execute all cells in sequence.
   - Alternatively, run each cell individually using the play button next to each code block.

### Running Locally

If you prefer to run the notebook on your local machine:

1. **Download the Notebook**:  
   Go to `BirdDetection.ipynb` in the GitHub repository, click on `Raw`, then right-click and choose "Save as" to download the notebook to your computer.

2. **Download the Dataset**:  
   From [this Kaggle link](https://www.kaggle.com/datasets/langatfestus/bird-audio-detection), download:
   - `ff1010bird_metadata.csv`
   - The `ff1010bird_wav` folder containing all the audio files.

3. **Place Files in Same Directory**:  
   Ensure that both the CSV file and the `ff1010bird_wav` folder are in the same directory as the notebook.

4. **Run the Notebook**:  
   Open the notebook with Jupyter or another supported IDE (like VS Code with a Python environment). Run the cells sequentially or individually. Make sure your environment has the necessary dependencies installed.

