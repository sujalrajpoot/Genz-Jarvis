# Genz Jarvis

## Project Overview

**Genz Jarvis** is an advanced AI project designed to integrate multiple AI capabilities, including speech recognition, text processing, and image analysis, into a cohesive system. Named after the iconic AI assistant from popular culture, Jarvis is built with cutting-edge natural language processing capabilities, allowing users to interact with it through voice commands. Whether it's checking the weather, setting reminders, managing calendars, or searching the web, Jarvis is equipped to handle a wide range of tasks efficiently and effectively. With its intuitive interface and robust functionality, Jarvis aims to revolutionize the way users engage with technology, making everyday tasks simpler and more convenient.

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Directory Structure](#directory-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Connect with Us](#connect-with-us)

## Features

- **Speech Recognition**: Convert spoken language into text using various models.
- **Text Processing**: Analyze and generate text with multiple AI tools.
- **Image Analysis**: Perform image recognition and processing tasks.
- **Audio Tools**: Detect hotwords and manage audio playback interruptions.
- **Interactive Prompts**: Predefined prompts to guide AI interactions.

## **Features & Descriptions**

- **Open/Close Applications**  
  Launch or exit any installed software using voice or typed commands for quick multitasking.

- **Volume Controller**  
  Adjust system volume with commands like "increase volume" or "mute sound".

- **Music Player**  
  Play, pause, skip, or queue your favorite songs using simple commands.

- **Image Generation**  
  Generate AI-powered images from text prompts using built-in image generation tools.

- **Send Messages**  
  Send text messages or emails through integrated platforms like WhatsApp, SMS, or Gmail.

- **Schedule Reminder**  
  Set reminders for tasks, events, or deadlines that alert you via notifications or voice.

- **Check Latest Messages on Social Media**  
  Fetch and read recent DMs or notifications from platforms like Instagram, WhatsApp, or Messenger.

- **Google Calendar Manager**  
  Add, view, or delete calendar events using natural language instructions.

- **Screenshot**  
  Capture full-screen or custom-area screenshots instantly with optional naming or storage path.

- **Email Reader & Sender**  
  Read unread emails aloud and compose new emails through voice or text input.

- **Weather & News Briefing**  
  Get real-time weather updates and daily news summaries tailored to your preferences.

- **Clipboard Manager**  
  Access and manage your recent clipboard history to retrieve copied content easily.

- **Daily Planner**  
  Generate a smart summary of your day's meetings, tasks, and reminders in one view.

- **Habit Tracker**  
  Log, monitor, and remind yourself of daily routines like hydration, workouts, or reading.

- **Custom Greetings**  
  Personalized greetings based on time, mood, events, or even your energy level for the day.

- **Voice Cloning / Custom Wake Word**  
  Personalize Jarvis with a custom wake word and optionally clone your voice or a celebrity voice.

- **Chat Memory**  
  Let Jarvis remember context from past chats (mood, preferences, task patterns) to feel more human.

- **AI-Powered Note Summarizer**  
  Auto-summarize long notes, documents, or meeting transcripts.

- **Task Prioritizer with Urgency Detection**  
  Analyze tasks and rank them by deadlines, urgency, or user-defined priority. 

### **Coding & Development Tools**
- **Local Dev Assistant**  
  Help write, debug, and run code; suggest libraries, functions, or logic based on input.

- **Git Assistant**  
  Manage Git commits, branches, push/pull, etc., using natural language.

### **System & Performance Tools**
- **Battery & Resource Monitor**  
  Get system usage updates, memory usage, or alerts when something consumes too much power.

- **Auto System Cleaner**  
  Suggest or run cleanup routines: clear temp files, recycle bin, unused files, etc.

### **Voice & Gesture Control**
- **Gesture Command Integration**  
  Use hand gestures (via webcam or sensors) to control music, volume, or slides.

- **Emotion Recognition (via Camera)**  
  Detect mood using facial cues and adjust responses, lighting, or music accordingly.

### **Smart Life Integrations**
- **Expense Tracker**  
  Log expenses, categorize spending, and generate monthly spending reports.

- **AI Journal**  
  Speak or type thoughts, and Jarvis stores them in a private, timestamped journal.

- **Motivational Coach**  
  Daily quotes, affirmations, or even pep talks based on how you’re feeling.

- **Mood-Based Music & Lighting Suggestions**  
  Detect your mood and auto-suggest songs or adjust smart lights accordingly.

- **Focus Mode / Pomodoro Assistant**  
  Manage work-break intervals with focus timers and ambient sounds.

- **To-Do List Organizer with AI Suggestions**  
  Create smart tasks with suggestions based on time, past habits, and urgency.

- **Meeting Summarizer (Live or Recorded)**  
  Transcribe and summarize your meetings automatically.

- **File Search & Open via Voice**  
  Search for documents, media, or files using voice queries.

- **Language Translator & Pronunciation Coach**  
  Real-time translations and voice practice for learning new languages.

- **Book Summarizer & Tracker**  
  Summarize books or articles and track what you’ve read or want to read.

- **Voice-Based Navigation:**  
  - “Click on ‘Submit’ button”  
  - “Scroll down” / “Go to top”  
  - “Search for ‘Python tutorials’ on this page”  
  - “Next tab” / “Close current window”  
  - “Zoom in/out”

- **Gesture-Based Actions (using webcam or hand-tracking):**  
  - Swipe left/right = Switch tabs  
  - Hand raise = Pause media  
  - Pinch in/out = Zoom  
  - Point = Move cursor  
  - Double tap gesture = Click  
  - Circle motion = Scroll

- **Voice-Controlled Keyboard Shortcuts You say:**
  - “Press Control + C” → Jarvis simulates copy
  - “Press Alt + F4” → Jarvis closes the current window
  - “Press Windows + D” → Minimize all and show desktop

- **Website Summarizer (Voice Command Example):**
    
    "Jarvis, summarize this page"

    Jarvis fetches the visible text or entire page content, then summarizes it using an LLM (like GPT or local model).

- **Voice Navigation on Any Website**

    > *"Go to Wikipedia dot org"*  
    > *"Search Python programming"*  
    > *"Scroll down"*  
    > *"Zoom in"*  
    > *"Click the first link"*

### **Example Flow:**

#### Step-by-step use case:
    1. Open YouTube and search for lo-fi music
    2. Interact with search box
    3. Voice Scroll & Click
    Bonus: Visual Pointer + Voice Click

**Let Jarvis highlight clickable elements (links/buttons) and say:**
- *"Click button 2"*

## Directory Structure

The project is organized into several key directories:

```
Genz Jarvis/
├── assets
│   ├── activation_sound.wav
│   ├── conversation_history.json
│   ├── current_image.jpg        
│   ├── deactivation_sound.wav   
│   ├── generated_image.jpg   
│   ├── leonardo_cookies.json 
│   ├── leonardo_response.json
│   ├── stt.html
│   └── todo_list.txt
├── config
│   └── tools_config.py       
├── core
│   ├── assistant.py
│   ├── conversation.py       
│   ├── stream
│   │   ├── text
│   │   │   └── deepinfra.py  
│   │   └── tts
│   │       └── deepgram.py
│   ├── stt.py
│   ├── system_instructions.py
│   ├── tts.py
│   └── vosk_recog.py
├── functions
│   ├── RawDog.py
│   ├── camera_vision.py      
│   ├── control_volume.py     
│   ├── currency_ops.py       
│   ├── datetime.py
│   ├── file_ops.py
│   ├── generate_image.py     
│   ├── note_ops.py
│   ├── play_on_youtube.py    
│   ├── system_ops.py
│   ├── to_do_list_manager.py 
│   ├── weather_ops.py        
│   ├── web_search.py
│   └── website_assistant.py  
├── tools
│   ├── Hotword_Detection.py
│   ├── Interrupted_Playsound.py
│   └── Jarvis_Telegram_Bot.py
├── utils
│   ├── colors.py
│   ├── history_manager.py
│   ├── logger.py
│   └── message_formatter.py
├── .env  
├── README
├── main.py
├── requirements.txt
└── test.py
```

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/sujalrajpoot/Genz-Jarvis.git
   cd Genz-Jarvis
   ```

2. **Install the required packages**:
   ```bash
   pip install -r requirements.txt
   ```

3. **(Optional) Install Vosk Speech Recognition Models**:

   Vosk provides pre-trained models for various languages. To install the models for your desired language, follow these steps:

   - Go to the Vosk GitHub repository releases page: [Vosk GitHub Releases](https://github.com/alphacep/vosk-api/releases)
   - Download the model folder for your language. For example, if you want English models, download the folder named `vosk-model-en-us-aspire-0.2` You can visit here [Vosk Models](https://alphacephei.com/vosk/models).
   - Extract the contents of the folder into a directory named `ASSETS` in your project directory.
   - Ensure that the extracted model folder is directly under the `ASSETS` directory, without any additional nesting.
   - Now, you should have a structure like this: `<your-main-project-directory>/ASSETS/vosk-model-en-us-aspire-0.2`.
   - Modify the `main.py` or any relevant script to point to the model directory. For example:
     ```python
     from ENGINE.STT.vosk_recog import speech_to_text

     for speech in speech_to_text(model_path="assets\vosk-model-small-en-us-0.15"):
         if speech != "":
             print("Human >>", speech)
     ```  

## Usage

1. **Run the main script**:
   ```bash
   python main.py
   ```

2. **Configuration**: Modify API configuration

 in the `.env` directory to suit your needs.

## Contributing

We welcome contributions to improve Genz-Jarvis. To contribute, follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a new Pull Request.

## License

This project is licensed under the MIT License. See the [LICENSE](https://github.com/sujalrajpoot/Genz-Jarvis/blob/main/LICENSE) file for details.

## Connect with Us

Made With 💓 By - Naman Singh Patel
