# Autonomous Drone Vision System (Simple Version)

This is a beginner-friendly computer vision project that simulates an autonomous drone using only a laptop webcam. It uses OpenCV to detect human faces in real-time and prints simple behavior (e.g., hovering, moving toward a face) to simulate drone logic.

> ⚠️ No real drone is needed — this version uses your webcam and prints simulated commands.

---

## 🎯 Features

- Real-time face detection using OpenCV
- Simulated drone behavior in terminal
- Live webcam feed with bounding boxes on detected faces
- Lightweight and easy to run

---

## 📁 Project Structure

```
autonomous-drone-vision/
├── main.py                          # Main program for face detection
├── requirements.txt                # Python dependencies
└── haarcascade_frontalface_default.xml  # OpenCV face detection model
```

---

## 🔧 Requirements

- Python 3.6+
- OpenCV

Install required packages with:

```bash
pip install -r requirements.txt
```

---

## 🚀 How to Run

1. **Download or clone** the repository.
2. Make sure the file `haarcascade_frontalface_default.xml` is in the same folder as `main.py`.

   👉 [Download it from OpenCV GitHub](https://raw.githubusercontent.com/opencv/opencv/master/data/haarcascades/haarcascade_frontalface_default.xml)

3. Run the program:

```bash
python main.py
```

4. The webcam feed will open. Press **`q`** to quit.

---

## 🧠 How It Works

- The script uses OpenCV’s pre-trained Haar Cascade model to detect faces.
- If one or more faces are detected, the program simulates a drone moving toward the face.
- If no face is found, the simulated drone "hovers".

Example output in terminal:

```
1 face(s) detected. Drone moving toward face.
No face detected. Drone is hovering.
```

---

## 📸 Screenshot

> _(You can add a screenshot of your webcam feed with a detected face here)_

---

## 📌 Future Improvements

- Add color tracking (e.g., follow a red object)
- Use actual drone SDK (e.g., DJI Tello via `djitellopy`)
- Implement obstacle avoidance
- Add gesture recognition

---

## 📜 License

This project is free to use for educational and non-commercial purposes.
