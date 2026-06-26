# oaqjp-final-project-emb-ai

This project creates a Flask application for emotion detection using the Watson NLP library.
This project is built to fulfill the grading criteria for the IBM Watson NLP Emotion Detection project.

## Features

- Detects emotions (anger, disgust, fear, joy, sadness) from text.
- Determines the dominant emotion.
- Deployed as a web application using Flask.

## Structure

- `EmotionDetection/`: A package containing the emotion detection logic.
    - `__init__.py`: Package initialization.
    - `emotion_detection.py`: Contains the `emotion_detector` function.
- `test_emotion_detection.py`: Unit tests for the application.
- `server.py`: The Flask server to host the application.
- `templates/index.html`: The user interface for the web app.

## How to Run

1.  **Install dependencies:**
    ```bash
    pip install requests flask
    ```

2.  **Run the Flask application:**
    ```bash
    python server.py
    ```

3.  **Access the application:**
    Open your browser and navigate to `http://localhost:5000`.

## Testing

To run the unit tests:

```bash
python -m unittest test_emotion_detection.py
```
*(Note: The tests may fail if the Watson NLP mock service endpoint is currently down or timing out.)*
