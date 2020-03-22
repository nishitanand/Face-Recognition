# Face Recognition

This program is used for face recognition.

I have used Numpy, Pandas and OpenCV libraries.
KNN is used.
In this project there are two python files, one to collect face data and the other to recognize faces.

In face_collect.py, I have used OpenCV to get video input from Front Camera. First person's name is taken input and then I used Haarcascade Face Classifier to identify faces. The python program then saves the face region continuously till we hit "q" on the keyboard and saves it as a .npy file with the person's name in the "data" Folder

Then Face_Recognition.py loads all the .npy files from the "data" Folder and once again using front camera a face is detected and then KNN is used to predict that this detected face is whose from the list of names of all .npy files and the predicted name is displayed on the frame of the detected face.

To use it, first write this command in the command line

pip install -r requirements.txt

or (for Mac)

pip3 install -r requirements.txt


and then to feed your face data, to run the file write

python face_collect.py

or (for Mac)

python3 face_collect.py


and then for face recognition, to run the file write

python Face_Recognition.py

or (for Mac)

python3 Face_Recognition.py
