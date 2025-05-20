# HandSignRecognition-CV
A real-time emergency hand gesture detection system using OpenCV and MediaPipe. It identifies critical signs like fire alerts, medical emergencies, brake failure, violence at home, and help signals via webcam—enabling quick, silent responses in urgent situations.

# 🚨 Emergency Hand Sign Detection using OpenCV and MediaPipe

This project uses computer vision techniques to recognize **emergency hand signs** in real-time using a webcam feed. The recognized signs correspond to different critical situations such as fire alerts, medical emergencies, brake failures, and violence at home. This can help in **quickly notifying authorities or triggering alerts** without requiring verbal communication.

## ✨ Features

- 🔥 Detects **Fire Alert** signal using the Vulcan Salute gesture
- 🩺 Detects **Medical Emergency** hand posture
- 🚗 Detects **Brake Failure** alert sign
- 🆘 Detects **Violence at Home / Help** sign
- 🖐️ Recognizes Open Hand gesture for general Help alert
- 📹 Real-time detection using webcam and OpenCV
- ✋ Accurate finger position detection using **MediaPipe Hand Tracking**

---

## 🛠️ Tech Stack

- **Python**
- **OpenCV**
- **MediaPipe**
- **Math** (for distance calculations)

---

## 👨‍💻 Authors

- **Thoufiq Ahamed**
- **Zafeera F**
- **Syed Shabib Ahamed**

---

## 🚀 How it Works

The system uses MediaPipe to detect hand landmarks and then classifies gestures based on the position and orientation of fingers.

### Gesture Conditions

| Emergency Type        | Gesture Description                                                                 |
|-----------------------|--------------------------------------------------------------------------------------|
| 🔥 Fire Alert         | Vulcan salute-style gesture (space between fingers)                                 |
| 🩺 Medical Emergency  | All fingers above thumb (hand facing upward)                                        |
| 🆘 Violence at Home   | Thumb folded in with all fingers extended (common help signal)                      |
| 📢 Help Signal        | Open hand with significant distance between thumb and fingers                       |
| 🚗 Brake Failure      | Thumb and index finger extended, other fingers curled down                          |

---

## 🖥️ Installation and Running

### Prerequisites

- Python 3.x
- pip (Python package manager)

## 🔧 Setup Instructions
```bash
git clone https://github.com/your-username/emergency-hand-gesture-detection.git
cd emergency-hand-gesture-detection
pip install -r requirements.txt
python hand_sign_detection.py
