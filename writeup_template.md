# **Finding Lane Lines on the Road** 

## 1.General Information


##Goal
The goals / steps of this project are the following:
* Detect Lane Lines on the road.
* Draw Lines on the image to represent the aerea where the car is supposed to operate.


##Methods
Operating only under Conputer Vision techniques.

##Ressources
General : Python 3, Anaconda
Specific : OpenCV, Panda, Nympy, Matplotlib, Math

##Steps
Color Selection 
Region Masking
Canny Edge Detection
Hough Transform 


[//]: # (Image References)

[image1]: ./examples/grayscale.jpg "Grayscale"

---



### 2.pipeline.
*Applying a gray scale to the input image 

*Applying a gaussian blur to the gray image

*Applying the Canny Edge detection to the blur image

*Applying a polygone to mask a region of interest where Lanes are potentially located from the camera

*Applying the Hough transform to the result image with an approximation of the detected line to
extrapolate pixels into lines

![alt text][image1]

### 3. Improvements 

We could use a color filter to detect lanes from their color for exemple applying a yellow and white detection because they are widelyspred used and/or using HSL color space.

Also a linear regression and extrapolation to find the lines and/or separate the region of interst by a left and a right ones. 
