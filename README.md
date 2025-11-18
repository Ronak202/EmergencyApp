# 🚨 VNIT Smart Emergency Detection & Alert System  
### _AI-powered emergency classification, responder detection & WhatsApp alerting_

---

## 📌 Overview  
The **VNIT Smart Emergency System** is an AI-driven platform that detects emergencies from user text, classifies them into multiple categories, finds the nearest responders (hospital, police, fire station), and sends WhatsApp alerts to emergency contacts.

It uses **Sentence-Transformer embeddings**, **multi-label classification**, **Flask backend**, **MySQL**, **Geoapify**, and **Twilio WhatsApp API**.

---

## ✨ Features  

### 🧠 AI Classification  
- Multi-label classification for: **Health**, **Fire**, **Police**, **Non-emergency**  
- Subcategory detection: **Critical / Normal**  
- Embedding using `all-MiniLM-L6-v2` (Sentence-BERT)

### 📍 Responder Detection  
- Uses Geoapify Places API  
- Retrieves nearest hospital / fire station / police station  
- Auto-generates Google Maps links (view + embed)

### 📲 Emergency Alerts  
- Sends WhatsApp alert to:  
  - Personal number  
  - Two emergency contact numbers  
- Supports simulation mode (no Twilio cost)

### 🌐 Web App  
- User registration & login  
- Protected emergency dashboard  
- Panic trigger with location access  
- MySQL-based user storage

---

## 🧩 Project Structure

- **app.py**
- **train_model.py**
- **emergency_dataset.csv**

- **transformer_embedder.pkl**
- **main_model.pkl**
- **sub_model.pkl**
- **label_binarizer.pkl**
- **subcategory_encoder.pkl**

- **templates/**
- **static/**
- **signup/**

- **.env**
- **requirements.txt**
- **README.md**



---

## 📦 Installation  

### 1️⃣ Clone Repository  
```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
