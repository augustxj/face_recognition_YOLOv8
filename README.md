# Face Recognition with OpenCV and Face_Recognition

## Overview
This project showcases the use of the `face_recognition` library for efficient face detection and recognition in images. It processes a folder of images, identifying faces and matching them with known face encodings. While this task could be accomplished using only OpenCV, the primary objective was to explore and understand the `face_recognition` package due to its simplicity and powerful functionalities.

## Libraries Used
- **Face_Recognition**: used for face detection and recognition, it encodes facial features and matches them against a dataset of known faces. It utilizes `Dlib`, a machine learning library that powers the core face detection and recognition models using deep learning.
- **OpenCV** (`cv2`): used for processing images, converting color spaces, detecting facial features, drawing bounding boxes around detected faces, and resizing images for display.
- **NumPy**: used for efficient handling and manipulation of image arrays, enabling fast computations for facial encoding and distance calculations.
- **YOLOv8**: used to detect faces in the images.

## How It Works
1. **Load Images**: Reads images from a specified folder.
2. **Face Detection**: Uses `face_recognition.face_locations()` to detect faces in each image.
3. **Face Encoding**: Extracts facial features using `face_recognition.face_encodings()`.
4. **Face Recognition**: Compares detected faces with known encodings and assigns names if a match is found.
5. **Visualization**: Draws rectangles around faces and labels them.

## Usage
1. Enter the `face_recognition_YOLOv8.ipynb ` file in this repository and click "Run in Collab".
2. Go into Colab setting and choose TPU enviroment.
3. You can test with web images (through !wget) or utilize your own folder with reference images.
4. it's extremely important that your file names are your actual label names. Ex:  `Sherlock.jpeg `.
    - you can chage it easily inside Colab. Go into the folder and rignt click "rename".
6. follow the code flow: put the know images inside the  `labels` folder and in the and the images you want to recognize in the  `test` folder.

## Example Output
The script processes images and outputs recognized faces:
```plaintext
Recognized persons in image1.jpg: John, Alice
No recognized faces in image2.jpg.
```
Each processed image will be displayed with bounding boxes and names over the detected faces.

## Notes
- Ensure images are clear and contain visible faces for better recognition accuracy.
- The system may require fine-tuning depending on lighting conditions and image quality.


