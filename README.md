# Voice Authentication & Gender Classification

This repository contains the implementation and reports for the final machine learning project.  
The goal is to explore **machine learning approaches for voice-based authentication** and **gender classification**, using real audio data.

---

## Project Objectives
- Preprocess raw audio signals (noise reduction, normalization, windowing).
- Extract features from speech signals, such as:
  - MFCC (Mel-Frequency Cepstral Coefficients)
  - Log Mel Spectrogram
  - FFT (Fast Fourier Transform)
  - Spectral Centroid, Contrast, Chroma, Zero-Crossing Rate
  - LPC / PLP features
- Perform **classification tasks**:
  - Gender classification (male/female)
  - Speaker identity authentication (closed-set)
- Perform **clustering tasks**:
  - Apply clustering methods to group voice features and evaluate similarity
- Evaluate results using:
  - Confusion matrix
  - Accuracy, Precision, Recall, F1-score
  - ROC curves and AUC values

---

## Dataset
- Audio recordings are provided in the format:  
  `HWx_Qy_StudentID_gender.mp3`
- Contains multiple speakers of both genders.
- Each recording may vary in length and requires preprocessing before feature extraction.
- Data is split into training (~75%) and testing (~25%).

### Dataset Link
The audio files can be accessed from the following Google Drive link:  
[Google Drive Dataset](https://drive.google.com/drive/folders/1pq_jGqdBda_QjNnK2yAzD4N2grbPF8Rs?usp=sharing)

**Note:**  
To run the code correctly, update the `audio_directory` variable in the scripts to the path where you store the downloaded audio files.

---

## Methods
- **Preprocessing:** noise reduction, resampling, normalization, windowing  
- **Feature Extraction:** MFCC, spectrograms, spectral features, temporal features  
- **Classification Models:** Logistic Regression, KNN, SVM, MLP, AdaBoost, XGBoost (at least 3 models compared)  
- **Clustering:** K-Means, hierarchical clustering, evaluated using silhouette score  

---

## Evaluation
- Gender classification accuracy  
- Speaker authentication results across multiple trials  
- Error analysis with confusion matrices  
- ROC curves and AUC values for classifier evaluation  

---
