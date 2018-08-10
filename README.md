# **Finding Lane Lines on the Road** 
**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on work in a written report

[//]: # (Image References)

[image1]: ./examples/grayscale.jpg "Grayscale"

---

### Reflection

### 1. Procedure to find lane lines   

My pipeline consisted of 5 steps. First, I converted the images to grayscale, then I set up kernel size as 7 for Gaussian blur method; then set up low and high threshold for Caany edge detection. A masked edges are created with polygon-shape  

In order to draw a single line on the left and right lanes, I modified the draw_lines() function by modifying the input parameters such as threshold=15, min_line_length=100, and max_line_gap = 100

### 2. Identify potential shortcomings with your current pipeline

One potential shortcoming would be that  my drawed lines are not clear and clean as example video shown.

To draw a line on single image could be easy, but with video clip, every time step the road condition changes, the original setup may not be suitable for all road cases.


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to automatically setup parameters for different road condition to draw a line more precisely.

