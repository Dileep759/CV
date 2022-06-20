# Written-text-detection-and-segmentation-using-OpenCV.ipynb
I converted RGB image into HSV image to get lower and upper pixel values for the binary transformation of original image.
created kernel to get structuring element as a rectangle around the contours.
applied opening and closing morphologyEx methods to do morphology transformations of the binary image(mask) like Erode, Dilation etc.
Increased morphologyEx opening iterations to reduce extra white space and do extra cleaning.
found contours (object) using findContours method then found the coordinated of an object using boundingRect method.
I applied same coordinates to the original image to get ROI(Region of Interest)
Finallly I wrote result, ROI to get separate window images.
