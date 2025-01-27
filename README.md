# Realtime-Facial-Expression-Recognition  ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/spleeter) 

>  :warning:   Please go through the ```requirements.txt``` file before running the models and install all packages.
>  ```powershell
>  pip install -r requirements.txt --upgrade
>  ```

I have selected this project as one of my final year project. This is a realtime facial expression recognition model which uses FER 2013 dataset. I have used Keras, OpenCV and Flask. 

In this project, we will build and train a convolutional neural network (CNN) in Keras from scratch to recognize facial expressions. The data consists of 48x48 pixel grayscale images of faces. The objective is to classify each face based on the emotion shown in the facial expression into one of seven categories (0=Angry, 1=Disgust, 2=Fear, 3=Happy, 4=Sad, 5=Surprise, 6=Neutral). We will use OpenCV to automatically detect faces in images and draw bounding boxes around them. Once we have trained, saved, and exported the CNN, we will directly serve the trained model to a web interface and perform real-time facial expression recognition on video and image data.

The project can be braodly divided into two parts -
1) Build and train a model in Keras for Facial Expression Recognition.
2) Deploy the model on web using FLASK and run it on videos.

# Steps to follow

1) Extract train and test images from ```data.rar``` file.
2) Install dependencies using

   ```powershell
   pip install pipenv
   ```

   ```powershell
   pipenv install
   ```

3) Run the jupyter notebook for training, ```model.json``` and ```model_weights.h5``` files will be created after training.
4) Add the correct path to the video file in camera.py on line 11.
5) Now run  

   ```powershell
   pipenv run python3 main.py
   ```
