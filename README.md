# E-Commerce Chatbot

This project implements an E-Commerce Chatbot using natural language processing and machine learning. The chatbot is designed to handle various customer queries related to e-commerce operations.

## Overview

The notebook contains the following main sections:

1. Data Import and Preprocessing
2. Model Creation and Training
3. Chatbot Response Generation
4. GUI Interface

## Key Components

- **Data Processing**: The chatbot uses a JSON file (`intents.json`) containing various intents and their corresponding patterns and responses.
- **NLP Techniques**: NLTK is used for tokenization and lemmatization of text data.
- **Neural Network Model**: A sequential neural network is built using Keras with the following architecture:
  - Input layer with 128 neurons and ReLU activation
  - Dropout layer (0.5)
  - Hidden layer with 64 neurons and ReLU activation
  - Dropout layer (0.5)
  - Output layer with softmax activation
- **Model Training**: The model is trained on preprocessed data for 200 epochs.
- **Response Generation**: Functions are implemented to process user input, predict the intent, and generate appropriate responses.
- **GUI**: A graphical user interface is created using Tkinter, allowing users to interact with the chatbot.

## Libraries Used

- NLTK
- Keras
- NumPy
- Tkinter
- JSON
- Pickle

## How it Works

1. The chatbot loads the trained model and preprocessed data.
2. User input is processed and converted into a bag-of-words representation.
3. The model predicts the intent of the user's message.
4. Based on the predicted intent, an appropriate response is selected and displayed.

## GUI Features

- Chat window to display conversation history
- Input box for user messages
- Send button to submit messages
- Scrollbar for navigating through chat history