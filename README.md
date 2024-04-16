# Facial Emotion Recognition using OpenCV and Deepface

## Overview
This project uses the deepface library and OpenCV to implement real-time facial emotion detection. By using the webcam feed, it detects faces and provides predictions for the emotions associated with each face. The detected emotions are then displayed on the frames in real-time. This implementation offers a concise yet effective method for monitoring emotions in real-time using minimal code.
*****************************


## Dependencies
- deepface: A deep learning facial analysis library that provides pre-trained models for facial emotion detection. It relies on TensorFlow for the underlying deep learning operations.

- OpenCV: An open-source computer vision library used for image and video processing.
******************************



## Approach

1. Import the necessary libraries: cv2 for video capture and image processing, and deepface for the emotion detection model.

2. Load the Haar cascade classifier XML file for face detection using cv2.CascadeClassifier().

3. Start capturing video from the default webcam using cv2.VideoCapture().

4. Enter a continuous loop to process each frame of the captured video.

5. Convert each frame to grayscale using cv2.cvtColor().

6. Detect faces in the grayscale frame using face_cascade.detectMultiScale().

7. For each detected face, extract the face ROI (Region of Interest).

8. Preprocess the face image for emotion detection using the deepface library's built-in preprocessing function.

9. Make predictions for the emotions using the pre-trained emotion detection model provided by the deepface library.

10. Retrieve the index of the predicted emotion and map it to the corresponding emotion label.

11. Draw a rectangle around the detected face and label it with the predicted emotion using cv2.rectangle() and cv2.putText().

12. Display the resulting frame with the labeled emotion using cv2.imshow().
******************************
## Installation
- Git clone this repository Run: git clone https://github.com/ArchitArora03/face-emotion-recognition
- Run: cd Facial Emotion Recognition using OpenCV and Deepface
* Install the required dependencies:

    * pip install deepface
    * pip install tf_keras
    * pip install opencv-python
- Download the Haar cascade XML file for face detection: Visit the OpenCV GitHub repository and download the haarcascade_frontalface_default.xml file.
- Run the code: The webcam will open, and real-time facial emotion detection will start. Emotion labels will be displayed on the frames around detected faces. 
******************************
## Contributing
Contributions to this project are welcome. If you find any bugs or have suggestions for improvement, please open an issue or submit a pull request.
## License

[MIT](https://choosealicense.com/licenses/mit/)

