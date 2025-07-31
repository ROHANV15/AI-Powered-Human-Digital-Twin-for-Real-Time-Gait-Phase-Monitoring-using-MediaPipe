
# 🧠 AI-Powered Human Digital Twin for Real-Time Gait Phase Monitoring using MediaPipe

This project presents a real-time **Human Digital Twin system** that analyzes and monitors key gait phases such as **heel-strike**, **knee extension**, **stride symmetry**, and **arm swing**. The system uses **MediaPipe Pose Estimation** to extract skeletal joint landmarks from video input and applies **rule-based AI logic** to assess biomechanical gait patterns.

## 🧪 Project Summary

- 🔬 **Domain**: Healthcare / Biomedical Engineering / Computer Vision  
- 🧠 **Core Technology**: MediaPipe Pose + OpenCV + Numpy  
- 🧮 **Model Type**: Rule-Based Gait Phase Analysis using 3D joint tracking  
- 📹 **Input**: Video of walking subject (`gait_video.mp4`)  
- 🗂️ **Output**: Frame-wise feedback on gait parameters (`gait_feedback_log.txt`)



## 🚀 Features

- ✅ Real-time joint tracking using **MediaPipe Pose**
- ✅ Visualizes a **Digital Twin** using line rendering
- ✅ Detects and logs:
  - Heel Strike
  - Knee Extension
  - Stride Symmetry
  - Arm Swing
- ✅ Saves gait report to a log file for further evaluation


## 📁 Project Structure

human-digital-twin-gait-monitoring/
├── src/
│ ├── main.py # Main execution file
│ ├── digital_twin.py # Draws pose lines (Digital Twin)
│ ├── gait_analysis.py # Rule-based gait phase logic
│ ├── gait_video.mp4 # Input walking video
│ └── gait_feedback_log.txt # Generated log with analysis
├── LICENSE # MIT License
└── README.md # You're reading it!


## ⚙️ Installation

### Requirements

```bash
pip install opencv-python mediapipe numpy
▶️ How to Run
Place your walking video as gait_video.mp4 in the src/ folder.

Run the program:

cd src
python main.py
You will see:

The digital twin rendered live.

Terminal output of detected gait events.

A file named gait_feedback_log.txt containing feedback per frame.

📊 Gait Parameters Tracked

Heel Strike	---Checks for minimum foot height near ground using heel and hip position
Knee Extension	---Measures angle between hip–knee–ankle landmarks
Stride Symmetry	---Compares hip–knee movement across frames for both legs
Arm Swing	---Tracks wrist-shoulder displacement across time

👨‍⚕️ Applications
Post-surgical rehabilitation (e.g., knee replacements)

Fall risk detection in elderly patients

Remote physiotherapy assistance

Sports injury recovery tracking

🎯 Future Enhancements
Deep learning model to automatically classify abnormal gait

Real-time feedback to mobile or web dashboards

Integration with IMU sensor data

📜 License
This project is licensed under the MIT License.


👨‍💻 Author
[ROHAN V]
EMAIL: rohanvoff@gmail.com
