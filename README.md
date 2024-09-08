# Voice Assistant AI

A Python-based voice-controlled AI assistant that integrates real-time audio recognition, command processing, and prompt generation functionalities. This project leverages the Whisper model for voice recognition and LangChain for language processing, along with live webcam video stream processing.

## Features

- **Real-time Speech Recognition**: Powered by OpenAI’s Whisper model, this assistant listens for voice commands and responds promptly.
  
- **Text-to-Speech Response**: The assistant generates verbal responses using OpenAI’s text-to-speech functionality, creating a natural interaction experience.
  
- **Image-Based Inference**: The assistant uses a webcam feed, converting frames into base64-encoded images and processing visual information along with voice commands for more context-rich responses.
  
- **Multiple Model Support**: The assistant is designed to work with multiple models:
  - **OpenAI GPT-4** for robust natural language processing.
  - **Google Generative AI (Gemini 1.5 Flash)** for faster responses with image processing capabilities.
  
- **Command Processing**: It uses LangChain for complex natural language command interpretation and processing.

- **Webcam Stream Processing**: Integrates `opencv-python` to capture live video frames that can be used as part of the model's inference process.

- **Ambient Noise Adjustment**: Automatically adjusts to ambient noise levels for better speech recognition performance using the SpeechRecognition library.

## Installation

To set up the project on your local machine, follow these steps.

### Prerequisites

Ensure that you have the following installed:
- Python 3.8 or higher
- A working microphone and webcam
- Git (for cloning the repository)

### Step-by-Step Guide

1. **Clone the Repository**:

   ```bash
    git clone https://github.com/your-username/voice-assistant-ai.git
    cd voice-assistant-ai
2. **Install Required Dependencies**:
   
   The required libraries are listed in the requirements.txt file.This will install the necessary packages:
   
   Opencv-python (For webcam video processing)

   Langchain, langchain-openai, langchain_google_genai (For natural language understanding and model integration)

   Pyaudio (For microphone input and text-to-speech)

   SpeechRecognition (For handling voice input)

   Whisper model from GitHub (For voice-to-text conversion) Install them with the following command:
   
   ```bash
    pip install -r requirements.txt
3. **Set Up Environment Variables**:

   Create a .env file in the root directory to store your API keys. You can use this template:

   ```env
    OPENAI_API_KEY=your_openai_api_key
    GOOGLE_API_KEY=your_google_api_key
4. **Run the Voice Assistant**:

    Once everything is installed and set up, you can start the voice assistant by running the following command:

   ```bash 
   python assistant1.py`
   ```
## Interacting with the Assistant

Speak into your microphone.

The assistant will process your command using Whisper for real-time transcription.

The webcam feed will also be active, capturing visual information and incorporating it into the assistant's responses.

The assistant will respond through text.
   
