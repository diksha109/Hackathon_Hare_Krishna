# **Gesture2Health: Breaking the Communication Barrier between Hearing-Impaired Patients and Healthcare Professionals in India**

Gesture2Health is an innovative project that aims to bridge the communication gap between hearing-impaired patients and healthcare professionals in India.  There are an estimated 18 million hearing-impaired individuals in India. Many healthcare professionals are not trained in ISL or other sign languages. The system uses a camera to capture the patient's gestures, which are then processed and analyzed by the model. The model then generates written text output, which can be used by healthcare professionals to communicate with the patient. 

Gesture2Health is not just a technological solution, but also a social one. The project is designed to promote greater awareness and understanding of the needs of hearing-impaired patients in healthcare settings and to promote more inclusive and equitable healthcare services.
    
## Table of Contents
* [Objective](#objective)
* [Methodology](#methodology)
* [Technologies And Tools](#technologies-and-tools)
* [Running the Project](#running-the-project)
* [Demo Video](#demo-video)
* [References](#references)

## Objective: 
The objective of the Gesture2Health project is to develop a state-of-the-art sign language recognition model that can accurately recognize Indian sign language (ISL) gestures and translate them into written text in real-time. This project aims to bridge the communication gap between hearing-impaired patients and healthcare professionals in India, thereby providing a more inclusive and effective healthcare experience for hearing-impaired patients by removing communication barriers. Through the use of advanced technology and a focus on promoting greater awareness and understanding of the needs of hearing-impaired patients in healthcare settings, Gesture2Health aims to create a more just and equitable healthcare system for all.

## Methodology
- Our dataset consisted of `8` classes(Indian Sign Language Gestures) of `Healthcare Domain`.
- The classes are `Afternoon`, `Allergy`, `Blood`, `Doctor`, `Help`, `Sick`, `Today`, `Winter`.
- Each class has `15` videos for training.
- First, we extract the frames from  all the videos, and using `MediaPipe`, we extract the keypoints for all the frames and store it in a csv file.
- Next, we preprocess these keypoints and divide the csv file into train and test sets.
- Next, we train the `BiLSTM Model` which has `3 Bidirectional LSTM layers` and `2 dense layers`.
- After training and saving the model, we have used it for deploying our application. 

## Technologies And Tools
The following technologies and tools were used for the implemetation of our project:
- Python
- Mediapipe
- OpenCV
- TensorFlow
- Keras
- NumPy
- Flask
- HTML5

## Running the project: 
- Download the repository and create a Virtual Environment using python.
- Activate the Virtual Environment.
- Install the required dependencies mentioned below:
    ```python
     pip install -r requirements.txt
    ```
 - Run the `main.py` file.
 - Open your browser and navigate to `http://127.0.0.1:5000`. 
 - Here you will find the app.

## Demo Video
Here is the demo video of our project:

https://user-images.githubusercontent.com/90503933/232321349-fe5abdb9-e94f-4913-859e-d11afe4c0ce8.mp4


## References
We have referred the following research paper for dataset and code:
```
@INPROCEEDINGS{9456116,
  author={Gandhi, Jash and Gandhi, Parth and Gosar, Aayush and Chaudhari, Sheetal},
  booktitle={2021 2nd International Conference for Emerging Technology (INCET)}, 
  title={Video Recognition Techniques for Indian Sign Language in Healthcare Domain}, 
  year={2021},
  volume={},
  number={},
  pages={1-5},
  doi={10.1109/INCET51464.2021.9456116}}
```
