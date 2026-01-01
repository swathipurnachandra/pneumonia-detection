# Pneumonia Detection using K-Nearest Neighbors (KNN)

A machine learning project that detects pneumonia from chest X-ray images using K-Nearest Neighbors classifier.

## Dataset
This project uses the Chest X-Ray Images (Pneumonia) dataset containing:
- **Training set**: ~5,000 images
- **Validation set**: 16 images
- **Test set**: 624 images
- Two classes: NORMAL and PNEUMONIA

## Model Details
- **Algorithm**: K-Nearest Neighbors (KNN)
- **K value**: 5
- **Distance metric**: Euclidean
- **Image preprocessing**: Grayscale, resized to 128x128, normalized (0-1)
- **Feature extraction**: Flattened pixel values (16,384 features)


## Results
- **Training accuracy**: 93.68%
- **Test accuracy**: 73.24%
The model is highly sensitive to pneumonia (99% recall) but has lower precision for normal cases. This means it rarely misses pneumonia cases but may over-diagnose.

## Requirements
- Python 3.7+
- NumPy
- OpenCV
- scikit-learn
- Matplotlib
- Seaborn
- Joblib