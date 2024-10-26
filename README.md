# Invisibility Cloak Project using OpenCV

This project creates a real-time "invisibility cloak" effect using OpenCV in Python. By isolating a specific color and replacing it with a background frame, the code simulates an optical illusion where the cloak appears invisible.

## Code Breakdown

### 1. Trackbar Creation
- Trackbars allow users to adjust HSV (Hue, Saturation, Value) parameters, setting the color range of the cloak to be detected.
- This range isolates the cloak color, creating a mask to filter it out.

### 2. Background Capture
- The code captures an initial frame to serve as the background, which will replace the cloak area when the effect is applied.

### 3. Color Masking and Filtering
- Each frame is converted to the HSV color space, and a mask is created based on the selected color of the cloak.
- The mask is further adjusted with median blur and dilation to smooth edges and enhance visibility.

### 4. Frame Processing for Invisibility
- Using bitwise operations, the area covered by the cloak is replaced with the initial background frame, creating the illusion of invisibility.

### 5. Final Output
- The processed frame, displaying the invisibility effect, is shown in a window named "Harry's Cloak."
- The program can be exited by pressing the 'q' key.

## How It Works

This code combines image processing and computer vision techniques to achieve an interactive invisibility illusion. Adjust the HSV sliders on the trackbars to match the cloak color for the desired effect.

**Requirements**: OpenCV, Numpy, and a working webcam.

## Run the Code

1. Install the required packages:
   ```bash
   pip install opencv-python numpy
2. Run the script:
   ```bash
   python cloak.py
3. Adjust the trackbars to set the color range for your cloak, and watch the invisibility effect in real-time!
