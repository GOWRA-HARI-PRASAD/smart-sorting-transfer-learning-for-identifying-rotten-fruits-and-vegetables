

# Smart Sorting & Transfer Learning for Identifying Rotten Fruits and Vegetables

## 🚀 Project Overview

This project leverages machine learning and IoT technologies to automatically **detect and sort rotten fruits and vegetables**. It uses **Transfer Learning** to classify images, and a **servo-controlled sorting mechanism** to physically separate good from spoiled produce.

## 📌 Objectives

- Automatically identify rotten fruits and vegetables.
- Control a mechanical system to sort produce based on prediction.
- Display classification results on a real-time dashboard.
- Improve efficiency in food quality monitoring and reduce human labor.

---

## 📷 Features

- 🍎 Image-based classification using pre-trained models like MobileNet or ResNet.
- 🤖 Servo motor control for physical sorting.
- 📊 Real-time dashboard to view classification logs.
- 🛠 Arduino/Raspberry Pi integration for hardware control.
- ☁️ Scalable to cloud or local environments.

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|------------|
| **Frontend** | HTML, CSS, JavaScript, React.js |
| **Backend** | Python (Flask / Django) |
| **Machine Learning** | TensorFlow / Keras with MobileNetV2 |
| **Database** | SQLite / Firebase |
| **Microcontroller** | Arduino UNO / Raspberry Pi |
| **Cloud (Optional)** | Firebase, IBM Cloud, AWS |
| **Others** | OpenCV, NumPy, Pandas |

---

## 🧠 Machine Learning Model

- **Model Used**: Transfer Learning with MobileNetV2 or ResNet50
- **Classes**: `Fresh`, `Rotten`
- **Tools**: TensorFlow, Keras
- **Training Dataset**: Fruits and vegetables image dataset (can be custom or public dataset)

---

## 🧩 Architecture

User (Camera Input or Upload)
↓
Frontend Interface (Web / Mobile)
↓
Python Backend (Classification + Motor Control)
↓
TensorFlow Model (Transfer Learning)
↓
Decision
├── Fresh → Servo Channel A
└── Rotten → Servo Channel B
↓
Database Logging + Dashboard

yaml
Copy
Edit

---

## 📁 Folder Structure

📦 smart-sorting-project
├── model/
│ └── trained_model.h5
├── arduino/
│ └── servo_sorting.ino
├── backend/
│ └── app.py
│ └── utils.py
├── frontend/
│ └── index.html
│ └── script.js
├── static/
│ └── images/
├── templates/
│ └── dashboard.html
├── data/
│ └── dataset/
└── README.md

yaml
Copy
Edit

---

## 🚦 How to Run the Project

### 🔧 Prerequisites

- Python 3.8+
- Arduino IDE (for uploading `.ino` file)
- TensorFlow, Flask
- USB Cable for microcontroller connection

### ▶️ Steps

```bash
# Clone the repository
git clone https://github.com/your-username/smart-sorting-project.git
cd smart-sorting-project

# Create virtual environment and activate it
python -m venv venv
source venv/bin/activate  # On Windows use venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run backend server
cd backend
python app.py
Open browser at http://127.0.0.1:5000 to view dashboard.

Upload fruit/veg image or use real-time input.

Watch classification results and servo motor actions.

💡 Future Enhancements
Integrate real-time camera for continuous scanning.

Add MQTT or Bluetooth for wireless control.

Train model with more produce types (multi-class classification).

Cloud-based analytics dashboard.

📜 License
This project is licensed under the MIT License.

🙋‍♂️ Team
Team ID: LTVIP2025TMID35093

Project Date: 15 February 2025

🙏 Acknowledgements
TensorFlow for ML support

Arduino for embedded hardware control

IBM Cloud & Firebase for backend options

Faculty and mentors for project guidance
