# Banking-Atm-Facial-Recognition-Software
This repository contains a banking ATM facial recognition software developed using Tkinter for the GUI and OpenCV for the facial recognition functionality. The software is designed to enhance security by using facial recognition as part of the authentication process at ATMs.

Overview
This project leverages deep learning and machine learning models to extract facial embeddings and perform real-time facial recognition. The software integrates these functionalities into a banking application interface created using Tkinter.

Features
Facial Embedding Extraction: Extracts facial embeddings from a dataset using a pre-trained deep learning model.
Model Training: Trains an SVM classifier for facial recognition using the extracted embeddings.
Real-Time Face Recognition: Performs facial recognition using a live video stream from the webcam.
Tkinter GUI: A user-friendly graphical interface for interaction with the banking system.
Project Structure
extract_embeddings(self): Extracts facial embeddings from a dataset and saves them to disk.
train_model(self): Trains an SVM classifier on the extracted embeddings and saves the model to disk.
video_check(self): Performs real-time face recognition using the webcam and verifies the recognized user against known users.
Tkinter GUI Initialization: Sets up the GUI interface for the banking application.
Setup
Prerequisites
Ensure you have the following installed:

Python 3.7+
OpenCV
Tkinter
scikit-learn
Other dependencies listed in requirements.txt
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/Godfathxx/Banking-Atm-Facial-Recognition-Software.git
cd banking-atm-facial-recognition
Install dependencies:

bash
Copy code
pip install -r requirements.txt
Prepare the Dataset:

Place your dataset of images in the appropriate directory as specified in your script for facial embedding extraction.

Running the Software
1. Extract Facial Embeddings:
go
Copy code
```bash
python software.py
```
This command extracts facial embeddings from the dataset and saves them for later use.

2. Train the Face Recognition Model:
go
Copy code
```bash
python software.py
```
This command trains an SVM classifier on the extracted facial embeddings and saves the trained model.

3. Run Real-Time Face Recognition:
go
Copy code
```bash
python software.py
```
This command starts the Tkinter GUI and performs real-time face recognition using the webcam.

4. Start the Banking Application:
go
Copy code
```bash
python software.py
```
This command initializes the Tkinter GUI for the banking application, allowing users to authenticate using facial recognition.

Usage
User Authentication: The software captures facial images, checks for a match against known users, and if successful, proceeds to password verification.
Retry and Lockout Mechanism: If the user is not recognized or confidence is below the threshold, the system allows a limited number of retries before locking the user out.
Results
The facial recognition process is displayed in the GUI window, showing the user's face, bounding boxes, and recognized names. Alerts are triggered for unknown users or failed matches.

Contributing
Contributions are welcome! Please feel free to submit issues or pull requests.

License
This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgments
OpenCV
Tkinter
scikit-learn
