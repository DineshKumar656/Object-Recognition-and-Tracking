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
