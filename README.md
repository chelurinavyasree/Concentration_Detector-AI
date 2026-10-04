# 🎯 Real-Time Concentration Detection System

A real-time AI-based concentration monitoring system using **Python**, **OpenCV**, and **MediaPipe**. This project detects user focus levels using webcam input by analyzing **blink detection**, **gaze direction**, and **head orientation** to compute a smooth **concentration score (1% to 100%)** dynamically.

---

## 📌 Features

- ✅ Real-time face tracking using MediaPipe
- 👁️ Eye blink detection using Eye Aspect Ratio (EAR)
- 🧿 Gaze direction estimation based on iris movement
- 🧠 Head pose-based attention tracking
- 📊 Real-time, continuous concentration score (1% to 100%)
- 📉 Score smoothing using history buffer
- 🔍 Face scanning effect in UI
- 🎯 Visual alerts: distraction count, blinking status, FPS indicator
- 🔴 Press `q` to exit the program

---

## 🛠️ Technologies Used

- **Python 3.9**
- **OpenCV**
- **MediaPipe**
- **NumPy**
- **deque** (from `collections` for score smoothing)

---

## 📦 Setup Instructions

1. **Clone this repository**
   ```bash
   git clone https://github.com/chelurinavyasree/Concentration_Detector-AI.git
   cd Concentration_Detector-AI
Install the required dependencies

bash
Copy
Edit
pip install opencv-python mediapipe numpy
Run the application

bash
Copy
Edit
python CSound.py
📊 How the System Works
Component	Functionality
Blink Detection	Detects frequent blinking using Eye Aspect Ratio (EAR)
Gaze Tracking	Estimates gaze direction using iris landmark coordinates
Head Orientation	Uses nose position to determine if head is facing forward
Concentration Score	Weighted average of blink, gaze, and head pose (1–100%)
Distraction Counter	Increments on continuous low concentration (< 40%)

💡 Visualization
📈 Concentration bar shows focus level with green (focused) and orange (distracted) colors

👁️ BLINKING status appears when user blinks

🔄 Face mesh and scanning overlay enhance UI feedback

📉 Distraction counter displayed when user loses focus

⏱️ FPS and live activity status (ACTIVE/DISTRACTED) shown in top-right corner

🎨 Customization
Score Thresholds: Currently, 40% is used as the distraction threshold

Score History: Adjustable smoothing via deque(maxlen=10)

Visual UI: Customize colors, fonts, and messages in the code

👨‍💻 Author
Prepared by:
Navya Sree
GitHub: https://github.com/chelurinavyasree


🙌 Acknowledgments
Google MediaPipe

OpenCV

Educational resources and online documentation

📝 License
This project is open-source and free to use for academic and non-commercial research purposes.

