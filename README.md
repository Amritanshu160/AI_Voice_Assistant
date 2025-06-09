# 🤖 AI Voice Assistant - Carlo

**Carlo** is a Python-based desktop voice assistant capable of performing various tasks such as searching Wikipedia, opening websites, playing music, reporting the time, and sending emails — all through voice commands.

---

## 🎯 Features

- Text-to-speech with `pyttsx3`
- Voice recognition using Google’s speech recognition API
- Wikipedia search and summary reading
- Opens common websites like YouTube, Google, and Stack Overflow
- Plays local music from a specified directory
- Tells the current time
- Sends emails through Gmail

---

## 🛠️ Tech Stack

- Python 3.x
- pyttsx3
- speechRecognition
- wikipedia
- smtplib
- webbrowser
- os
- datetime

---

## 📁 File Structure

```
AI_Voice_Assistant/
├── Ai_Mini_.py        # Main Python script for voice assistant
└── README.md          # Project documentation
```

---

## 🧪 Setup Instructions

### 🔧 Prerequisites

Make sure you have Python 3.x installed and install the required libraries:

```bash
pip install pyttsx3 SpeechRecognition wikipedia
```

### ⚙️ Running the Assistant

Simply run the Python script:

```bash
python Ai_Mini_.py
```

> The assistant will greet you and start listening for voice commands.

---

## 🔐 Email Configuration Warning

This script currently includes **hardcoded Gmail credentials** in `sendEmail()`:
```python
server.login('your_email@gmail.com', 'your_password')
```

> **⚠️ WARNING:** Hardcoding credentials is insecure.  
> Use environment variables or encrypted secrets in production.

To send emails:
1. Enable "Less secure app access" or use **App Passwords** in Gmail.
2. Replace the email and password in the script with your secure method.

---

## 🎤 Sample Commands

- "Open YouTube"
- "Search Albert Einstein"
- "What’s the time?"
- "Open Google"
- "Play music"
- "Email to Shubham"

---

## 🧠 Logic Overview

- **`wishMe()`**: Greets user based on the time of day
- **`takeCommand()`**: Uses microphone to take speech input and convert it to text
- **`speak()`**: Converts text to speech
- **`sendEmail()`**: Sends an email using SMTP
- **Main Loop**: Continuously listens for commands and executes matched logic

---

## 👤 Author

**Amritanshu Bhardwaj**  
AI & Data Science, BMS College of Engineering  

---
