Environmental-Sound-Recognition-using-Deep-Learning

This project implements a Convolutional Neural Network (CNN) to classify environmental sounds from the UrbanSound8K dataset. The system processes audio files, converts them into Mel spectrograms, and uses a trained CNN model to identify the sound's category. The entire application is packaged with a Flask API for easy deployment on cloud platforms like AWS or GCP.

Project Description: 
The goal of this project is to build an accurate and deployable audio classification system. Raw audio waveforms are not ideal for pattern recognition with CNNs. Therefore, we transform audio signals into Mel spectrograms, which are 2D visual representations of the spectrum of frequencies in a sound over time. These spectrograms can be treated like images, making them perfect for analysis with a CNN.
The trained model can distinguish between 10 different urban sound classes.

🎵 Dataset :-
This project uses the UrbanSound8K dataset. It contains 8732 labeled sound excerpts (<=4s) of 10 urban sound classes:

air_conditioner

car_horn

children_playing

dog_bark

drilling

engine_idling

gun_shot

jackhammer

Of course. Here is a comprehensive README.md file for your project. You can copy and paste this directly into a file named README.md in your project's root directory.

Urban Sound Classification using Deep Learning
This project implements a Convolutional Neural Network (CNN) to classify environmental sounds from the UrbanSound8K dataset. The system processes audio files, converts them into Mel spectrograms, and uses a trained CNN model to identify the sound's category. The entire application is packaged with a Flask API for easy deployment on cloud platforms like AWS or GCP.

📝 Table of Contents
Project Description

Features

Dataset

Methodology

Technology Stack

Files in this Repository

Setup and Installation

Running the Application

Deployment

📖 Project Description
The goal of this project is to build an accurate and deployable audio classification system. Raw audio waveforms are not ideal for pattern recognition with CNNs. Therefore, we transform audio signals into Mel spectrograms, which are 2D visual representations of the spectrum of frequencies in a sound over time. These spectrograms can be treated like images, making them perfect for analysis with a CNN. The trained model can distinguish between 10 different urban sound classes.

✨ Features
Accurate Classification: Achieves high accuracy on the 10 classes of the UrbanSound8K dataset.

End-to-End System: From audio preprocessing to model prediction and API endpoint.

Image-like Feature Representation: Uses Mel spectrograms to capture time-frequency patterns.

Ready for Deployment: Includes a Flask API and is structured for deployment on cloud services.

🎵 Dataset
This project uses the UrbanSound8K dataset. It contains 8732 labeled sound excerpts (<=4s) of 10 urban sound classes:

air_conditioner

car_horn

children_playing

dog_bark

drilling

engine_idling

gun_shot

jackhammer

siren

street_music

🧠 Methodology
The workflow is as follows:

Audio Preprocessing: An input audio file is loaded using librosa. It is then converted into a Mel spectrogram.

Feature Scaling: The spectrogram is normalized to be suitable for the neural network.

Model Prediction: The preprocessed spectrogram (now a 2D array) is fed into the trained CNN model (cnn2.keras).

Output: The model outputs a prediction, which is decoded using the labelencoder.pkl to get the final sound class name (e.g., "dog_bark").

siren

street_music


💻 Technology Stack
Backend: Python, Flask

Machine Learning: TensorFlow, Keras
Audio Processing: Librosa
Data Handling: NumPy, Scikit-learn (for the LabelEncoder)
Frontend: HTML
Deployment: AWS, GCP, Heroku (or any other cloud platform that supports Python)
