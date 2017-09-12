# **Finding Lane Lines on the Road** 

## Writeup 

---

**Finding Lane Lines on the Road**


[image1]: ./test_images/solidWhiteCurve.jpg "solidWhiteCurve"

[image2]: ./test_images_output/solidWhiteCurve.jpg "processedSolidWhiteCurve"
---

### Reflection

### 1. Pipeline


explain how you modified the draw_lines() function.

My pipeline consisted of 5 steps. First, I converted the images to grayscale, then I .... 

In order to draw a single line on the left and right lanes, I modified the draw_lines() function by ...

If you'd like to include images to show how the pipeline works, here is how to include an image: 

![alt text][image1]


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
