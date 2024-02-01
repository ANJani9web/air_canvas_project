# Air Canvas project
Computer vision project implemented with OpenCV

Have you ever desired to bring your imagination to life simply by waving your finger in the air? In this post, we will explore how to construct an Air Canvas capable of drawing anything by tracking the motion of a colored marker using a camera. Here, a colored object placed at the tip of the finger serves as the marker.

We will utilize computer vision techniques from OpenCV to develop this project. Python is the preferred language due to its extensive libraries and easy-to-use syntax. However, with a basic understanding, it can be implemented in any language supported by OpenCV.

Here Colour Detection and tracking is used in order to achieve the objective. The colour marker in detected and a mask is produced. It includes the further steps of morphological operations on the mask produced which are Erosion and Dilation. Erosion reduces the impurities present in the mask and dilation further restores the eroded main mask.

# Algorithm

1. Start reading the frames and convert the captured frames to HSV colour space.(Easy for colour detection)
2. Prepare the canvas frame and put the respective ink buttons on it.
3.. Adjust the trackbar values for finding the mask of coloured marker.
4. Preprocess the mask with morphological operations.(Erotion and dilation)
5. Detect the contours, find the center coordinates of largest contour and keep storing them in the array for successive frames .(Arrays for drawing points on canvas)
6. Finally draw the points stored in array on the frames and canvas .

Requirements: python3 , numpy , opencv installed on your system.

<!-- <img src="https://raw.githubusercontent.com/infoaryan/Air-Canvas-project/master/Screenshots/sample_project_img1.png" width="800" height="400"> -->
