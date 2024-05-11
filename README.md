# Gemini Explorer Chat Application

This application integrates Google's Vertex AI generative models into a Streamlit web interface to provide an interactive chat experience.

## Features

- **Vertex AI Integration**: Utilizes the `vertexai` Python package to integrate a generative model, enabling natural language processing capabilities.
- **Interactive Chat Interface**: Built with Streamlit, this feature allows real-time interaction between users and the AI model.
- **Session State Management**: Manages chat history using Streamlit's session state to maintain conversation context.

## Setup

1. **Vertex AI Project Initialization**:
    - The application initializes with a specified project ID from Google Cloud (`gemini-explorer-423002`).

2. **Generative Model Configuration**:
    - Configures the AI model (`gemini-pro`) with a generation configuration to control the response style and randomness (`temperature=0.4`).

3. **Streamlit Web Interface**:
    - Features include a title, a user input box, and a section to display the chat history.

## Usage

- **Start the Application**: Run the Streamlit application, and it will load the chat interface.
- **Interact with the AI**: Enter queries into the chat input box. The AI, named "ReX" and powered by Google Gemini, responds interactively, using emojis for a friendly user experience.

## Code Functionality

- **`llm_function`**: A helper function to send queries to the AI model and display responses.
- **Chat Initialization**: On the first run, the AI introduces itself to set the tone of the conversation.

## Requirements

- Python 3.6 or later
- Streamlit
- Vertex AI Python client library

## Installation

Install the required packages using pip:

```bash
pip install -r requirements.txt
```

## Run the Application
Execute the application with Streamlit:
```bash
streamlit run gemini-explorer.py
```