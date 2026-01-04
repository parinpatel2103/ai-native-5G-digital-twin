# 🤖 AI-Native 5G Base Station Receiver Trained with a Digital Twin

🎓 Senior Design / Honors Project — UT Austin  
👨‍🏫 Advisor: Prof. Kaushik Chowdhury  

---

## 📌 Overview
This project studies how an **AI-native 5G receiver** compares to a **traditional signal-processing receiver** when evaluated using a **realistic digital twin** of the UT Austin campus.

Instead of relying on simplified wireless channel models, we use physics-based simulation to better understand how receivers behave in real-world environments.

---

## 💡 Motivation (Why)
Wireless systems are often designed and tested under ideal assumptions that don’t fully capture real-world effects like:
- multipath propagation  
- blockage from buildings  
- interference from nearby transmitters  

The goal of this project is to explore whether **machine-learning-based receivers**, when trained on realistic digital-twin-generated data, can adapt better to these conditions than classical approaches.

---

## 🧠 System Design (What)
The system is designed as an end-to-end evaluation pipeline that includes:
- 🏙️ A 3D digital twin of the UT Austin campus  
- 📡 Physics-based wireless channel simulation  
- 📊 A traditional 5G receiver baseline  
- 🤖 An AI-native receiver architecture  
- 🧪 Hardware-in-the-loop validation using a channel emulator  

---

## 🛠️ The Process (How)

### 🏗️ Digital Twin & Channel Simulation
- Imported campus geometry using **OpenStreetMap** and **LiDAR data**
- Built a ray-tracing-based simulation environment using **NVIDIA Sionna**
- Generated channel impulse and frequency responses for different transmitter–receiver locations
- Verified that simulated propagation behavior matched expected physical trends

### 📶 Traditional Receiver Baseline
- Studied and implemented a classical 5G receiver chain
- Analyzed synchronization, channel estimation, equalization, and decoding stages
- Defined evaluation metrics such as **BER**, **BLER**, and **throughput** based on 3GPP standards

### 🤖 AI-Native Receiver Design
- Designed an ML-based receiver intended to replace parts of the classical decoding pipeline
- Defined data generation and training workflows using digital-twin-simulated channels
- Planned integration with **Keysight Propsim** and **OpenAirInterface** for testbed evaluation

---

## 🚦 Current Status
✔ Digital twin creation pipeline validated  
✔ Ray-tracing-based channel simulations verified  
✔ Traditional receiver baseline established  
✔ System architecture and evaluation plan defined  
⏳ AI model training and hardware integration in progress  

This repository documents the **system design, simulation validation, and risk reduction work** completed so far.

---

## 🧰 Tools & Technologies
- ⚡ NVIDIA Sionna (ray tracing & channel modeling)  
- 🐍 Python  
- 🧠 Machine learning frameworks (planned)  
- 📡 OpenAirInterface (5G stack)  
- 🧪 Keysight Propsim (channel emulation)  
- 🗺️ OpenStreetMap & LiDAR data  

---

## 📝 What I Learned
- How to translate wireless theory into a simulation-driven system design  
- How realistic channel modeling changes receiver behavior compared to idealized models  
- The importance of validating system components before full hardware deployment  
- How to fairly compare AI-based receivers with classical signal-processing methods  

---

## 🚀 Next Steps
- Train AI-native receiver models using digital-twin-generated datasets  
- Integrate both receivers into a hardware testbed  
- Compare performance under interference, mobility, and multipath conditions
