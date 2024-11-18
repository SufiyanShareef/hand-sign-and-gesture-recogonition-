Hand Sign and Gesture Recognition

This repository implements a  Hand Sign and Gesture Recognition System  using  MediaPipe ,  OpenCV , and  TensorFlow . It supports the recognition of American Sign Language (ASL) alphabets (A–Z), numbers (0–9), and a few common gestures such as  thumbs up ,  thumbs down ,  peace ,  stop , and  hi .

  🚀 Features
-  Real-Time Recognition : Recognizes hand gestures in real-time using a webcam.
-  ASL Support : Detects alphabets (A-Z) and numbers (0–9).
-  Custom Gestures : Detects custom gestures like thumbs up, thumbs down, peace, stop, etc.
-  Easy Data Collection : Includes a script to capture hand gesture data for training.
-  Model Training : A TensorFlow-based deep learning model for gesture classification.
-  Expandable Dataset : Easily add new gestures or signs to the system.

 

  📂 Project Structure

hand-sign-and-gesture-recognition/
├── Image/                         Dataset folder containing collected landmarks
│   ├── A/
│   │   └── landmarks.npy
│   └── ...                       Other folders for alphabets, numbers, and gestures
├── collect_data.py               Script to collect gesture data and save as landmarks
├── preprocess_data.py            Script to preprocess the data for training
├── train_model.py                Script to train the gesture recognition model
├── run_recognition.py            Script for real-time hand gesture recognition
├── requirements.txt              Required dependencies for the project
└── README.md                     Project documentation
 

 

  🛠️ Installation

1.  Clone the repository :
    bash
   git clone https://github.com/SufiyanShareef/hand-sign-and-gesture-recognition.git
   cd hand-sign-and-gesture-recognition
    

2.  Install dependencies :
   Ensure you have Python 3.7–3.10 installed, then run:
    bash
   pip install -r requirements.txt
    

3.  Verify MediaPipe Installation :
   MediaPipe requires a compatible version of Python (3.7–3.10). If you have Python 3.13 or higher, install Python 3.10 and create a virtual environment for the project.

 

  🖐️ How to Use

   1.  Data Collection 
   Run `collect_data.py` to collect gesture data:
    bash
   python collect_data.py
    
   - Use the webcam to record gestures for alphabets, numbers, or custom gestures.
   - The collected landmarks are saved under the `data/` folder.

   2.  Preprocess the Data 
   Prepare the dataset for training:
    bash
   python preprocess_data.py
    

   3.  Train the Model 
   Train the gesture recognition model using TensorFlow:
    bash
   python train_model.py
    

   4.  Run Real-Time Recognition 
   Test the trained model in real-time:
    bash
   python run_recognition.py
    

 

  👨‍💻 Development

   Adding New Gestures
1.  Data Collection :
   - Record the new gesture using `collect_data.py`.
   - Save the gesture data under the `data/` folder with a unique name.

2.  Retrain the Model :
   - Run `train_model.py` to include the new gestures.

3.  Test the Gesture :
   - Verify the new gesture using `run_recognition.py`.

 

  🤖 Technologies Used
-  MediaPipe : For hand landmark detection.
-  OpenCV : For webcam input and real-time video processing.
-  TensorFlow : For building and training the gesture recognition model.
-  NumPy : For data preprocessing and manipulation.

 


 
Sufiyan Shareef 
Email mdsufiyanshareef@gmail.com
For questions or contributions, feel free to [open an issue](https://github.com/SufiyanShareef/hand-sign-and-gesture-recognition/issues) 

 

