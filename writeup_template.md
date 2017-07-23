# **Finding Lane Lines on the Road** 

## Writeup Template

### You can use this file as a template for your writeup if you want to submit it as a markdown file. But feel free to use some other method and submit a pdf if you prefer.

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


### 1. Reflection

My pipeline consists of the following steps.
Steps:
* Converting image to a grayscale image.
* Applying Gaussian smoothing on the grayscale image.
* Applying canny edge detection on gaussian blur image.
* Image masking on canny image using the helper function region of interest.
* Apply hough transform to detect the lines on image.
* Overlaying the lines on original image.

  * I have modified the draw_lines() helper function to draw a single line on the left and right lanes. 


### 2. Identify potential shortcomings with your current pipeline
* The current pipe line will work only for first two videos and for the optional challgene getting  float NaN to integer error.
* To save the images and videos, need to create two folders in side project test_images_output and test_videos_output.
* For image mask is used static values to the helper funtion region of interest.

### 3. Suggest possible improvements to your pipeline
* First improvment is to fix the current pipe line to work for 3rd video.
* The quality of lane detection using draw_line function needs to improved based on the different input videos.
