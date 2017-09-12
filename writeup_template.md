# **Finding Lane Lines on the Road** 

## Reflection
In this project the goal was to create a pipieline extracting lane lines from images and drawing them.
Later a video sequence was used to further improve the processing chain.

Example image
<img src="test_images/solidWhiteCurve.jpg" width="300">

Example result
<img src="test_images_output/solidWhiteCurve.jpg" width="300">
The red lines are an analytical expression (y=mx+b) of the detected lines

### 1. Pipeline

My pipeline constists of 8 steps

#### 1 Grayscale conversion
#### 2 Color selection (threshold filter)
#### 3 Defining region of interest (ROI)
#### 4 Applying a gaussian blur
#### 5 Detect edges with Canny edge detector
#### 6 Detect lines by Hough transformation
#### 7 Overlay the original image with the detected lines
#### 8 Save the result



### 2. Shortcoming 

#### A The maximum number of lines in my algorithm is two. I am only looking for one positive and one negative gradient - for the sake of simplicity.

#### B The lines are not stable. They are flickering.

#### C If the curvature is high, the line representation y = m*x+b representation is not well suited

#### D All this processing is in the image coordinate system and not in the world coordinate system. It's not suited for any controlling for example.


### 3. Suggest possible improvements to your pipeline

#### A For more complex scenarios I suggest a clustering algorithm (commented in my code)

#### B Apply a filter (PT1 for the sake of simplicity). Maybe Kalman filter

#### C I recommend using a different representation like polynomial of order of 2 upwards or even clothoids

#### D Transform to world coordinate system

