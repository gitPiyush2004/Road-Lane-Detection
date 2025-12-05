# 🛣️ Road Lane Detection using OpenCV

This project uses computer vision methods in OpenCV to identify road lane markings from dashcam footage. It demonstrates the core idea behind a simple lane-following mechanism, a fundamental building block in autonomous driving systems.

# Developed by: Piyush Bhatia, VIT Bhopal University

---

## 🎥 Input vs Output Video

### 🔹 Original Input Video  
<video src="https://github.com/user-attachments/assets/0b14c4a3-f1c7-417f-bb34-58b8f2309ed5" width="400" controls></video>

### 🔸 Output Video with Lane Detection  
<video src="https://github.com/user-attachments/assets/a0d5acb2-529b-40c5-9548-52e2c5852ec6" width="400" controls></video>

## 📹 Input Video

- **File:** `solidWhiteRight.mp4`  
- **Source:** [Udacity Self-Driving Car Dataset](https://github.com/udacity/CarND-LaneLines-P1)
- Clean white-lane driving footage recorded in daylight

---

## 🔴 Live Demo
👉 Try the model on Streamlit: [Road Lane Detection App](https://road-lane-detection-opencv-qfwagy6zxuj8zkuaspkwu4.streamlit.app/)

---

## How the System Works
1. The input video frame is first converted into grayscale to simplify processing.
2. A Gaussian blur is applied to smooth the image and reduce noise.
3. Canny edge detection is used to highlight the prominent edges in the frame.
4. A region of interest (ROI) is defined so that only the relevant road area is processed.
5. The Hough Line Transform is then used to identify straight line segments.
6. Detected lines are grouped, averaged, and extended to form complete left and right lane boundaries.
7. Finally, the calculated lanes are drawn back onto the original frame to visualize the detection.

---

## 🧠 Technologies Used

- Python 3
- OpenCV
- NumPy

---

## 📦 Requirements

```bash
opencv-python
numpy
```

> Install them using:  
> `pip install -r requirements.txt`

---

## 📁 Project Structure

| File                          | Description                                           |
|-------------------------------|-------------------------------------------------------|
| `lane_detection.py`           | Main script that processes the video                 |
| `solidWhiteRight.mp4`         | Input driving video                                  |
| `lane_detected_output.mp4`    | Output video with detected lanes                     |
| `requirements.txt`            | Python libraries used                                |
| `README.md`                   | Project documentation                                |

---

## 🚀 How to Run

```bash
pip install -r requirements.txt
python lane_detection.py
```

---



---



