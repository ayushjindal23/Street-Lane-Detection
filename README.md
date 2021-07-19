# Street-Lane-Detection
I would be using Canny Edge Detector and Hough Lines for the same. Their functions can be implemented using OpenCV.
## MODEL PIPELINE.
1. Read the image and convert it to RGB format. Get its height and width and define a region of interest which is required for the Lane Detection.
2. Then convert the image to GRAY format because the Canny Edge Detector takes only GRAY images as input. Pass the image to Canny Edge Detector.
3. Now, mask the image by the region of interest defined earlier.
4. Then apply Hough transform to the image which is a feature extraction technique that gives instances of objects within a certain class of shapes. In our case, the shape will be a line thus we will use HoughLines function.
5. Finally, the transform will return the detected lines and we will draw it in our image as output.
.
