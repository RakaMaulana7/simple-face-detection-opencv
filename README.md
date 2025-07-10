# 😊 Simple Face Detection using OpenCV

This repository contains a basic real-time face and eye detection system using OpenCV and Haar Cascade classifiers. It is designed to demonstrate the fundamentals of computer vision for detecting facial features using Python.

---

## 📌 Features

- 👤 Real-time face detection with Haar Cascade
- 👁️ Eye detection within detected face regions
- 📷 Supports webcam and video file input
- 📦 Lightweight and easy to use
- 🔁 Live visualization with bounding boxes
- ⛔ Exit detection easily with the ESC key

---

## 📁 Folder Structure

```
simple-face-detection-opencv/
├── facedetect.py    # Main detection script
└── README.md        # Project documentation
```

Other required files must be downloaded manually (see below).

---

## 📦 Requirements

Before running the script, make sure the following modules and files are available:

### 🐍 Python Modules

- Python 3.x
- NumPy
- OpenCV

Install with pip:

```bash
pip install numpy opencv-python
```

---

## 📥 Download Required Files

You need to download the following supporting files and place them in the **same directory** as `facedetect.py`.

### 1. 🔧 Library Files (for video and rendering utilities)

Download from:  
**📎 [Library Folder (libcommon, libvid, librender)](https://drive.google.com/drive/folders/1j8csJdaLu8-8jaSbV-WXxmil9OjuMKY7?usp=drive_link)**

**Files included:**
- `libcommon.py`
- `libvid.py`
- `librender.py`

### 2. 🧠 Haar Cascade XML Files (for face and eye detection)

Download from:  
**📎 [Haarcascade XML Folder](https://drive.google.com/drive/folders/13lDjzhoYb8BTlExsGRlY33tbFAsO0oBu?usp=drive_link)**

**Files required:**
- `haarcascade_frontalface_alt.xml`
- `haarcascade_eye.xml`

Make sure these files are in the **same folder** as `facedetect.py`.

---

## 🚀 How to Use

### ▶️ Run with webcam:

```bash
python facedetect.py
```

### 🎥 Run with a video file:

```bash
python facedetect.py path/to/video.mp4
```

### ⚙️ Use custom cascade files:

```bash
python facedetect.py --cascade="haarcascade_frontalface_alt.xml" --nested-cascade="haarcascade_eye.xml"
```

---

## 🔍 How It Works

1. **Load Haar Cascade XMLs** for face and eye detection.
2. **Capture frames** from webcam or video.
3. **Convert to grayscale** and enhance contrast.
4. **Detect faces**, then detect **eyes** inside each face region.
5. **Draw bounding boxes** for faces and eyes.
6. Display the result in a window that updates in real-time.
7. Press **ESC** to exit.

---

## 🧠 About `__pycache__` and `.pyc` Files

When you run the program, Python may automatically generate a `__pycache__/` folder containing `.pyc` files — compiled bytecode versions of your scripts.

These files improve performance but **are not necessary to upload to GitHub**.

### ✅ Recommended `.gitignore`

If you’re using Git, create a `.gitignore` file with:

```
__pycache__/
*.pyc
```

---

## 🤝 Contributing

Pull requests and suggestions are welcome. If you’d like to improve the detection logic, structure, or documentation, feel free to contribute!

---

## 📄 License

This project uses OpenCV's Haar Cascade classifiers, distributed under the Intel Open Source License.  
All custom Python code is released under the MIT License.

---

## 🙏 Acknowledgements

- [OpenCV](https://opencv.org) for the computer vision framework.
- Haar Cascade authors (e.g., Rainer Lienhart) for the detection models.
