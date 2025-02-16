# Face Recognition with OpenCV and Face_Recognition

## Overview
This project demonstrates how to use OpenCV and the `face_recognition` library for detecting and recognizing faces in images. It iterates through a folder containing images, detects faces, and matches them with known face encodings.

## Technologies Used
- **Python**: Main programming language.
- **OpenCV** (`cv2`): Used for image processing and visualization.
- **Face_Recognition**: A Python library based on `dlib` for detecting and recognizing faces.
- **NumPy**: Used for handling numerical operations.

## Requirements
Before running the project, install the required dependencies:
```bash
pip install opencv-python face-recognition numpy
```

## How It Works
1. **Load Images**: Reads images from a specified folder.
2. **Face Detection**: Uses `face_recognition.face_locations()` to detect faces in each image.
3. **Face Encoding**: Extracts facial features using `face_recognition.face_encodings()`.
4. **Face Recognition**: Compares detected faces with known encodings and assigns names if a match is found.
5. **Visualization**: Draws rectangles around faces and labels them.

## Usage
1. **Prepare a folder with reference images** (e.g., known persons with filenames as their names).
2. **Run the script**:
```python
recognize_faces("path/to/your/images")
```

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

## License
This project is open-source and available under the MIT License.

