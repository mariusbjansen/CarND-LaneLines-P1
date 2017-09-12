# **Finding Lane Lines on the Road** 
---

### Reflection
In this project the goal was to create a pipieline extracting lane lines from images and drawing them.
Later a video sequence was used to further improve the processing chain.

### 1. Pipeline

My pipeline constists of 8 steps

## STEP 1 Grayscale conversion
## STEP 2 Color selection (threshold filter)
## STEP 3 Defining region of interest (ROI)
## STEP 4 Applying a gaussian blur
## STEP 5 Detect edges with Canny edge detector
## STEP 6 Detect lines by Hough transformation
## STEP 7 Overlay the original image with the detected lines
## STEP 8 Save the result

My pipeline consisted of 5 steps. First, I converted the images to grayscale, then I .... 

In order to draw a single line on the left and right lanes, I modified the draw_lines() function by ...

If you'd like to include images to show how the pipeline works, here is how to include an image: 

explain how you modified the draw_lines() function.

<img src="test_images/solidWhiteCurve.jpg" width="300">


### 2. Shortcoming 

Number of lines maximum 2
Curvature
Linear representation
clothoid
polynomia
One potential shortcoming would be what would happen when ... 

Need to keep in mind that this is not suited for controlling since we are in the image COS and not world COS

Another shortcoming could be ...


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to ...

Another potential improvement could be to ...

polyfit polynomial
use clothoids
