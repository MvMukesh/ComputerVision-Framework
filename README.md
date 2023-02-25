# ComputerVision-Framework

OpenCV projects, step towards Computer Vision and Deep Learning <br>
This repository includes any projects that I have completed in research, projects. <br>
`Main focus is to study fields that cross over Machine Learning(SVM, K-means), Deep Learning(CNN), Computer Vision and Data Science`

<p align="center">
  <kbd><img src="https://user-images.githubusercontent.com/26667491/221328025-1e8c4bfc-2534-4742-a7f5-0b0e9d0e29f7.png"/></kbd>  
  <!--<kbd><img src="https://user-images.githubusercontent.com/26667491/221328101-153a4910-3cae-4524-be10-3001c0ce6ea0.png"/></kbd>-->
  
  ## Deep Learning Timeline
  <kbd><img src="https://user-images.githubusercontent.com/26667491/221328067-954ea17f-8ba3-49d1-9766-126056fc287f.png"/></kbd>
</p>

<p align="right">
  <img src="https://user-images.githubusercontent.com/26667491/221327988-f36a7b53-3609-4347-9708-50d0241c05c9.gif" width=30% height=0%/>
</p>

## Index:
1. [Basics of Computer Vision and OpenCV](#)
2. [Image Manipulation and Processing](#)
3. [Image Segmentation and Contours](#)
4. [Object Detection Part 1: Intro](#)
5. [Object Detection Part 2: Build a Face, people and Car Detectors](#)
6. [Augmented Reality (AR): Facial Landmark Identification](#)
7. [Simple Machine Learning using OpenCV](#)
8. [Object Tracking and Motion Analysis](#)
9. [Computational Photography](#)
10. [Self Driving Cars](#)
11. [Deep Learning](#)
  
## Section:
#### Computer Vision & OpenCV - Basics
Image processing ==> blurring image, understanding image morphology, geometric transforms, image histograms

|             |          |           |
|-------------|----------|-----------|
|OpenCV Basic | | displaying image <br> plt.imshow(cv2.cvtColor(input, cv2.COLOR_BGR2RGB))|
|Grayscaling | |very popular technique in computer vision used to find <br>`gradient on edge points of an image` |
|Colors HSV-Hue | |in HSV it is more easier to represent a color than in BGR color-space <br> first convert BGR image to HSV `HSV is used to extract a colored object`|
|Colors Gray-RGB | |OpenCV allow to convert an RGB image into Grayscale in two ways <br> 1. using cvtColor function <br> 2. using imread function |
|Color Red-Green-Blue | |machine can only understand three colors: red, green, blue <br> here will tweek color intensity in RGB |
|Histogram | | helps to understand distribution behind colors of an image <br> important to know when you plan on compiling a ML algorithm with balanced dataset|
|Drawings of Shapes | | ever need to have shapes to interact with computer vision world like object detection, it's common to create digital shapes to represent them|

----

#### Image Manipulation & Image Processing
Will apply following function on an image using OpenCV:
1. Image Transformations
  * Affine and Non-Affine Transformation
2. Image Translations
  * Moving image up, down, left and right 
3. Rotation of image
  * Spinning image 
4. Scaling, Resizing, and Interpolation 
5. Image Pyramids 
  * Another way of resizing 
6. Cropping
  * Cutting out wanted image region 
7. Arithmetic operations for Brightening and Darkening of images

|             |          |           |
|-------------|----------|-----------|
|Transformation | |how to transform images for rotation, scaling, bitwise pixel manipulations and edge detection <-- Why this all?? <br> before sending a picture or frame into a computer vision model, one `need to adjust features(histogram)` in order to change quality |
|Image Translation | |helps in croping picture to adjust features within input <br> Say if you needed to train an AI to detect a specific object, you would want to crop your main label and avoid pixels irrelevant to what your detecting |
|Rotations | | real time objects in an imagea needs to be trained are not properly positioned correctly to help AI understand features we want to aggregate <br> Using rotations we can help position object correctly to help train our algorithm|
|Scaling | |sometimes zooming into a picture looses pixel quality <br> With scaling in opencv, we can generate new pixels to prevent blury content with zooming in |
|Image Pyramids <br>(Resize) | |to resize images for visiual designers |
|Region of intrest <br> (Crop) | |in self driving cars we need to focus on street lanes in order to teach a car to drive by itself <br>With region of interest, we can crop out a section of an image and focus on pixels representing a street |
|Bitwise Operations <br> (Mask) | | after grayscaling an image to detect edges with high gradients <br> it's neccessary to trigger a bitwise operation and seperate white and black pixels similar to logic gates with 1's and 0's.|
|Convolutions & Blurring | | aggregating pixels can generate noise, <br> so using probability algorithms to generate new pixels like Gaussian will reduce noices and blurry content |
|Sharpening| | when a picture is blurry we can use interpolation to sharpen images|
|Thresholding| | if theres a huge intensity between black and white pixel, <br>we calcualte thershold in order to find gradients for edges in an image|
|Dilation & Erosion| |most `basic morphological operations` are <br> `dilation and erosion`<br> Dilation `adds pixels to boundaries of objects` in an image <br> while erosion `removes pixels on object boundaries`|
|Edge Detection| |identifying a variety of mathematical methods that aim at identifying points in a digital image at which image brightness changes sharply <br>or more formally has discontinuities |
|Perspective & Affine Transforms| |Affine Transform is a function between affine spaces which preserves points, straight lines and planes |















