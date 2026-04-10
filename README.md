# 🚗 Driver Drowsiness Detection System

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![OpenCV](https://img.shields.io/badge/OpenCV-Computer%20Vision-green?logo=opencv)
![MediaPipe](https://img.shields.io/badge/MediaPipe-FaceMesh-orange)
![Status](https://img.shields.io/badge/Status-Active-success)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

A real-time computer vision system designed to detect driver fatigue and enhance road safety by monitoring eye activity and triggering alerts when drowsiness is detected.


## 🛠️ Technologies Used

- Python  
- OpenCV  
- MediaPipe  
- Pygame (for audio alerts)  
- PySerial (for Arduino communication)  
- Jupyter Notebook  


## ▶️ How to Run

## 1. Clone the Repository

Clone the project repository from GitHub:

```bash
git clone https://github.com/your-username/driver-drowsiness-detection.git
```
Navigate into the project directory:

```bash
cd driver-drowsiness-detection
```

## 2. Create a Virtual Environment

```bash
python -m venv venv
```

## 3. Activate the Virtual Environment

**Windows:**

```bash
venv\Scripts\activate
```

**macOS/Linux:**

```bash
source venv/bin/activate
```

## 4. Install Dependencies

```bash
pip install -r requirements.txt
```

## 5. Install JupyterLab to run cells easly

```bash
pip install jupyterlab
```

## 6. Run JupyterLab

```bash
jupyter lab
```

## 7. Open the Notebook

```bash
drowsiness_detection.ipynb
```
---

## 🔊 Important Notes

- Ensure `alarm.mp3` is in the same folder as the notebook  
- Webcam access is required  
- Do not rename files unless paths are updated in the code  
- For Arduino:
  - Configure the correct COM port  




---

## ⚙️ Key Features

- 🎥 Real-time face and eye tracking using computer vision  
- 👁️ Eye Aspect Ratio (EAR) for blink and drowsiness detection  
- ⏱️ Threshold-based fatigue detection:  
  - EAR < 0.25 → eyes considered closed  
  - Alert triggered after ~2 seconds  
- 🔊 Audio alert system using alarm sound  
- 🔌 Optional Arduino integration for physical buzzer alerts  
- ⚡ Low-latency processing (edge AI approach)  

---



## 📄 Files Description
```plaintext
driver-drowsiness-detection/
│
├── drowsiness_detection.ipynb
├── requirements.txt
├── alarm.mp3
├── README.md
├── instruction.pdf
├── SleepDetect-ARDUINO.ino
└── face-detection-steps.pdf
```

### 🧠 `drowsiness_detection.ipynb`
- Main project notebook containing the full system logic  
- Implements:
  - Camera initialization  
  - Face landmark detection using MediaPipe  
  - Eye Aspect Ratio (EAR) calculation  
- Includes fatigue detection logic:
  - Detects eye closure duration  
  - Triggers alert after ~2 seconds  
- Supports:
  - 🔊 Audio alert using Pygame  
  - 🔌 Hardware alert via Arduino (PySerial)  

---

### 📦 `requirements.txt`
- Contains all required Python dependencies  
- Ensures reproducibility of the environment  
- Key libraries:
  - `opencv-python`  
  - `mediapipe==0.10.9`  
  - `pygame`  
  - `pyserial`  

---

### 🔊 `alarme.mp3`
- Audio file used for the alert system  
- Played when drowsiness is detected  
- Must remain in the same directory as the notebook  

---

### 📘 `instruction.pdf`
- Step-by-step setup guide  
- Explains:
  - Virtual environment creation  
  - Dependency installation  
  - How to run the project  
- Includes important usage notes and warnings  

---

### 🔌 `SleepDetect-ARDUINO-.ino`
- Arduino code for physical buzzer alert  
- Uses serial communication:
  - `'1'` → turn buzzer ON  
  - `'0'` → turn buzzer OFF  
- Configured to control buzzer via a digital pin  ( change the pin based on your circuit )

---

### 📑 `face-detection-steps.pdf`
- Detailed project development guide  
- Covers step-by-step implementation:
  - Face detection  
  - EAR calculation  
  - Fatigue detection logic  
- Includes code snippets for each stage  

---




## 👨‍💻 Author

**Marwane Haddane**  
Robotics & Embedded Systems Enthusiast 🤖  
Cybersecurity Engineer 🔐  

---

## ⭐ Support

If you like this project:

- ⭐ Star the repo  
- 🍴 Fork it  
- 🧠 Share ideas & improvements  




