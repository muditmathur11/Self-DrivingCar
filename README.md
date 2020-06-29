# Self-DrivingCar

In this repository I will update with several projects for the Self-Driving Car NanoDegree Program from Udacity. The first featured project is the Traffic Light Classifier. Read below for more information about this project:

# Traffic Light Classifier
In this project, I used my knowledge of computer vision techniques to build a classifier for images of traffic lights! I was provided a dataset of traffic light images in which one of three lights is illuminated: red, yellow, or green.

## Classification Steps

With the provided notebook, I was responsible to pre-process the given images, extract features that will help distinguish the different types of images, and use those features to classify the traffic light images into three categories: red, yellow, or green. The tasks were broken down into a few sections:

1. Loading and visualizing the data. The first step in any classification task is to be familiar with your data; I loaded in the images of traffic lights and visualized them.

2. Pre-processing. The input images and output labels need to be standardized; I ensured the input was of the same type of data and of the same size, and the output was a numerical label. This way, I could analyze all the input images using the same procedures, and I know what output to expect when you eventually classify a new image.

3. Feature extraction. Next, I extracted some features from each image that distinguished and classified these images. The features that I made help distinguish between the 3 classes of traffic light images because they separate the image into 3 "slices" from top to bottom, and measure the intensity of value in HSV colorspace. It does this by averaging the brightness value in each slice and comparing the brighter value.

4. Classification and visualizing error. Finally, I wrote a function to use my features to classify any traffic light image. This function takes in an image and output a label. I was then able to classify a test set of data, compare my predicted label with the true label, and determine the accuracy of my classification model.

5. Evaluate your model. My model resulted in ~97% accuracy and never classified any red lights as green!
