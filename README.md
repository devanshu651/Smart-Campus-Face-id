# CampusEye AI – Smart Campus Face-ID Attendance System

A real-time, computer vision–based attendance system built as a **solo project** using Python.  
The goal is to automate manual attendance through face recognition while keeping the system simple, modular, and practical.

# 🚀 Features
- Real-time face detection and recognition via webcam  
- Automatic attendance logging with timestamps  
- Anti-duplicate entry logic within a defined time window  
- Streamlit-based dashboard for live monitoring  
- Lightweight SQLite database for persistence  

# 🛠 Tech Stack
- **Language:** Python  
- **Computer Vision:** OpenCV, `face_recognition` (dlib)  
- **Database:** SQLite  
- **UI:** Streamlit  

# 📁 Project Structure
```text
student_db/        # Face image dataset for encoding (prototype-scale, privacy-safe)
encoder.py         # Generates and serializes face encodings
data_cleaner.py    # Preprocessing and cleanup of face image data
db_init.py         # Initializes SQLite database schema
main_app.py        # Real-time recognition, attendance logic, and Streamlit UI

⚙️ How It Works 

- The system captures frames from a webcam, detects faces using OpenCV, generates 128-d face encodings using a dlib-based model, and compares them against stored encodings.
- On a successful match, attendance is logged with a timestamp in an SQLite database and reflected live on a Streamlit dashboard.

📌 Current Status
- Working prototype .
- Tested on a limited dataset for demonstration purposes .
- Runs locally .
- Designed to scale to multiple users without architectural changes .

🚧 Limitations
- Tested with a small dataset (privacy-safe prototype)
- Basic anti-spoofing is not yet implemented
- No cloud deployment in the current version

🔮 Planned Improvements
- Liveness / anti-spoofing checks
- Performance optimization for low-end devices
- Cleaner deployment workflow

🤖 AI Usage Disclosure
- AI tools were used as a mentor/assistant for ideation and documentation support.
- All core logic, system design, implementation, and debugging were done independently by me.

👤 Author
-Developed independently by a 1st-year B.Tech (AI/ML) student.
