# Chord Classification with CNN

This project is focused on classifying audio files into major or minor chords using a Convolutional Neural Network (CNN). The project utilizes various Python libraries, including `librosa` for audio processing and `TensorFlow` for building and training the CNN model.

## Project Overview

The goal of this project is to accurately classify audio files as either major or minor chords. This is achieved through the following steps:
1. **Audio Processing**: Audio files are processed and converted into spectrogram images using `librosa`.
2. **Model Design**: A Convolutional Neural Network (CNN) is designed to classify the spectrograms.
3. **Training**: The model is trained on a dataset of labeled major and minor chord spectrograms.
4. **Evaluation**: The trained model is evaluated on unseen data to determine its accuracy and robustness.

## Directory Structure
```
├── Chords/
│ ├── Major/
│ │ ├── Major_1.wav
│ │ ├── Major_2.wav
│ │ └── ...
│ └── Minor/
│ ├── Minor_1.wav
│ ├── Minor_2.wav
│ └── ...
├── Image_Folder/
│ ├── Major/
│ └── Minor/
```

- `Chords/`: Contains the audio files categorized into Major and Minor chords.
- `Image_Folder/`: Stores the generated spectrogram images from the audio files.
- `Scale_Recognition.ipynb`: Jupyter notebook with the full implementation.

## Results

The CNN model achieves an accuracy of approximately X% on the validation set and Y% on the test set, demonstrating its effectiveness in classifying major and minor chords.

## Conclusion


The CNN model shows strong performance on the training set, achieving an accuracy of 99.25% with a minimal loss of 0.0469. However, the model's performance on the validation set indicates overfitting, with a significantly lower accuracy of 60.00% and a high validation loss of 9.2013. This suggests that while the model has learned to classify the training data effectively, it struggles to generalize to unseen data.

To address this issue, further steps such as regularization techniques, data augmentation, or additional tuning of the model architecture and hyperparameters may be necessary. Despite the current limitations, this project provides a solid foundation for audio file preprocessing and classification using CNNs, particularly in distinguishing between major and minor chords.

