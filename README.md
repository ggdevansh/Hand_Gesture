# Hand Gesture Recognition

This project implements a real-time Hand Gesture Recognition system using computer vision and machine learning techniques. It detects and classifies static hand gestures captured via webcam using OpenCV and MediaPipe, enabling gesture-based interaction.

## Features

- Real-time hand landmark detection using MediaPipe
- Custom gesture classification using trained models
- Support for multiple gestures (e.g., thumbs up, peace sign, etc.)
- Modular code with separate scripts for data collection, model training, and recognition

## Project Structure

```
Hand_Gesture/
├── dataset/                  # Collected gesture images
├── models/                   # Saved models for classification
├── trained_model.pkl         # Trained classifier
├── HandTrackerModule.py      # Hand tracking logic using MediaPipe
├── GestureRecognition.py     # Gesture classifier logic
├── collect_data.py           # Script to capture training data
├── train_model.py            # Training script for gesture classification
├── main.py                   # Main application to run gesture recognition
├── requirements.txt          # Required Python packages
└── README.md
```

## Requirements

Install dependencies:

```bash
pip install -r requirements.txt
```

## How to Run

1. **Collect Data (optional)**  
   ```bash
   python collect_data.py
   ```

2. **Train the Model**  
   ```bash
   python train_model.py
   ```

3. **Run Gesture Recognition App**  
   ```bash
   python main.py
   ```

## Model & Approach

- **Hand Tracking**: MediaPipe detects 21 hand landmarks.
- **Feature Extraction**: Landmarks converted into feature vectors (angles/distances).
- **Classification**: Uses an SVM or KNN model trained on gesture data.

## Future Improvements

- Add more gestures and examples
- Train with a deep learning model for better accuracy
- Implement dynamic gesture recognition

## Author

**Devansh Gupta**  
[GitHub](https://github.com/ggdevansh)
