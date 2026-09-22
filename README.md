# IoT-Based Practical Learning Assistant

An IoT-based educational platform designed to make practical learning more interactive, accessible, and engaging. The system combines IoT sensors, a web dashboard, and AI-powered assistance to help students perform experiments, monitor real-time data, understand results, and test their knowledge.

## 🚀 Features

* 📡 Real-time sensor data collection using ESP8266
* 🌡️ Temperature and humidity monitoring
* 📊 Interactive web dashboard
* 📖 Step-by-step practical experiment guidance
* 🤖 AI-powered explanations and learning assistance
* ❓ Interactive quizzes
* 📈 Student learning progress tracking
* 💡 Real-time feedback based on experiment results

## 🎯 Problem Statement

Students often perform practical experiments by following instructions without fully understanding the concepts behind the observations. Traditional practical learning may also lack real-time feedback and personalized guidance.

The **IoT-Based Practical Learning Assistant** aims to bridge this gap by combining physical experiments with IoT technology, interactive learning, and AI-based assistance.

## 💡 Proposed Solution

The system collects real-time data from sensors connected to an ESP8266 microcontroller. The collected data is sent through Wi-Fi to a web-based dashboard where students can observe experiment results.

The platform also provides explanations, quizzes, and AI assistance to help students understand the practical concepts behind the collected data.

## 🏗️ System Architecture

```text
             Student
                │
                ▼
       Practical Experiment
                │
                ▼
        ┌──────────────┐
        │    DHT11     │
        │    Sensor    │
        └──────┬───────┘
               │
               ▼
        ┌──────────────┐
        │   ESP8266    │
        │ Microcontroller│
        └──────┬───────┘
               │
              Wi-Fi
               │
               ▼
        ┌──────────────┐
        │   Backend    │
        │  / API Layer │
        └──────┬───────┘
               │
               ▼
        ┌──────────────┐
        │ Web Dashboard │
        └──────┬───────┘
               │
       ┌───────┴────────┐
       ▼                ▼
   Quiz System      AI Assistant
       │                │
       └───────┬────────┘
               ▼
        Student Progress
```

## 🛠️ Technologies Used

### Hardware

* ESP8266 NodeMCU
* DHT11 Temperature & Humidity Sensor
* Breadboard
* Jumper Wires
* LED / Buzzer

### Software

* HTML
* CSS
* JavaScript
* Python
* Flask
* Arduino IDE

### AI & Data

* Generative AI API
* Sensor data processing
* Student performance tracking

## 📂 Project Structure

```text
iot-practical-learning-assistant/
│
├── frontend/
│   ├── index.html
│   ├── style.css
│   └── script.js
│
├── backend/
│   └── app.py
│
├── esp8266/
│   └── sensor.ino
│
├── docs/
│   ├── architecture/
│   └── images/
│
└── README.md
```

## 🔄 How It Works

1. The student starts a practical experiment.
2. The DHT11 sensor collects temperature and humidity data.
3. ESP8266 processes the sensor readings.
4. ESP8266 sends the data through Wi-Fi.
5. The backend receives and processes the data.
6. The web dashboard di
