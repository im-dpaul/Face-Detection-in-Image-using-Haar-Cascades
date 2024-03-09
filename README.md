# Project: Face and Eye Detection using Haar Cascade Classifier

## Introduction:

This project demonstrates the use of Haar Cascade classifiers for real-time face and eye detection in images. It leverages OpenCV, a powerful library for image processing and computer vision tasks.

## Key Concepts:
- Haar Cascade Classifiers: A type of machine learning algorithm used for object detection. It employs a cascade of simple features to efficiently detect objects like faces and eyes.
- OpenCV (Open Source Computer Vision Library):  A comprehensive library with a wide range of functions for real-time computer vision.

## Import Necessary Libraries:
   - `numpy`: For numerical computations and array operations.
   - `cv2`: For image processing and computer vision tasks.
   - `cv2_imshow` (from Google Colab): To display images within a notebook environment.

## Load Haar Cascade Classifiers:
   - Load the pre-trained Haar cascade XML files for face and eye detection.

## Read an Image:
   - Load an image ("group_img.jpg" in this example) using `cv2.imread()`.

## Convert to Grayscale:
   - Convert the image to grayscale using `cv2.cvtColor()`.

## Detect Faces:
   - Apply the face cascade classifier to detect faces in the grayscale image.
   - Iterate through the detected faces:
     - Draw rectangles around each face using `cv2.rectangle()`.
     - Extract the region of interest (ROI) for each face for eye detection.

## Detect Eyes:
   - Apply the eye cascade classifier to detect eyes within each face ROI.
   - Iterate through the detected eyes:
      - Draw rectangles around each eye using `cv2.rectangle()`.

## Display the Image:
   - Show the final image with detected faces and eyes using `cv2_imshow()`.

## Running the Project:
1. Install required libraries: `numpy` and `opencv-python`.
2. Ensure you have the Haar cascade XML files (download from [https://github.com/opencv/opencv/tree/master/data/haarcascades](https://github.com/opencv/opencv/tree/master/data/haarcascades)) in the same directory as your script.
3. Run the Python script to detect faces and eyes in the specified image.

