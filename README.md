# Finding Brightest star
import cv2
import numpy
image=cv2.imread("image")
gray=cv2.cvtColor(image,cv2.COLOR_BGR2GRAY)
(minval,maxval,minloc,maxloc)=cv2.minMaxLoc(gray)
cv2.circle(image,maxloc,(400,0,0))
cv2.circle(image,maxloc,('radius'),(400,0,0))
