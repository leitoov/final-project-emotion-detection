# Emotion Detection Application

A web-based emotion detection application built with Python, Flask, and the Watson NLP Emotion Predict API.

## Project Description
This application analyzes user-provided text and identifies the underlying emotions (anger, disgust, fear, joy, and sadness) along with the dominant emotion.

## Package Structure
- `EmotionDetection/`: Python package containing the emotion detection module.
  - `emotion_detection.py`: Contains the `emotion_detector` function that interfaces with Watson NLP API.
  - `__init__.py`: Package initialization file exposing `emotion_detector`.
- `server.py`: Flask web application server providing endpoints for the UI and emotion detection analysis.
- `test_emotion_detection.py`: Unit tests validating emotional classification correctness.
- `static/mywebscript.js`: Client-side logic for submitting text and displaying results.
- `templates/index.html`: Web interface front-end.

## Installation and Execution
1. Clone the repository:
   ```bash
   git clone git@github.com:leitoov/final-project-emotion-detection.git
   cd final-project-emotion-detection
   ```
2. Install requirements:
   ```bash
   pip install flask requests pylint
   ```
3. Run unit tests:
   ```bash
   python3 test_emotion_detection.py
   ```
4. Start the server:
   ```bash
   python3 server.py
   ```
5. Open your browser at `http://localhost:5000`
