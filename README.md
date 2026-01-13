# Artificial Intelligence and Machine Learning 2

## 1. Table of Contents

- [1. Table of Contents](#1-table-of-contents)
- [2. About The Project](#2-about-the-project)
    - [2.1. Submission Title](#21-submission-title)
    - [2.2. Developer Names](#22-developer-names)
    - [2.3. Release Notes](#23-release-notes)
    - [2.4. Built With](#24-built-with)
- [3. Getting Setup](#3-getting-setup)
    - [3.1. Contents of Submission](#31-contents-of-submission)
    - [3.2. Prerequisites](#32-prerequisites)
    - [3.3. Installation](#33-installation)
- [4. Usage](#4-usage)
- [5. Roadmap](#5-roadmap)
- [6. Acknowledgements](#6-acknowledgements)

## 2. About The Project

### 2.1. Submission Title

Rock-Paper-Scissors Hand Gesture Recognition System

### 2.2. Developer Names

Thomas Joseph Webster

### 2.3. Release Notes

This is the assessment project for the Artificial Intelligence and Machine Learning 2 (AIML2) module. This project implements a deep learning-based hand gesture recognition system for Rock-Paper-Scissors gameplay. The system uses computer vision and neural networks to identify hand gestures in real-time and enables interactive gameplay between a human player and AI opponents.

### 2.4. Built With


- Python 3.12.3
- TensorFlow 2.20.0
- Keras 3.11.3
- OpenCV 4.12.0
- NumPy 2.2.6
- TensorFlow/Keras for neural network implementation
- scikit-learn for evaluation metrics
- matplotlib/seaborn for visualization

## 3. Getting Setup

### 3.1. Contents of Submission

**Main Application:**
- `app.py` - Main menu and application entry point

**Model Training:**
- `models/custom_cnn.py` - Custom CNN implementation and training
- `models/transfer_learning.py` - VGG16 transfer learning implementation
- `models/lstm_predictor.py` - LSTM move predictor for smart AI
- `models/evaluate.py` - Model evaluation and comparison

**Game Implementation:**
- `game/game.py` - Rock-Paper-Scissors game with AI opponents

**Dataset:**
- `dataset_augmented/` - Augmented training dataset (1920 images) (Note this folder is empty and the images must be retrieved from the link below
- [LINK TO BE ADDED]

**Trained Models:**
- `models/custom_cnn.h5` - Trained custom CNN model
- `models/transfer_learning.h5` - Trained VGG16 transfer learning model
- `models/lstm_predictor.h5` - Trained LSTM pattern predictor

**Results:**
- `results/custom_cnn_training_history.png` - Training curves
- `results/transfer_learning_history.png` - Training curves
- `results/lstm_training_history.png` - LSTM training curves
- `results/custom_cnn_confusion_matrix.png` - Confusion matrix
- `results/transfer_learning_confusion_matrix.png` - Confusion matrix
- `results/custom_cnn_classification_report.txt` - Detailed metrics
- `results/transfer_learning_classification_report.txt` - Detailed metrics
- `results/model_comparison.txt` - Side-by-side comparison

**Documentation:**
- `README.md` - This file
- `requirements.txt` - Python dependencies
- `AI_Transparency_Statement.txt` - AI usage declaration
- `AI_Prompts_Log.txt` - AI chat prompts used during development

**Computer Images (for game display):**
- `images/rock.png`
- `images/paper.png`
- `images/scissors.png`

### 3.2. Prerequisites

- Python 3.8 or higher
- pip (Python package manager)
- Webcam/camera for live gameplay
- All dependencies are listed in `requirements.txt`.

### 3.3. Installation

**Step 1: Extract the submission**
```bash
unzip AIML.zip
cd /path/to/AIML
```

**Step 2: Create and activate virtual environment**

Linux/macOS:
```bash
python3 -m venv venv
source venv/bin/activate
```

Windows:
```bash
python -m venv venv
venv\Scripts\activate
```

**Step 3: Install dependencies**
```bash
pip install -r requirements.txt --break-system-packages  # Linux
```
OR
```bash
pip install -r requirements.txt  # Windows/macOS
```

**Step 4: Verify installation**
```bash
python app.py
```

You should see the main menu appear.

**Step 5: Download the augmented_dataset folder from google drive**

Insert link here

**Step 6: Place augmented_dataset folder in AIML root**

Everything is now installed and ready.

## 4. Usage
**Main Menu**

<img width="594" height="331" alt="image" src="https://github.com/user-attachments/assets/779056f1-e681-4eff-a698-5282986563f5" />

1. Opens the Custom CNN Menu. Training is not strictly necessary to play the game as models have already been prepared.

<img width="609" height="209" alt="image" src="https://github.com/user-attachments/assets/6c282fd6-1d85-4401-bbb4-058a67099a88" />

2. Opens the Transfer Learning Menu. Training is not strictly necessary to play the game as models have already been prepared.

<img width="679" height="309" alt="image" src="https://github.com/user-attachments/assets/c011a5ac-2933-4883-82d3-68f16282fd98" />

3. Play a game using the Custom CNN model. Play against either a random AI or a harder LSTM AI that learns your moves.

<img width="609" height="262" alt="image" src="https://github.com/user-attachments/assets/f683bdd4-a348-4660-922a-69a88cc1e4b8" />

4. Play a game using the Transfer Learning model. Play against either a random AI or a harder LSTM AI that learns your moves.

<img width="609" height="262" alt="image" src="https://github.com/user-attachments/assets/f683bdd4-a348-4660-922a-69a88cc1e4b8" />

5. Run evaluation tools to compare the effectiveness of both models.

**Game Instructions:**
1. Position your hand in the left rectangle
2. Make your gesture (rock/paper/scissors)
3. Press **SPACE** when ready
4. View the result (win/lose/draw)
5. Choose to continue or quit
6. Press **R** to reset AI memory (LSTM mode only)
7. Press **Q** to quit the game

**Tips:**
- Keep hand centered in the rectangle
- Ensure good lighting
- Hold gesture steady before pressing SPACE
- Try playing multiple rounds to see LSTM learn your patterns

## 5. Acknowledgements

Use this final section for listing links to any resources you have used, frameworks, information sources etc...

**Frameworks & Libraries:**
- [TensorFlow Documentation](https://www.tensorflow.org/api_docs)
- [Keras Documentation](https://keras.io/api/)
- [OpenCV Python Documentation](https://docs.opencv.org/4.x/d6/d00/tutorial_py_root.html)
- [scikit-learn Documentation](https://scikit-learn.org/stable/)

**Pre-trained Models:**
- [VGG16 ImageNet Weights](https://keras.io/api/applications/vgg/)

**Learning Resources:**
- [TensorFlow Transfer Learning Tutorial](https://www.tensorflow.org/tutorials/images/transfer_learning)
- [Understanding LSTM Networks](http://colah.github.io/posts/2015-08-Understanding-LSTMs/)
- [Deep Learning Specialization - Andrew Ng](https://www.coursera.org/specializations/deep-learning)

**Tools:**
- [Matplotlib for Python Visualization](https://matplotlib.org/)
- [NumPy Documentation](https://numpy.org/doc/)
