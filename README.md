# Emotion and Hand Gesture-Based Music Recommendation System 


## Introduction 

The project addresses limitations in conventional music recommendation systems by integrating user emotions and hand gestures to enhance the auditory experience. Current research typically focuses on either hand gesture-based controllers or emotion-based players, but not both simultaneously.

![System Design](/api/placeholder/800/400)

## Methodology

The system employs two main components:

### 1. Gesture Recognition
- Uses MediaPipe framework with TensorFlow for hand detection and gesture recognition
- Implemented on the Hand Gesture Recognition dataset from Kaggle using DenseNet201
- Recognizes 8 distinct gestures including Okay, Thumbs Up, Thumbs Down, Stop, Rock, Call Me, Live Long, and Fist
- Hand gesture recognition achieved 95% accuracy

![Hand Gestures](/api/placeholder/600/300)

### 2. Emotion Detection
- Utilizes Facial Expression Recognizer (FER) algorithm on the FER2013 dataset
- Identifies seven emotions: Angry, Disgust, Fear, Happy, Sad, Surprise, and Neutral
- Emotion recognition achieved 82% accuracy

![Emotion Detection](/api/placeholder/600/300)

### Implementation Process
1. Initialize MediaPipe framework
2. Detect hand landmarks from webcam input
3. Recognize gestures using trained model
4. Process facial expressions for emotion detection
5. Map detected emotions to appropriate music categories
6. Play corresponding music based on detected gesture/emotion

## Technical Components

- **Frontend**: Tkinter module for GUI design
- **Music Playback**: Pygame module for controlling audio files
- **Data Processing**: OpenCV for facial expression recognition
- **Emotional Mapping**: Maps Navarasa (nine emotions) to Melakarta ragas

## Results and Performance

- The hybrid model achieved an overall accuracy of 88%
- Successfully plays music corresponding to detected emotions and gestures
- Outperforms existing solutions in terms of performance and accuracy

![System Performance](/api/placeholder/700/350)

## Future Scope

The project identified several opportunities for future development:
- Improving hand gesture recognition with advanced machine learning techniques
- Exploring multimodal input combinations for better preference understanding
- Implementing real-time feedback mechanisms
- Developing context-aware recommendation algorithms
- Extending the approach to other domains beyond music
