# Student-face-recognition-system
Developed a student face recognition system using computer vision and machine learning to automate attendance and enhance campus security. Implemented real-time face detection and recognition with high accuracy, reducing manual efforts and improving efficiency in tracking student presence.     
Facerecognition
Face recognition is a biometric technology that identifies or verifies a person by analyzing and comparing patterns based on their facial features. It uses advanced computer vision and deep learning algorithms to detect faces in images or video and match them with stored face data.

🎯 Face Recognition Attendance System
A real-time face recognition-based attendance system using OpenCV, Flask, and optionally the Buffalo model (InsightFace) for robust face detection and recognition.

📸 Features
Real-time face detection and recognition using webcam
Attendance logging with timestamp
Face dataset creation
Preprocessing with face alignment (optional)
Flask web interface for ease of access
CSV-based attendance record keeping
Optionally uses InsightFace (Buffalo) for advanced recognition
🧠 Tech Stack
Python
OpenCV
Flask
InsightFace (optional: RetinaFace + ArcFace)
NumPy
Pandas
SQLite or CSV for storing data
⚙ Installation
Clone the repository
git clone https://github.com/sreelekhakummetha/face-recognition-attendance.git
cd face-recognition-attendance
Create and activate virtual environment (optional)
python -m venv venv source venv/bin/activate # On Windows: venv\Scripts\activate

Install dependencies
pip install -r requirements.txt

Download Pretrained Models (if using InsightFace)
Face Detection: RetinaFace

Face Recognition: ArcFace

🚀 Running the App

python app.py

Open http://127.0.0.1:5000 in your browser.

Use the UI to register a face or take attendance.

✅ How It Works

Registration
Capture face images with the user's name.

Save the cropped and aligned faces into dataset/.

Training (if using own embeddings)
Extract embeddings for all registered faces and store them.

Recognition
During live detection, compare current embedding with stored ones using cosine similarity.

Mark attendance if match is found and not already marked.

Attendance
Attendance is saved in attendance.csv with:

Name

Time

Date

📦 Requirements

Python 3.7+

OpenCV

Flask

NumPy

Pandas

insightface (if using Buffalo model)

📄 Example .csv Output

Name,Date,Time Sreelekha,03/08/2025,10:32:17 Lokeswarreddy,03/08/2025,10:32:45

🛡 License

This project is licensed under the MIT License - see the LICENSE file for details.

🙏 Acknowledgements

OpenCV

InsightFace by DeepInsight

Flask
