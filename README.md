# **Finding Lane Lines on the Road**

<img src="test_image.jpg" width="480" alt="Combined Image" />


Overview

---



When we drive, we use our eyes to decide where to go.  The lines on the road that show us where the lanes are act as our constant 
reference for where to steer the vehicle.  Naturally, one of the first things we would like to do in developing a self-driving car
is to automatically detect lane lines using an algorithm.



In this project I will detect lane lines in images using Python and OpenCV.


### 1. pipeline


My pipeline consisted of 6 steps:

* Convert image to grayscale.
* Apply Canny edge detection to obtain edges.

* Set vertices of the region of interest and apply a selection mask to select the region of lane lines.
* Applying Hough transform to the masked image to get a lines image.
* Combine lines image with original image.