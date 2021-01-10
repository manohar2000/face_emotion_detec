# Facial Emotion Recognition
Deployment mode : Via Flask backend [ runs on the localhost]

Task : Develop convolutional neural network (CNN) in Keras from scratch to recognize facial expressions.

# Steps to run the model:
To install the dependencies create a new environment, and  run the following command
"cd webapp"
“pip install -r requirements.txt”

For the backend part we have used Flask, for model inference in real-time, we have made of use Tensorflow backend. In case of the GPU support available in you system, you could fasten up the inference time.

The Working of the project could be done by running the “main.py” file with the command 
“python main.py” 

This will create a local server using Flask and once the server gets active, you can visit 
“localhost:5000/” and you can see the responsive site active. 


Upon clicking the “Start Live Demo” button, we would be redirected to a page wherein the rendered frames
1)	with the bounding box [ detecting the face ] and
2)	Text showing the emotion of the frame after getting classified with the help of our model.


# Steps for making the prediction:
1)	 Visit the web application
2)	Click on the Start Live Demo button.
3)	Live video capture starts.
4)	The frames are captured.
5)	The haarcascade filters helps in drawing a bounding box across the detected human face.
6)	The bounding box region is cropped : creating a ROI containing just the face.
7)	This cropped face frame is sent to the Machine Learning Model for prediction.
8)	The model classifies the frame into one of the 7 categories : 
9) The predicted output label is shown on the screen.
