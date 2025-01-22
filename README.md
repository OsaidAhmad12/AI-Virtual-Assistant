# AI-Virtual-Assistant

Overview
This project is a simple AI Virtual Assistant built using Python. It provides basic conversational capabilities, executes user commands like opening websites, fetching weather updates, and playing music, and includes a graphical user interface (GUI) for interaction.

Features
Text and Voice Interaction:

Users can interact via text input or voice commands.
The assistant responds with text and speech output.
Predefined Commands:

Greeting and Basic Responses: Answers questions like "What is your name?" or "How are you?".
Weather Updates: Fetches the current weather for a specific location.
Time Query: Tells the current time.
Google and YouTube Access: Opens Google or YouTube in a browser.
Music Playback:
Online music: Opens Gaana.com.
Offline music: Plays songs from a specified directory.
Shutdown: Closes the application upon user request.
GUI Interface:

Developed using Tkinter.
Includes buttons for sending text commands, initiating voice input, and clearing the chat history.
Text-to-Speech (TTS):

Converts assistant responses into audible speech using the pyttsx3 library.
Speech Recognition:

Converts user voice input into text using the speech_recognition library.
Weather Information:

Scrapes Google weather search results using the requests-html library.
Prerequisites
To run this project, ensure you have the following installed:

Python 3.x
Required Python libraries:
bash
Copy
Edit
pip install pyttsx3
pip install speechrecognition
pip install requests-html
pip install lxml
Project Modules
action.py
Handles all user commands and determines the appropriate response or action:

Interprets text or voice input.
Responds to commands like playing music, fetching weather, or opening websites.
speak.py
Implements the text-to-speech (TTS) functionality using pyttsx3.

spech_to_text.py
Converts voice input into text using the speech_recognition library. Includes error handling for cases of no internet or unrecognized speech.

weather.py
Fetches real-time weather updates for a specific location by scraping Google search results with the requests-html library.

Main GUI Script
Builds the graphical user interface using Tkinter:

Allows users to type or speak commands.
Displays the chat history in a text widget.
Includes buttons for "Ask," "Send," and "Delete."
How to Run
Clone this repository:
bash
Copy
Edit
git clone https://github.com/your-username/AI-Virtual-Assistant.git
Navigate to the project directory:
bash
Copy
Edit
cd AI-Virtual-Assistant
Run the main script:
bash
Copy
Edit
python main_gui.py
Directory Structure
bash
Copy
Edit
AI-Virtual-Assistant/
├── main_gui.py          # Main script to launch the application
├── action.py            # Handles user commands and responses
├── speak.py             # Text-to-speech functionality
├── spech_to_text.py     # Voice-to-text functionality
├── weather.py           # Fetches weather updates
├── image/
│   └── assistant.png    # Image used in the GUI
├── README.md            # Documentation
Future Enhancements
Add support for more commands, such as reminders or calendar events.
Improve natural language understanding with NLP libraries like SpaCy or GPT APIs.
Enhance the GUI design for a more modern look.
Support for multiple languages.
License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgments
Libraries used: pyttsx3, speech_recognition, requests-html, Tkinter
Inspired by the concept of virtual assistants like Alexa and Google Assistant


<img src="image/working.png" width="550" height="675">
