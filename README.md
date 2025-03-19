# Face Recognition with OpenCV

A basic Python script utilizing OpenCV to recognize faces in real-time using a webcam.

## Features

- **Face Detection**: Utilizes OpenCV's Haar Cascade Classifier to detect faces in real-time.
- **Face Recognition**: Employs the Local Binary Patterns Histograms (LBPH) face recognizer for identifying detected faces.

## Requirements

- Python 3.x
- OpenCV
- NumPy

## Installation

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/ssrinivash/Face_recognition_opencv.git
   ```


2. **Navigate to the Directory**:

   ```bash
   cd Face_recognition_opencv
   ```


3. **Install Dependencies**:

   ```bash
   pip install opencv-python-headless numpy
   ```


## Usage

1. **Prepare Training Data**:

   - Collect face images of individuals you want to recognize.
   - Organize the images into subdirectories within a main directory (e.g., `dataset/`), where each subdirectory is named after the individual.

2. **Train the Recognizer**:

   - Use the `train_model.py` script to train the LBPH face recognizer on your dataset.

     ```bash
     python train_model.py --dataset dataset/ --model model.yml
     ```

3. **Run the Face Recognition Script**:

   - Execute the main script to start real-time face recognition using your webcam.

     ```bash
     python open_cv_face_reg.py --model model.yml
     ```

## Acknowledgements

- This project is inspired by various OpenCV face recognition tutorials and implementations.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details. 
