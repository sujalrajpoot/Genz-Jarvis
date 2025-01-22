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

This project is licensed under the MIT License. See the [LICENSE](https://github.com/sujalrajpoot/Genz-Jarvis/blob/main/LICENCE) file for details.

## Connect with Us

Made With 💓 By - Naman Singh Patel
