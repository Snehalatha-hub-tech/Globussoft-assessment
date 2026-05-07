# Globussoft AI Assessment

## 📌 Overview

This repository contains solutions for the Globussoft assessment. It includes:

* **Task 1:** Amazon Laptop Data Scraper
* **Task 2:** Face Authentication API using FastAPI

Both tasks are implemented in Python with a focus on simplicity, reliability, and clean structure.

---

# 🧩 Task 1: Amazon Laptop Scraper

## 🔍 Description

A Python script that scrapes laptop data from Amazon India and stores it in a CSV file.

## 📊 Extracted Fields

* Product Title
* Image URL
* Rating
* Price
* Ad / Organic Result

## ⚙️ How to Run

```bash
python task1.py
```

## 📁 Output

* CSV file saved with timestamp
* Example:

```
amazon_laptops_20260506_180610.csv
```

---

# 🧩 Task 2: Face Authentication API

## 🔍 Description

A FastAPI-based service that compares two face images and determines whether they belong to the same person.

## ⚙️ Features

* Accepts two images
* Processes images using OpenCV
* Computes similarity score
* Returns verification result

## 📥 Input

* Two face images (`image1`, `image2`)

## 📤 Output

```json
{
  "status": "success",
  "verification": "same person",
  "similarity_score": 0.82
}
```

---

## 🚀 How to Run

### 1. Install dependencies

```bash
pip install -r requirements.txt
```

### 2. Start FastAPI server

```bash
uvicorn app:app --reload
```

### 3. Open API Docs

```
http://127.0.0.1:8000/docs
```

---

# 🧠 Design Decisions

* Used OpenCV for lightweight and fast face comparison
* Avoided heavy models to ensure easy setup and reliability
* Designed API to be easily extendable with advanced models like InsightFace or FaceNet

---

# 📁 Project Structure

```
Globussoft-main/
│
├── task1.py
├── app.py
├── train.py
├── test.py
├── requirements.txt
├── README.md
├── image1.jpg
├── image2.jpg
└── venv/
```

---

# 📦 Requirements

* Python 3.11+
* fastapi
* uvicorn
* opencv-python
* numpy
* pillow
* requests
* beautifulsoup4
* python-multipart

---

# ⚠️ Notes

* The face comparison is based on image similarity (OpenCV)
* For production systems, deep learning models can be integrated
* Amazon scraping may occasionally fail due to anti-bot protection

---

# ✅ Conclusion

This project demonstrates:

* Web scraping skills
* API development using FastAPI
* Basic computer vision techniques

---

# 👩‍💻 Author

Haripriya K
