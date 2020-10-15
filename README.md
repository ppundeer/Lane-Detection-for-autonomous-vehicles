# Lane-Detection-for-autonomous-vehicles

The lines on the road that show us where the lanes are act as our constant reference for where to steer the vehicle. Naturally, one of the first things we would like to do in developing a self-driving car is to automatically detect lane lines using an algorithm.

In this project we detect lane lines in images using Python and OpenCV2. OpenCV means "Open-Source Computer Vision", which is a package that has many useful tools for analyzing images.

The tools we have are color selection, region of interest selection, grayscaling, Gaussian smoothing, Canny Edge Detection and Hough Tranform line detection. Our goal is piece together a pipeline to detect the line segments in the image, then average/extrapolate them and draw them onto the image for display. 

Shortcomings
1. Hough Transform is fit for Straight Lines only but in reality curved lane lines exists where this may fail.
2. There are many roads which don't have lane markings where this will fail.
