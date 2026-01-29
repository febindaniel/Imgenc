# 🖼️ Imgenc – Secure Steganography App

**Imgenc** is a secure steganography application that allows users to **hide encrypted text or files inside images**.
It combines **cryptography and steganography** to ensure both **data confidentiality and concealment**, making it suitable for secure data handling and educational cybersecurity use cases.

The application uses a **Flutter-based desktop interface** with a **Python backend** for encryption and image processing.

---

## ✨ Features

* 🔐 Embed text messages or files inside PNG/BMP images
* 🔑 AES-256 encryption using a password-derived key
* 📦 Automatic capacity calculation based on image size
* 🌙 Modern Flutter UI with dark-mode support
* 🧠 Python backend for secure cryptographic operations

---

## 🛠 Tech Stack

* **Frontend:** Flutter (Windows Desktop)
* **Backend:** Python (Flask API)
* **Security:**

  * AES-256 (CBC / GCM)
  * SHA-256 hashing
  * Zlib compression

---

## ⚡ Quick Start (Windows)

The easiest way to run the application is using the provided PowerShell launcher.

1. Right-click **`run_app.ps1`**
2. Select **“Run with PowerShell”**
3. The script will:

   * Install required Python dependencies (first run only)
   * Start the local backend server
   * Launch the Flutter desktop application

> **Note:** Ensure **Python** and **Flutter** are installed and added to your system PATH.

---

## 📦 Build for Release (Windows)

To generate a portable Windows build:

1. Right-click **`build_release.ps1`**
2. Select **“Run with PowerShell”**
3. After completion, find the output in:

   ```
   Imgenc_Release/
   ```

The generated folder can be zipped and run on other Windows systems without requiring Flutter.

---

## 🔧 Manual Setup

### Backend (Python)

```bash
cd backend
python -m venv venv
.\venv\Scripts\activate
pip install -r requirements.txt
python app.py
```

The backend runs at:

```
http://127.0.0.1:5000
```

---

### Frontend (Flutter)

```bash
cd frontend
flutter pub get
flutter run -d windows
```

---

## 📚 Learning Outcomes

* Practical implementation of **AES-based encryption**
* Understanding of **image steganography techniques**
* Secure file handling using Python
* Cross-platform desktop UI development with Flutter
* Integration of frontend and backend systems


---

## ⚠️ Disclaimer

This project is developed **for educational and learning purposes only**.
It should not be used for illegal or unauthorized data concealment.

---

## 📄 License

MIT License — free to use and modify.

---
