# 🌿 Plant Disease Classification API (Deep Learning + FastAPI)

## 📌 Overview

This project is a **Deep Learning-based web API** that classifies plant leaf diseases from images.  
The model is trained using TensorFlow/Keras and deployed using FastAPI to provide real-time predictions.

---

## 🚀 Features

* 🌱 Classifies plant diseases from leaf images  
* ⚡ FastAPI-based REST API for real-time inference  
* 📤 File upload support (image input)  
* 📊 Returns predicted class with confidence score  
* 🔥 Ready for deployment (Render / Cloud platforms)  

---

## 🧠 Model Details

* Framework: TensorFlow / Keras  
* Model Format: `.keras`  
* Classes:  
  * Early Blight  
  * Late Blight  
  * Healthy  

---

## 🛠️ Tech Stack

* Python  
* FastAPI  
* TensorFlow / Keras  
* NumPy  
* Pillow  
* Uvicorn  

---

## 📂 Project Structure

```
project/
│── app/
│   └── main.py
│── model/
│   └── model.keras
│── requirements.txt
│── README.md
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the repository

```
git clone <https://github.com/SATYABRATA-cloud/Potato-plant-disease-detection-model>
cd project
```

---

### 2️⃣ Create virtual environment

```
python -m venv venv
venv\Scripts\activate   # Windows
```

---

### 3️⃣ Install dependencies

```
pip install -r requirements.txt
```

---

### 4️⃣ Run the API

```
uvicorn app.main:app --reload
```

---

### 5️⃣ Open in browser

```
http://localhost:8000/docs
```

👉 Use the `/predict` endpoint to upload an image and get prediction.

---

## 📡 API Endpoints

### 🔹 GET `/`

Check if API is running  

**Response:**

```
"Hello, I am alive"
```

---

### 🔹 POST `/predict`

Upload an image file for prediction  

**Request:**

* Form-data  
* Key: `file`  
* Value: Image file  

**Response:**

```
{
  "class": "Early Blight",
  "confidence": 0.97
}
```

---

## 🖼️ Image Preprocessing

* Resized to model input size (e.g., 224×224)  
* Normalized (pixel values scaled to 0–1)  

---

## 🌐 Deployment

This API can be deployed on:

* Render  
 

---



## 👨‍💻 Author

**Satyabrata Nayak**

---

## ⭐ Acknowledgements

* TensorFlow Documentation  
* FastAPI Documentation  
* Open-source datasets  
