Motion Detection using OpenCV

This project implements a basic motion detection system using Python, OpenCV, and Imutils. The program captures video from a webcam, detects motion by comparing frames with a background reference, and highlights moving objects with bounding boxes in real-time.

🚀 Features

Real-time motion detection using webcam

Background subtraction with frame differencing

Noise reduction using Gaussian blur and morphological operations

Bounding box around detected moving objects

Status display: "Normal" or "Moving Object detected"

Press q to exit gracefully

📂 Project Structure
motion-detection/
│-- motion_detection.py   # Main script
│-- README.md             # Project documentation

🛠️ Requirements

Make sure you have the following installed:

Python 3.x

OpenCV (cv2)

Imutils

Install dependencies with:

pip install opencv-python imutils

▶️ Usage

Clone this repository:

git clone https://github.com/your-username/motion-detection.git
cd motion-detection


Run the script:

python motion_detection.py


A window will open showing the live camera feed:

Green rectangles highlight moving objects

Text "Moving Object detected" appears when motion is found

Press q to quit

📸 Example Output

Normal State
No movement detected → Status: "Normal"

Motion Detected
Moving object highlighted → Status: "Moving Object detected"

⚡ How It Works

Capture video frames from webcam

Convert frames to grayscale and apply Gaussian blur

Store the first frame as background reference

Compute absolute difference between current frame and background

Apply thresholding and dilation to detect motion regions

Draw bounding boxes around moving objects

demo
<img width="1737" height="1079" alt="Screenshot 2025-09-10 054908" src="https://github.com/user-attachments/assets/13f8cb03-af78-48a8-b649-beb5396b3592" />

<img width="1893" height="1079" alt="Screenshot 2025-09-10 054924" src="https://github.com/user-attachments/assets/1a41a2ac-f771-4efa-b852-2801cd9047de" />
<img width="1916" height="1079" alt="Screenshot 2025-09-10 054839" src="https://github.com/user-attachments/assets/8ddcf970-f9a6-41d1-9a71-1e8ec8cbc53c" />



