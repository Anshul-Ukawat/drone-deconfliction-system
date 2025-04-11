# 🛰️ Drone Deconfliction System

Strategic 4D deconfliction and simulation for autonomous drone flight planning.  
This system verifies the safety of a drone’s waypoint mission in shared airspace by checking for spatial and temporal conflicts with other drones — with **AI integration**, **automated tests**, and **4D visualization**.

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)
![License](https://img.shields.io/badge/License-MIT-green)
![Tests](https://img.shields.io/badge/Tests-Automated-success)
![AI](https://img.shields.io/badge/AI-RandomForest-informational)

---

## 📸 Demo

<img src="https://user-images.githubusercontent.com/demo-visual.gif" alt="Demo" width="600"/>

> 🔗 Demo Video: [YouTube Link Here](https://www.youtube.com/your-demo)

---

## 📦 Features

- ✅ **Waypoint Mission Validation** (Spatial + Temporal)
- 🧠 **AI Conflict Predictor** using Random Forest Classifier
- 🔁 **Automated Tests** for various conflict cases
- 📊 **Interactive Simulation & 4D Visualization** (x, y, z, t)
- 🗂️ **Modular, Scalable Design**
- ☁️ **Future-ready for real-time multi-drone scenarios**

---

## 🗂️ Folder Structure

drone-deconfliction-system/<br> 
├── main.py # Entry point <br>
  ├── ai_conflict_predictor.py # AI-based classifier module <br>
├── conflict_checker.py # Spatial & temporal checks <br>
├── simulator.py # Drone path simulation logic <br>
├── visualizer.py # 2D/3D/4D visualization functions <br>
├── test_conflict_checker.py # Automated tests using unittest <br>
├── data/ <br>
│ ├── primary_mission.json # Primary drone flight plan <br>
│ └── other_flights.json # Simulated drone flight schedules<br> 
├── README.md <br>
└── Reflection.md # Design decisions & architecture<br>

---

## 🚀 How to Run

### 1. 📥 Clone the Repo
```bash
git clone https://github.com/yourusername/drone-deconfliction-system.git
cd drone-deconfliction-system
```
### 2. 🐍 Install Dependencies
```bash
pip install -r requirements.txt
```
### 3. ▶️ Run the Main Program
```bash
python main.py
```

---
## 🔬 Testing
```bash
python -m unittest test_conflict_checker.py
```
Includes tests for:

- ✅ Conflict-free missions
- 🕒 Time-only conflicts
- 📍 Space-only conflicts
- 🔄 Combined space-time violations
- ⚠️ Edge buffer overlaps

---
## 🧠 AI Integration
This system uses a Random Forest Classifier as an AI-powered pre-check to quickly classify whether a mission is likely to be safe or conflicted. It helps optimize performance before expensive detailed checks.<br>
Highlights:<br>
- 🧬 **Feature Engineering** on mission overlap, speed, spacing, and time windows  
- 🧪 **Trained on Synthetic Conflict Data** to simulate real-world scenarios  
- ⚡ **Fast Filtering Layer**: Skips detailed checks on clearly safe or clearly conflicting missions  

---
## 🌍 Scalability Strategy
To scale this to handle tens of thousands of drones:
- ⚙️ Distributed Conflict Checking (e.g., using Apache Kafka + Dask)
-📡 Real-Time Data Ingestion from drone APIs or edge devices
- ☁️ Cloud Deployment (e.g., AWS Lambda + S3 + DynamoDB)
- 🧠 AI Model Optimization via continual learning or federated learning
More detail in Reflection.md

---
## 📝 License
MIT License – free to use, modify, and distribute.

## ⭐ Feedback & Contributions
Pull requests and issue reports are welcome!<br>
If you like the project, give it a ⭐ and share it!
